---
title: フォント
description: Adobe Dynamic Media Classicでフォントを使用する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 23%

---

# フォント{#fonts}

Adobe Dynamic Media Classicでは、特定のフォントでテキストを入力またはレンダリングするために、フォントファイルをアップロードする必要がある場合があります。 例えば、テンプレートレイヤー上のテキストの特定のフォントを使用するには、フォントファイルをアップロードします。eCatalog ビューアページ番号を特定のフォントで表示するには、フォントファイルをアップロードします。

Adobe Dynamic Media Classicでは、次のフォントタイプをサポートしています。

* すべての TrueType フォント
* PostScript® フォント
* OpenType/TrueType フォント
* OpenType/PostScript フォント
* PhotoFont

フォントファイルをアップロードしたら、情報編集画面でAdobe Dynamic Media Classic ID、フォント名、タイプ情報を変更できます。

>[!NOTE]
>
>Adobe Dynamic Media Classicでは、テンプレートレイヤーでフォントを使用する予定がある場合に、すべてのフォントスタイル（太字、斜体、太字/斜体、標準）をアップロードすることをお勧めします。 Adobe Dynamic Media Classicがリクエストを処理するには、これらのフォントスタイルが必要です。 フォント `PostScript/Adobe Type1` 詳細なカーニング情報が含まれるフォントもあるため、フォントに関連付けられているすべてのファイルをアップロードすることをお勧めします。

## フォントファイルのアップロード {#uploading-font-files}

フォントファイルのアップロードは、その他のファイルをアップロードするのと同じ方法で行います。フォントファイルは任意のAdobe Dynamic Media Classic フォルダーに保存できます。 詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## フォントファイル情報の編集 {#editing-font-file-information}

フォントの ID 名とそのタイプ情報を変更できます。 フォントファイルを編集することで、フォントを容易に検索および識別できるようになります。

参照パネルで、詳細ビューで編集するフォントファイルを選択し、「ファイル」 > 「情報を編集」を選択します。 情報を編集画面が開きます。次のオプションを選択してから、「**[!UICONTROL 送信]**」を選択してください。

* **[!UICONTROL フォント名]**：この名前は、公開時にフォントを識別します。

* **[!UICONTROL PostScript名]**：この名前は、フォントの完全なPostScript名です。 通常は、太さまたはスタイルを示します。

* **[!UICONTROL RTF 名]**：この名前は、テンプレートテキストレイヤーが作成される RTF エディターのポップアップメニューに表示されます。

* **[!UICONTROL フォントファミリー名]**：この名前には、スタイル、太さ、フォントタイプインジケーターのないフォント名が一覧表示されます。

* **[!UICONTROL フォントスタイル]**：オプションは、「プレーン」、「太字」、「斜体」、「太字斜体」です。

* **[!UICONTROL フォントタイプ]**：オプションは TrueType とAdobe Type 1 です。 これらのフォントを別の名前で呼び出す場合は、その名前を入力します。

* **[!UICONTROL フォントタイプの略語]**：次のオプションがあります。

   * **[!UICONTROL TTF]**:PDF/PostScriptのレンダリングおよび画像サービングに使用される TrueType フォントファイル。

   * **[!UICONTROL AFM]**:Adobe PostScript Font Metrics の情報を含み、画像サービングに使用されるAdobe フォントファイル。

   * **[!UICONTROL PFM]**：バイナリのフォント指標情報を含むAdobe PostScript フォントファイル。

   * **[!UICONTROL PFB]**：バイナリのフォントアウトライン情報を含み、PDF/PostScriptのレンダリングおよび画像サービングに使用されるAdobe PostScript フォントファイル。
