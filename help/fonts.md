---
title: フォント
seo-title: フォント
description: 'null'
seo-description: Dynamic Mediaクラシックのフォントの使い方を学びます。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 40%

---


# フォント{#fonts}

場合によっては、Dynamic Mediaクラシックで、特定のフォントでテキストを入力またはレンダリングするために、フォントファイルのアップロードが必要になります。 例えば、テンプレートレイヤー上のテキストの特定のフォントを使用するには、フォントファイルをアップロードします。eCatalog ビューアページ番号を特定のフォントで表示するには、フォントファイルをアップロードします。

Dynamic Mediaクラシックでは、次のフォントタイプをサポートしています。

* すべての TrueType フォント
* PostScript®フォント
* OpenType/TrueType フォント
* OpenType/PostScript フォント
* PhotoFont

フォントファイルをアップロードした後、情報を編集画面で、Dynamic MediaクラシックID、フォント名および種類の情報を変更できます。

>[!NOTE]
>
>テンプレートレイヤーでフォントを使用する場合は、すべてのフォントスタイル（太字、斜体、太字/斜体、標準）をアップロードすることをお勧めします。 Dynamic Mediaクラシックでは、要求を処理する際に、これらのフォントスタイルが必要です。 フォントに関連付けられているすべての PostScript/Adobe Type 1 ファイルもアップロードすることもお勧めします。これらの一部のフォントには、詳細なカーニング情報が含まれています。

## フォントファイルのアップロード  {#uploading-font-files}

フォントファイルのアップロードは、その他のファイルをアップロードするのと同じ方法で行います。フォントファイルは、任意のDynamic Mediaクラシックフォルダーに格納できます。 詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## フォントファイル情報の編集  {#editing-font-file-information}

フォントの ID 名に加え、種類に関する情報を変更することができます。フォントファイルを編集することで、フォントを容易に検索および識別できるようになります。

参照パネルで、詳細ビューで編集するフォントファイルを選択して、ファイル／情報を編集を選択します。情報を編集画面が開きます。次のオプションを選択して、「送信」ボタンを選択します。

**フォント** 名この名前は、フォントが公開されるときにフォントを識別します。

**PostScript** Name：フォントの完全なPostScript名です。通常は、太さまたはスタイルを示します。

**RTF** 名この名前は、テンプレートテキストレイヤーが作成されるRTFエディタのポップアップメニューに表示されます。

**フォントファミリ** ー名この名前は、スタイル、重み付け、またはフォントの種類を示すインジケーターを除くフォント名をリストします。

**フォント** スタイルオプションは、標準、太字、斜体、太字斜体です。

**フォント** の種類TrueTypeとAdobeの種類1を指定できます。これらのフォントを別の名前で呼び出す場合は、その名前を入力します。

**フォントタイプ** 省略形オプションは次のとおりです。

**PDF/PostScriptのレンダリングと画像サービングに使用される** TTFTrueTypeフォントファイル。

**adobeフォントメトリクス情報が含まれ、画像サービングに使用される** AFMAdobe PostScriptフォントファイル。

**バイナリフォントメトリック情報を含む** PFMAdobe PostScriptフォントファイル。

**バイナリフォントのアウトライン情報が含まれ、PDF/PostScriptのレンダリングと画像サービングに使用される** PFBAdobe PostScriptフォントファイル。
