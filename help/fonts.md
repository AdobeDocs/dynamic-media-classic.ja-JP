---
title: フォント
description: Dynamic Media Classicでのフォントの使用方法を説明します。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
source-git-commit: 20a5e54a9f3fa442d3a993afae07aa5b1b13e9c3
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 33%

---

# フォント{#fonts}

Dynamic Media Classicでは、特定のフォントでテキストを入力またはレンダリングするために、フォントファイルのアップロードが必要になる場合があります。 例えば、テンプレートレイヤー上のテキストの特定のフォントを使用するには、フォントファイルをアップロードします。eCatalog ビューアページ番号を特定のフォントで表示するには、フォントファイルをアップロードします。

Dynamic Media Classicでは、次のフォントタイプをサポートしています。

* すべての TrueType フォント
* PostScript®フォント
* OpenType/TrueType フォント
* OpenType/PostScript フォント
* PhotoFont

フォントファイルをアップロードした後、情報を編集画面で、Dynamic Media Classic ID、フォント名およびタイプ情報を変更できます。

>[!NOTE]
>
>テンプレートレイヤーでフォントを使用する場合は、すべてのフォントスタイル（太字、斜体、太字/斜体、標準）をアップロードすることをお勧めします。 Dynamic Media Classicは、要求を処理するために、これらのフォントスタイルが必要です。 フォントに関連付けられているすべての PostScript/Adobe Type 1 ファイルもアップロードすることもお勧めします。これらの一部のフォントには、詳細なカーニング情報が含まれています。

## フォントファイルのアップロード {#uploading-font-files}

フォントファイルのアップロードは、その他のファイルをアップロードするのと同じ方法で行います。フォントファイルは、任意のDynamic Media Classicフォルダーに格納できます。 詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## フォントファイル情報の編集 {#editing-font-file-information}

フォントのID名と種類情報を変更できます。 フォントファイルを編集することで、フォントを容易に検索および識別できるようになります。

参照パネルで、詳細ビューで編集するフォントファイルを選択して、ファイル／情報を編集を選択します。情報を編集画面が開きます。次のオプションを選択し、「**[!UICONTROL 送信]**」を選択します。

* **[!UICONTROL フォント名]**  — フォントが公開される際にフォントを識別する名前です。

* **[!UICONTROL PostScript名]**  — フォントの完全なPostScript名です。通常は、太さまたはスタイルを示します。

* **[!UICONTROL RTF名]**  — この名前は、テンプレートテキストレイヤーが作成されるRTFエディターのポップアップメニューに表示されます。

* **[!UICONTROL フォントファミリ名]**  — この名前には、スタイル、太さ、フォントタイプのインジケーターを含まないフォント名が表示されます。

* **[!UICONTROL フォントスタイル]**  — オプションは、プレーン、太字、斜体および太字斜体です。

* **[!UICONTROL Font Type]**  - TrueTypeとAdobe Type1を選択します。これらのフォントを別の名前で呼び出す場合は、その名前を入力します。

* **[!UICONTROL フォントタイプの省略形]**  — オプションは次のとおりです。

   * **[!UICONTROL TTF]**  - PDF/PostScriptのレンダリングや画像サービングに使用されるTrueTypeフォントファイル。

   * **[!UICONTROL AFM]**  - Adobe PostScriptフォントファイル。Adobeフォントメトリック情報が含まれ、画像サービングに使用されます。

   * **[!UICONTROL PFM]**  — バイナリフォントメトリック情報を含むAdobe PostScriptフォントファイル。

   * **[!UICONTROL PFB]**  — バイナリフォントのアウトライン情報を含み、PDF/PostScriptレンダリングや画像サービングに使用されるAdobe PostScriptフォントファイル。
