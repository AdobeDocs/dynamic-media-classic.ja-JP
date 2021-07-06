---
title: 画像アセットまたはベクトルアセットのアップロード
description: 画像アセットまたはベクトルアセットをアップロードする方法を説明します。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: 2ef78fe6-1e7c-4f48-86da-137ddaa55bbf
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1497'
ht-degree: 78%

---

# 画像アセットまたはベクトルアセットのアップロード{#uploading-an-image-asset-or-a-vector-asset}

画像アセットをアップロードするには、その前に共有秘密キーを要求する必要があります。この共有秘密キーを、アップロードトークンの取得に使用します。取得したら、このアップロードトークンを使用して、画像アセットまたはベクトルアセットをアップロードします。

## 共有秘密キーの要求 {#requesting-a-shared-secret-key}

Admin Consoleを使用して&#x200B;*共有秘密鍵*&#x200B;を[に要求し、サポートケースを作成します。](https://helpx.adobe.com/enterprise/admin-guide.html/enterprise/using/support-for-experience-cloud.ug.html) サポートケースで、共有秘密鍵をリクエストします。

電子メールの本文には、画像アセットのアップロードに使用する会社名を記載してください。Dynamic Media Classicからキーを受け取ったら、後で使用するためにローカルに保存します。

## アップロードトークンの取得 {#retrieving-the-upload-token}

*アップロードトークン*&#x200B;は、ほかのユーザが同じ共有秘密キーを使用してアセットをアップロードすることができないようにします。つまり、アップロードの合法性とソースの信頼性を確保します。

アップロードトークンは英数字で構成された文字列で、一定の期間しか利用できません。共有秘密鍵を代わりに次のURLを使用して、アップロードトークンを取得できます。

* 画像
   `https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602`この例では、共有秘密鍵は  `fece4b21-87ee-47fc-9b99-2e29b78b602`

* ベクトル
   `https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9`この例では、共有秘密鍵は  `2d19f60e-890a-4e79-a1a5-9ac2875429b9`

初期設定で、アップロードトークンは取得後 5 分（300 秒）で有効期限切れになります。期限を延長するには、URL に `expires` パラメータを追加し、必要とする時間を秒単位で入力します。例えば、次のサンプル画像の URL では、1800 秒間有効なアップロードトークンを取得します。

```as3
https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=1800
```

画像に対する成功応答は、次のようになります。

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
|--- |--- |--- |
| op | 必須 | get_uploadtoken |
| shared_secret | 必須 | アップロードを行う会社の共有秘密キー。 |
| expires | オプション | アップロードトークンの有効秒数。指定しない場合は、初期設定の 300 秒になります。 |

**サンプル画像の URL：**

`https://s7ugc1.scene7.com/ugc/image?op=get_uploadtoken&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&expires=600`

**ベクトル URL例：**

`https://s7ugc1.scene7.com/ugc/vector?op=get_uploadtoken&shared_secret=2d19f60e-890a-4e79-a1a5-9ac2875429b9&expires=5000`

**許可されているHTTPメソッド：**
`GET` および  `POST`

これで、画像アセットをアップロードできるようになりました。

