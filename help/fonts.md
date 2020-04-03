---
title: フォント
seo-title: フォント
description: 'null'
seo-description: ダイナミックメディアクラシックでフォントを使用する方法を説明します。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# フォント{#fonts}

場合によっては、特定のフォントで入力したり、特定のフォントでテキストをレンダリングするのに、Scene7 Publishing System でフォントファイルをアップロードするよう求められることがあります。例えば、テンプレートレイヤー上のテキストの特定のフォントを使用するには、フォントファイルをアップロードします。eCatalog ビューアページ番号を特定のフォントで表示するには、フォントファイルをアップロードします。

Dynamic Media Classicは、次のフォントタイプをサポートしています。

* すべての TrueType フォント
* PostScript®フォント
* OpenType/TrueType フォント
* OpenType/PostScript フォント
* PhotoFont

フォントファイルをアップロードした後に、SPS ID、フォント名、および種類に関する情報を、情報を編集画面で変更することができます。

>[!NOTE]
>
>テンプレートレイヤーでフォントを使用する場合は、すべてのフォントスタイル（太字、斜体、太字/斜体および標準）をアップロードすることをお勧めします。 Dynamic Media Classicでは、要求を処理するためにこれらのフォントスタイルが必要です。 フォントに関連付けられているすべての PostScript/Adobe Type 1 ファイルもアップロードすることもお勧めします。これらの一部のフォントには、詳細なカーニング情報が含まれています。

## フォントファイルのアップロード {#uploading-font-files}

フォントファイルのアップロードは、その他のファイルをアップロードするのと同じ方法で行います。フォントファイルは、あらゆる SPS フォルダに入れることができます。詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## フォントファイル情報の編集 {#editing-font-file-information}

フォントの ID 名に加え、種類に関する情報を変更することができます。フォントファイルを編集することで、フォントを容易に検索および識別できるようになります。

参照パネルで、詳細ビューで編集するフォントファイルを選択して、ファイル／情報を編集を選択します。情報を編集画面が開きます。次のオプションを選択して、「送信」ボタンを選択します。

**[フォント名** ]発行時のフォントを示す名前です。

**PostScript名** ：この名前は、フォントの完全なPostScript名です。 通常は、太さまたはスタイルを示します。

**RTF名** ：この名前は、テンプレートテキストレイヤーが作成されるRTFエディタのポップアップメニューに表示されます。

**[フォントファミリ名** ]この名前は、スタイル、重み付け、またはフォントタイプのインジケーターを除くフォント名をリストします。

**フォントスタイル** ：標準、太字、斜体、太字斜体のオプションがあります。

**Font Type** TrueTypeとAdobe Type 1を選択できます。 これらのフォントを別の名前で呼び出す場合は、その名前を入力します。

**フォントの種類の省略形** ：次のオプションがあります。

**PDF/PostScriptのレンダリングと画像サービングに使用されるTTF** TrueTypeフォントファイル。

**Adobe Font Metrics情報を含み、画像サービングに使用されるAFM** Adobe PostScriptフォントファイル。

**バイナリフォントメトリック情報を含むPFM** Adobe PostScriptフォントファイル。

**PFB** Adobe PostScriptフォントファイル。バイナリフォントのアウトライン情報が含まれ、PDF/PostScriptのレンダリングと画像サービングに使用されます。
