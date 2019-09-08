---
title: フォント
seo-title: フォント
description: 'null'
seo-description: Dynamic Media Classicでフォントを使用する方法について説明します。
uuid: bdec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/support_ files
discoiquuid: 97cecd6a-30aa-44fe- a611- fd71b02fd5ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# フォント{#fonts}

場合によっては、特定のフォントで入力したり、特定のフォントでテキストをレンダリングするのに、Scene7 Publishing System でフォントファイルをアップロードするよう求められることがあります。例えば、テンプレートレイヤー上のテキストの特定のフォントを使用するには、フォントファイルをアップロードします。eCatalog ビューアページ番号を特定のフォントで表示するには、フォントファイルをアップロードします。

Dynamic Media Classicでは、次のフォントタイプをサポートしています。

* すべての TrueType フォント
* PostScript®フォント
* OpenType/TrueType フォント
* OpenType/PostScript フォント
* PhotoFont

フォントファイルをアップロードした後に、SPS ID、フォント名、および種類に関する情報を、情報を編集画面で変更することができます。

>[!NOTE]
>
>テンプレートレイヤーでフォントを使用する予定がある場合は、Dynamic Media Classicですべてのフォントスタイル（太字、斜体、太字/斜体、標準）をアップロードすることをお勧めします。Dynamic Media Classicでは、リクエストを処理するためにこれらのフォントスタイルが必要です。フォントに関連付けられているすべての PostScript/Adobe Type 1 ファイルもアップロードすることもお勧めします。これらの一部のフォントには、詳細なカーニング情報が含まれています。

## フォントファイルのアップロード {#uploading-font-files}

フォントファイルのアップロードは、その他のファイルをアップロードするのと同じ方法で行います。フォントファイルは、あらゆる SPS フォルダに入れることができます。詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## フォントファイル情報の編集 {#editing-font-file-information}

フォントの ID 名に加え、種類に関する情報を変更することができます。フォントファイルを編集することで、フォントを容易に検索および識別できるようになります。

参照パネルで、詳細ビューで編集するフォントファイルを選択して、ファイル／情報を編集を選択します。情報を編集画面が開きます。次のオプションを選択して、「送信」ボタンを選択します。

**フォント名** この名前は、公開時にフォントを識別します。

**PostScript名前** この名前は、フォントの完全なPostScript名です。通常は、太さまたはスタイルを示します。

**RTF名前** この名前は、テンプレートテキストレイヤーが作成されるRTFエディタのポップアップメニューに表示されます。

**Font Family Name** この名前には、スタイル、太さ、フォントタイプのインジケータのないフォント名が表示されます。

**フォントスタイル** 「標準」、「太字」、「斜体」、「太字斜体」のオプションがあります。

**フォントの種類** :オプションはTrueTypeおよびAdobe Type1です。これらのフォントを別の名前で呼び出す場合は、その名前を入力します。

**フォントタイプの省略形** 選択肢は次のとおりです。

**PDF/PostScriptレンダリングおよび画像サービングに使用されるTTF** TrueTypeフォントファイル。

**Adobe Font Metrics情報を含むAFM** Adobe PostScriptフォントファイル。画像サービングに使用されます。

**バイナリフォントメトリック情報を含むPFM** Adobe PostScriptフォントファイル。

**バイナリフォントアウトライン情報を含むPFB** Adobe PostScriptフォントファイル。PDF/PostScriptレンダリングと画像サービングに使用されます。