詳しくは、[画像アセットのアップロード](uploading-image-asset-or-vector.md#uploading_an_image_asset)を参照してください。

## 画像アセットのアップロード {#uploading-an-image-asset}

一定時間有効なアップロードトークンを取得したら、画像アセットをアップロードできます。この例では、マルチパート／フォームとしてアセットをアップロードし、残りの値を URL クエリ文字列として送信します。

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company
```

`upload_token`フィールドと`company_name`フィールドは必須です。

詳しくは、[アップロードトークンの取得](uploading-image-asset-or-vector.md#retrieving_the_upload_token)を参照してください。

詳しくは、[共有秘密キーの取得](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)を参照してください。

この例のように、他のオプションの値も URL クエリ文字列として送信できます。

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=jpg,gif
```

`file_limit`パラメーターは、ファイルサイズの制限をバイト単位で指定します。 `file_exts` パラメータでは、アップロード可能なファイル名拡張子を指定します。この 2 つのパラメータはオプションです。

ファイルサイズ制限とファイル名拡張子に適用されるグローバル制限は、アプリケーション内で設定されます。要求での送信内容がグローバル制限のサブセットの場合は、この制限が適用されます。グローバル制限は次のとおりです。

| グローバル制限 | 値 |
|--- |--- |
| すべてのクライアントのファイルサイズ | 20MB |
| アップロードでサポートされている画像ファイルの形式 | BMP、GIF、JPG、PNG、PSD |

アセットのアップロードには次の HTML フォームを使用できます。フォームからは次の情報の入力が求められます。

* 会社名.
* アップロードトークン.
* ファイルサイズ制限.
* ファイル名拡張子のリスト.
* アセットに関連付けられたカラープロファイルとファイル名を保持するかどうか。
* ノックアウトの背景を使用するかどうか。 [ノックアウトの背景]を有効にした場合は、[コーナー]、[許容差]、および[塗りつぶし方法]を設定します。
[アップロード時の画像編集オプションの「ノックアウトの背景」を参照してください。](image-editing-options-upload.md#image-editing-options-at-upload)
* アップロードするファイルの名前.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

上記のフォームに関連付けられたHTMLソースコードを表示するには、[https://s7ugc1.scene7.com/ugc/upload.html](https://s7ugc1.scene7.com/ugc/upload.html)

Firefoxで、ブラウザーウィンドウを右クリックし、「**[!UICONTROL ページソースを表示]**」をクリックします。 コードには、該当する URL クエリ文字列と、ユーザが&#x200B;**[!UICONTROL 「送信」]**&#x200B;をクリックしたときに実行される POST メソッドが表示されます。

XML 応答を Internet Explorer で表示するには、**[!UICONTROL 表示]**／**[!UICONTROL ソース]**&#x200B;をクリックします。FirefoxでXML応答を表示するには、**[!UICONTROL ツール]** / **[!UICONTROL ブラウザーツール]** / **[!UICONTROL Web開発者ツール]**&#x200B;をクリックします。 XML 応答の表示には、Firefox を使用することをお勧めします。

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

ほかの ImageServing リソースの場合と同様に、アセットには処理クエリを適用できます。例えば、以下の URL は、指定された幅と高さにストレッチされたアセットを要求します。

```as3
https://s7w2p1.scene7.com/is/image/S7WebUGC/ugc/9536356.tif?&wid=800&hei=100&fit=stretch
```

アップロードするアセットをマルチパート／フォームとしてアップロードし、残りの値を URL クエリ文字列として送信します。URL クエリ文字列で以下のフィールドを使用して、アセットをアップロードできます。

| URL パラメータ | 必須またはオプション | 値 |
|--- |--- |--- |
| `op` | 必須 | アップロード |
| `upload_token` | 必須 | 会社と関連付けられている共有秘密キーに対応するアップロードトークン。 |
| `company_name` | 必須 | アップロードを実行する会社の名前。 |
| `file_limit` | オプション | アセットのファイルサイズ制限（バイト単位）。 |
| `file_exts` | オプション | 画像アセットファイルで許可される拡張子のリスト。 |
| `preserve_colorprofile` | オプション | アップロードされたファイルを PTIFF 形式に変換するときに埋め込まれているカラープロファイルを保持します。値は true または false。初期設定は false。. |
| `preserve_filename` | オプション | アップロードされたアセットのファイル名を保持します。値は true または false。初期設定は false。. |

>[!NOTE]
>
>アップロードするアセットは、マルチパート POST 要求の唯一のフィールドとして送信する必要があります。

**サンプル URL：**

`https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d-312094e0ef20_18000&company_name=000Company`

**使用可能な HTTP メソッド：**

POST

### 画像のアセットメタデータの取得 {#getting-asset-metadata-for-images}

`image_info` を使用して、アップロードしたアセットのメタデータを取得できます。次に例を示します。

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
|--- |--- |--- |
| `op` | 必須 | image_info |
| `shared_secret` | 必須 | 会社の共有秘密キー. |
| `image_name` | 必須 | 画像の名前。 |

**サンプル URL：**

`https://s7ugc1.scene7.com/ugc/image?op=image_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**使用可能な HTTP メソッド：**

GET と POST

## ベクトルアセットのアップロード {#uploading-a-vector-asset}

一定時間有効なアップロードトークンを取得したら、ベクトルアセットをアップロードできます。この例では、マルチパート／フォームとしてアセットをアップロードし、残りの値を URL クエリ文字列として送信します。

```as3
https://s7ugc1.scene7.com/ugc/image?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company
```

`upload_token`フィールドと`company_name`フィールドは必須です。

詳しくは、[アップロードトークンの取得](uploading-image-asset-or-vector.md#retrieving_the_upload_token)を参照してください。

詳しくは、[共有秘密キーの取得](uploading-image-asset-or-vector.md#requesting_a_shared_secret_key)を参照してください。

この例のように、他のオプションの値も URL クエリ文字列として送信できます。

```as3
https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_token=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company&file_limit=2000000&file_exts=ai,pdf
```

`file_limit`パラメーターは、ファイルサイズの制限をバイト単位で指定します。 `file_exts` パラメータでは、アップロード可能なファイル名拡張子を指定します。この 2 つのパラメータはオプションです。

ファイルサイズ制限とファイル名拡張子に適用されるグローバル制限は、アプリケーション内で設定されます。要求での送信内容がグローバル制限のサブセットの場合は、この制限が適用されます。グローバル制限は次のとおりです。

| グローバル制限 | 値 |
|--- |--- |
| すべてのクライアントのファイルサイズ | 20MB |
| アップロードでサポートされているベクトルファイルの形式 | AI、EPS、PDF（以前、PDF ファイルが Adobe Illustrator CS6 で開いて保存されている場合のみ） |

アセットのアップロードには次の HTML フォームを使用できます。フォームからは次の情報の入力が求められます。

* 会社名.
* アップロードトークン.
* ファイルサイズ制限.
* ファイル名拡張子のリスト.
* アセットに関連付けられたカラープロファイルとファイル名を保持するかどうか。
* ノックアウトの背景を使用するかどうか。 [ノックアウトの背景]を有効にした場合は、[コーナー]、[許容差]、および[塗りつぶし方法]を設定します。
[アップロード時の画像編集オプションの「ノックアウトの背景」を参照してください。](image-editing-options-upload.md#image-editing-options-at-upload)
* アップロードするファイルの名前.

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Art Spec: If not leaving art spec, delete only the first of the 2 &lt;draft-comment> elements under &lt;adobefig>.</p>

 -->

次のHTMLコードは、ブラウザーウィンドウで右クリックし、例に示すフォームの「**[!UICONTROL ソースを表示]**」をクリックすると表示されます。 コードには、該当する URL クエリ文字列と、ユーザが&#x200B;**[!UICONTROL 「送信」]**&#x200B;をクリックしたときに実行される POST メソッドが表示されます。

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
<td><strong>Click Submit to upload your Vector: </strong></td> 
<td><input type="submit" value="Submit"></td> 
</tr> 
</table> 
</form> 
</body>
```

XML 応答を Internet Explorer で表示するには、**[!UICONTROL 表示]**／**[!UICONTROL ソース]**&#x200B;をクリックします。FirefoxでXML応答を表示するには、**[!UICONTROL ツール]** / **[!UICONTROL ブラウザーツール]** / **[!UICONTROL ページソース]**&#x200B;をクリックします。 XML 応答の表示には、Firefox を使用することをお勧めします。

以下は、アップロードが正常に完了した場合のサンプル応答です。

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
>アップロードされたアセット（AI、EPS、PDF など）は FXG 形式に変換され、応答ではその FXG アセットへの直接リンクが送信されます。

アセットは、他のWeb-to-Printリソースと同様です。処理クエリを適用します。 例えば、次の URL は FXG リソースを 500x500 png 画像に変換します。

```as3
https://s7w2p1.scene7.com/is/agm/W2PTest/ugc/8875744.fxg?fmt=png&wid=500&hei=500
```

アップロードするアセットをマルチパート／フォームとしてアップロードし、残りの値を URL クエリ文字列として送信します。URL クエリ文字列で以下のフィールドを使用して、アセットをアップロードできます。

| URL パラメータ | 必須またはオプション | 値 |
|--- |--- |--- |
| `op` | 必須 | アップロード |
| `upload_token` | 必須 | 会社と関連付けられている共有秘密キーに対応するアップロードトークン。 |
| `company_name` | 必須 | アップロードを実行する会社の名前。 |
| `file_limit` | オプション | アセットのファイルサイズ制限（バイト単位）。 |
| `file_exts` | オプション | アセットファイルで使用できる拡張子のリスト。 |

>[!NOTE]
>
>アップロードするアセットは、マルチパート POST 要求の唯一のフィールドとして送信する必要があります。

**サンプル URL：**

`https://s7ugc1.scene7.com/ugc/vector?op=upload&upload_to ken=aa2a378a-cd25-4c80-994d- 312094e0ef20_18000&company_name=000Company`

**使用可能な HTTP メソッド：**

POST
