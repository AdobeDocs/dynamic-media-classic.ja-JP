---
title: フォント
description: Adobe Dynamic Media Classicでのフォントの使用方法を説明します。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 28%

---

# フォント{#fonts}

Adobe Dynamic Media Classicでは、特定のフォントでテキストを入力またはレンダリングするために、フォントファイルのアップロードが必要な場合があります。 例えば、テンプレートレイヤー上のテキストの特定のフォントを使用するには、フォントファイルをアップロードします。eCatalog ビューアページ番号を特定のフォントで表示するには、フォントファイルをアップロードします。

Adobe Dynamic Media Classicでは、次のフォントタイプをサポートしています。

* すべての TrueType フォント
* PostScript®フォント
* OpenType/TrueType フォント
* OpenType/PostScript フォント
* PhotoFont

フォントファイルをアップロードした後、情報を編集画面で、Adobe Dynamic Media Classic ID、フォント名、および入力情報を変更できます。

>[!NOTE]
>
>テンプレートレイヤーでフォントを使用する場合は、すべてのフォントスタイル（太字、斜体、太字/斜体、標準）をアップロードすることをお勧めします。 Adobe Dynamic Media Classicで要求を処理するには、これらのフォントスタイルが必要です。 フォントに関連付けられているすべての PostScript/Adobe Type 1 ファイルもアップロードすることもお勧めします。これらの一部のフォントには、詳細なカーニング情報が含まれています。

## フォントファイルのアップロード {#uploading-font-files}

フォントファイルのアップロードは、その他のファイルをアップロードするのと同じ方法で行います。フォントファイルは、任意のAdobe Dynamic Media Classicフォルダーに格納できます。 詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## フォントファイル情報を編集 {#editing-font-file-information}

フォントの ID 名と種類情報を変更できます。 フォントファイルを編集することで、フォントを容易に検索および識別できるようになります。

参照パネルで、詳細ビューで編集するフォントファイルを選択し、ファイル/情報を編集を選択します。 情報を編集画面が開きます。次のオプションを選択し、「 」を選択します。 **[!UICONTROL 送信]**.

* **[!UICONTROL フォント名]**  — この名前は、フォントが公開される際にフォントを識別します。

* **[!UICONTROL PostScript 名]**  — この名前は、フォントの完全な PostScript 名です。 通常は、太さまたはスタイルを示します。

* **[!UICONTROL RTF 名]**  — この名前は、テンプレートテキストレイヤーが作成される RTF エディタのポップアップメニューに表示されます。

* **[!UICONTROL フォントファミリ名]**  — この名前は、スタイル、太さ、フォントの種類を示すインジケータを含まないフォント名をリストします。

* **[!UICONTROL フォントスタイル]**  — オプションは、「プレーン」、「太字」、「斜体」および「太字斜体」です。

* **[!UICONTROL フォントの種類]**  — オプションは TrueType とAdobe Type1 です。 これらのフォントを別の名前で呼び出す場合は、その名前を入力します。

* **[!UICONTROL フォントタイプ（省略）]**  — オプションは次のとおりです。

   * **[!UICONTROL TTF]** - TrueType フォントファイル (PDF/PostScript のレンダリングや画像サービングに使用 )。

   * **[!UICONTROL AFM]** - Adobe PostScriptフォントファイル。Adobeフォント指標情報が格納され、画像サービングに使用されます。

   * **[!UICONTROL PFM]**  — バイナリフォントメトリック情報を含むAdobe PostScriptフォントファイル。

   * **[!UICONTROL PFB]**  — バイナリフォントのアウトライン情報を含む、PDF/PostScript レンダリングや画像サービングに使用されるAdobe PostScriptフォントファイル。
