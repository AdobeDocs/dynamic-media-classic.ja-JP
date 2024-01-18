---
title: ラスター画像アセットをアップロードする
description: ラスター画像アセットをAdobe Dynamic Media Classicにアップロードする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
topic: Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 55%

---

# ラスター画像アセットをアップロードする {#uploading-an-image-asset-or-a-vector-asset}

画像アセットをアップロードするには、その前に共有秘密キーを要求する必要があります。この共有秘密キーを、アップロードトークンの取得に使用します。次に、アップロードトークンを使用して、ラスター画像アセットをアップロードします。

>[!IMPORTANT]
>
>2023 年 5 月 1 日以降、Dynamic Mediaの UGC アセットは、アップロード日から最大 60 日間使用できます。 60 日後にアセットが削除されます。

>[!NOTE]
>
>Adobe Dynamic Media Classicでの新規または既存の UGC ベクトルアセットのサポートは、2021 年 9 月 30 日に終了しました。

## 共有秘密鍵のリクエスト {#requesting-a-shared-secret-key}

リクエスト a *共有秘密鍵* 作成者 [Admin Consoleを使用してサポートケースを作成します。](https://helpx.adobe.com/enterprise/using/support-for-experience-cloud.html) サポートケースで、共有秘密鍵をリクエストします。

電子メールの本文には、画像アセットのアップロードに使用する会社名を記載してください。Adobe Dynamic Media Classicからキーを受け取ったら、後で使用するためにローカルに保存します。

## アップロードトークンの取得 {#retrieving-the-upload-token}

*アップロードトークン*&#x200B;は、ほかのユーザが同じ共有秘密キーを使用してアセットをアップロードすることができないようにします。つまり、アップロードの合法性とソースの信頼性を確保します。

アップロードトークンは英数字で構成された文字列で、一定の期間しか利用できません。アップロードトークンを取得できるよう、共有秘密鍵に代わって、次の URL を使用します。

* ラスターイメージ
  `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`この例では、共有秘密鍵はです。 `fece4b21-87ee-47fc-9b99-2e29b78b602`

<!-- * Vector
  `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`In this example, the shared-secret key is `2d19f60e-890a-4e79-a1a5-9ac2875429b9` -->

初期設定で、アップロードトークンは取得後 5 分（300 秒）で有効期限切れになります。さらに時間をリクエストするには、以下を含めます。 `expires` を指定し、必要な時間を秒単位で指定します。 例えば、次のサンプル画像の URL では、1800 秒間有効なアップロードトークンを取得します。

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

画像の成功応答は、次のようになります。

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
        <serviceName>User Generated Content - Images</serviceName> 
        <version>1.0.0</version> 
        <operationName>get_uploadtoken</operationName> 
        <serviceStatus>SUCCESS</serviceStatus> 
        <title>Upload Token for fece4b21-87ee-47fc-9b99-2e29b78b602</title> 
        <message> 
            <uploadtoken>aa2a378a-cd25-4c80-994d-312094e0ef20_1800</uploadtoken> 
            <expiration_in_seconds>1800</expiration_in_seconds> 
        </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

今後の要求で使用できるように、アップロードトークンをローカルに保存します。

クエリ URL 文字列で以下のフィールドを使用して、アップロードトークンを取得できます。

| URL パラメータ | 必須またはオプション | 値 |
| --- | --- | --- |
| op | 必須 | get_uploadtoken |
| shared_secret | 必須 | アップロードをおこなう会社の共有秘密鍵。 |
| 有効期限 | オプション | アップロードトークンの有効秒数。指定しない場合は、初期設定の 300 秒になります。 |

**サンプルのラスターイメージ URL:**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000` -->

**許可されている HTTP メソッド：**
`GET` および `POST`

これで、画像アセットをアップロードできるようになりました。

詳しくは、 [画像アセットのアップロード](uploading-image-asset-or-vector.md#uploading_an_image_asset).

## ラスター画像アセットをアップロードする {#uploading-an-image-asset}

一定時間有効なアップロードトークンを取得したら、画像アセットをアップロードできます。この例では、マルチパート／フォームとしてアセットをアップロードし、残りの値を URL クエリ文字列として送信します。

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

The `upload_token` および `company_name` フィールドは必須です。

詳しくは、 [アップロードトークンの取得](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

詳しくは、 [共有秘密鍵の取得](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

この例のように、他のオプションの値も URL クエリ文字列として送信できます。

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

The `file_limit` パラメータは、ファイルサイズの制限をバイト単位で指定します。 The `file_exts` パラメーターは、アップロード可能なファイル名拡張子を指定します。 この 2 つのパラメータはオプションです。

ファイルサイズ制限とファイル名拡張子に適用されるグローバル制限は、アプリケーション内で設定されます。要求での送信内容がグローバル制限のサブセットの場合は、この制限が適用されます。グローバル制限は次のとおりです。

| グローバル制限 | 値 |
| --- | --- |
| すべてのクライアントのファイルサイズ | 20MB |
| アップロードでサポートされている画像ファイルの形式 | BMP、GIF、JPG、PNG、PSD、TIFF |

アセットのアップロードには次の HTML フォームを使用できます。フォームからは次の情報の入力が求められます。

* 会社名。
* アップロードトークン。
* ファイルサイズの制限。
* ファイル名拡張子のリスト。
* アセットに関連付けられたカラープロファイルとファイル名を保持するかどうか。
* ノックアウトの背景を使用するかどうかを指定します。 [ ノックアウトの背景 ] を有効にした場合は、[ コーナー ]、[ 公差 ]、[ 塗り潰し方法 ] を設定します。
詳しくは、 [アップロード時の画像の微調整オプション](image-editing-options-upload.md#image-editing-options-at-upload).
* アップロードするファイルの名前。

上のフォームに関連付けられたHTMLのソースコードを表示するには、「 」を選択します。 [https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Firefox で、ブラウザーウィンドウを右クリックし、「 」を選択します。 **[!UICONTROL ページのソースを表示]**. このコードは、対応する URL クエリ文字列と、ユーザーが「 」を選択したときに実行されるPOSTメソッドを示します **[!UICONTROL 送信]**.

Internet Explorer で XML 応答を表示するには、に移動します。 **[!UICONTROL 表示]** > **[!UICONTROL ソース]**. Firefox で XML 応答を表示するには、に移動します。 **[!UICONTROL ツール]** > **[!UICONTROL ブラウザーツール]** > **[!UICONTROL Web 開発者ツール]**. XML 応答の表示には、Firefox を使用することをお勧めします。

以下は、アップロードが正常に完了した場合のサンプル応答です。

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>upload</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Your file has been uploaded Successfully.</title> 
            <message> 
            <url>https://s7w2p1.scene7.com/is/image/ </url> 
            <path>000Company/ugc/1442564.tif</path> 
            <fullurl>https://s7w2p1.scene7.com/is/image/000Company/ugc/1442564.tif </fullurl> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

>[!NOTE]
>
>アップロードされたアセット（JPG、GIF など）は PTIFF 形式に変換され、応答ではその PTIFF アセットへの直接リンクが送信されます。

ほかの ImageServing リソースの場合と同様に、アセットには処理クエリを適用できます。例えば、次の URL は、指定された幅と高さに引き伸ばされたアセットを要求します。

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

アップロードするアセットをマルチパート／フォームとしてアップロードし、残りの値を URL クエリ文字列として送信します。URL クエリ文字列で以下のフィールドを使用して、アセットをアップロードできます。

| URL パラメータ | 必須または任意 | 値 |
| --- | --- | --- |
| `op` | 必須 | アップロード |
| `upload_token` | 必須 | 会社と関連付けられている共有秘密キーに対応するアップロードトークン。 |
| `company_name` | 必須 | アップロードを実行する会社の名前。 |
| `file_limit` | オプション | アセットのファイルサイズ制限（バイト単位）。 |
| `file_exts` | オプション | 画像アセットファイルで許可される拡張子のリスト。 |
| `preserve_colorprofile` | オプション | アップロードされたファイルを PTIFF 形式に変換するときに埋め込まれているカラープロファイルを保持します。値は true または false。初期設定は false。 |
| `preserve_filename` | オプション | アップロードされたアセットのファイル名を保持します。値は true または false。初期設定は false。 |

>[!NOTE]
>
>アップロードするアセットは、マルチパート POST 要求の唯一のフィールドとして送信する必要があります。

**サンプル URL：**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**使用可能な HTTP メソッド：**

POST

### 画像のアセットメタデータの取得 {#getting-asset-metadata-for-images}

以下を使用できます。 `image_info` アップロードしたアセットのメタデータを取得する方法を次の例に示します。

```as3
https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

成功した応答の例は次のようになります。

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>image_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>More information on 1442564.tif</title> 
            <message> 
            File created on Tue Sep 08 19:02:04 CDT 2009, File Size = 243494 bytes 
            <imageFormat>Tiff</imageFormat> 
            <colorSpace>Rgb</colorSpace> 
            <width>686</width> 
            <height>457</height> 
            </message> 
        </response> 
    </user_generated_content> 
</scene7>
```

URL クエリ文字列で以下のフィールドを使用して、アセットの情報を要求できます。

| URL パラメータ | 必須またはオプション | 値 |
| --- | --- | --- |
| `op` | 必須 | image_info |
| `shared_secret` | 必須 | 会社の共有秘密鍵。 |
| `image_name` | 必須 | 画像の名前。 |

**サンプル URL：**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**使用可能な HTTP メソッド：**

GET と POST

<!-- ## Upload a vector asset {#uploading-a-vector-asset}

>[!IMPORTANT]
>
>Support for new or existing UGC vector image assets in Adobe Dynamic Media Classic end on September 30, 2021.

After you retrieve an upload token that is valid for a specific amount of time, you can upload a vector asset. You upload the asset as a multipart/form post while sending the rest of the values as a URL query string, as shown in this example:

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

The `upload_token` and `company_name` fields are required.

See [Retrieve the upload token](uploading-image-asset-or-vector.md#retrieving_the_upload_token).

See [Retrieve a shared-secret key](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key).

You can also send other optional values as URL query strings, as in this example:

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

The `file_limit` parameter specifies the file-size limit in bytes. The `file_exts` parameter specifies the filename extensions that are allowed for upload. Both of these values are optional.

A global limit is set in the application for the file size limit and the filename extensions allowed. If what you send in the request is a subset of the global limits, it is honored. The global limits are the following:

| Global limit | Value |
| --- | --- |
| File size for all clients | 20 MB |
| Supported vector file formats for upload | AI, EPS, PDF (only when the PDF is previously opened and saved in Adobe Illustrator CS6) |

The following HTML form lets a user upload an asset. The form asks the user to enter the following information:

* A company name.
* An upload token.
* A file size limit.
* A list of filename extensions.
* Whether to preserve the color profile and file name associated with the asset.
* Whether to use Knockout Background. If you enable Knockout Background, set the Corner, Tolerance, and Fill Method.
See Knockout Background in [Image fine-tuning options at upload](image-editing-options-upload.md#image-editing-options-at-upload).
* The name of the file to upload.

The following HTML code is displayed when you right-click in the browser window, and then select **[!UICONTROL View Source]** for the form shown in the example. The code shows the corresponding URL query string and the POST method that are run when the user selects **[!UICONTROL Submit]**.

```as3
<body> 
<script language="javascript"> 
function uploadImage() 
{ 
document.image_upload.action="vector?op=upload&company_name="+document.image_upload.company_name.value+"&upload_token="+document.image_upload.upload_token.value+"&file_limit="+document.image_upload.file_limit.value+"&file_exts="+document.image_upload.file_exts.value; 
return true; 
} 
</script> 
<form method="POST" enctype="multipart/form-data" name="image_upload" id="image_upload" onSubmit="return uploadImage();"> 
<table> 
<tr><td colspan="2"><strong> UGC Vector Upload Test Page: </strong></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr><td><strong> Company Name</strong></td><td><input type="text" size="40" name="company_name"></td></tr> 
<tr><td><strong> Upload Token </strong></td><td><input type="text" size="40" name="upload_token"></td></tr> 
<tr><td><strong> File Size Limit (in bytes) </strong></td><td><input type="text" size="40" name="file_limit"> bytes</td></tr> 
<tr><td><strong> File Extensions allowed </strong></td><td><input type="text" size="40" name="file_exts"></td></tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>File to upload: : </strong></td> 
<td><input name="filename" type="file" id="filename" size="58" maxlength="1024" /></td> 
</tr> 
<tr><td colspan="2"></td></tr> 
<tr> 
<td><strong>Select Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

To view the XML response in Internet Explorer, go to **[!UICONTROL View]** > **[!UICONTROL Source]**. To view XML response in Firefox, go to **[!UICONTROL Tools]** > **[!UICONTROL Browser Tools]** > **[!UICONTROL Page Source]**. Firefox is recommended for viewing XML responses.

The following is a sample response from a successful upload:

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
    <scene7> 
    <user_generated_content> 
    <response> 
    <serviceName>User Generated Content -Vector</serviceName> 
    <version>1.0.0</version> 
    <operationName>upload</operationName> 
    <serviceStatus>SUCCESS</serviceStatus> 
    <title>Your file has been uploaded Successfully.</title> 
    <message> 
    <url>https://s7w2p1.scene7.com/is/agm</url> 
    <path>W2PTest/ugc/8875744.fxg</path> 
    <fullurl> 
        https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg 
    </fullurl> 
</message> 
</response> 
</user_generated_content> 
</scene7>
```

>[!NOTE]
>
>The uploaded asset (AI, EPS, PDF so on) is converted to the FXG format and the response sends a direct link to that FXG asset.

The asset is like any other Web-to-print resource; you apply processing queries to it. For example, the following URL converts an FXG resource into a 500x500 png image.

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

Send the asset to upload as a multipart/form post while sending the rest of the values as a URL query string. You can use the following fields in the URL query string to upload an asset:

| URL Parameter | Required or Optional | Value |
| --- | --- | --- |
| `op` | Required | upload |
| `upload_token` | Required | Upload token for the shared-secret key associated with the company. |
| `company_name` | Required | Name of the company performing the upload. |
| `file_limit` | Optional | File size limit, in bytes, for the asset. |
| `file_exts` | Optional | List of allowable extensions for the asset file. |

>[!NOTE]
>
>You are required to send the asset to be uploaded as the only field in a multipart POST request.

**Sample URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**Allowed HTTP method:**

POST
 -->