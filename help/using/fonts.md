---
title: フォント
description: Adobe Dynamic Media Classicでのフォントの使用方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:50:28.929Z'
TQID: 'https://experienceleague.adobe.com/g-A6M8KM6VT4m-JVyDp6KMMN82CtGTXcoUFVvQsoLps'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 430
ht-degree: 23%

---

# フォント{#fonts}

Adobe Dynamic Media Classicでは、特定のフォントでテキストを入力またはレンダリングするために、フォントファイルをアップロードする必要がある場合があります。 例えば、テンプレートレイヤー上のテキストの特定のフォントを使用するには、フォントファイルをアップロードします。 eCatalog ビューアページ番号を特定のフォントで表示するには、フォントファイルをアップロードします。

Adobe Dynamic Media Classicでは、次のフォントタイプをサポートしています。

* すべての TrueType フォント
* PostScript® fonts
* OpenType/TrueType フォント
* OpenType/PostScript フォント
* PhotoFont

フォントファイルをアップロードした後、フォントファイルのAdobe Dynamic Media Classic ID、フォント名、およびフォントファイルの入力情報を「情報を編集」画面で変更できます。

>[!NOTE]
>
>Adobe Dynamic Media Classicでは、テンプレートレイヤーでフォントを使用する場合は、すべてのフォントスタイル（太字、斜体、太字/斜体、標準）をアップロードすることをお勧めします。 Adobe Dynamic Media Classicでは、リクエストを処理するためにこれらのフォントスタイルが必要です。 フォントに関連付けられたすべての`PostScript/Adobe Type1` ファイルをアップロードすることも推奨されます。これらのフォントには、カーニング情報の詳細が含まれているものもあります。

## フォントファイルをアップロード {#uploading-font-files}

フォントファイルのアップロードは、その他のファイルをアップロードするのと同じ方法で行います。 フォントファイルは、任意のAdobe Dynamic Media Classic フォルダーに保存できます。 詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## フォントファイル情報の編集 {#editing-font-file-information}

フォントのID名とそのタイプ情報を変更できます。 フォントファイルを編集することで、フォントを容易に検索および識別できるようになります。

参照パネルで、編集するフォントファイルを詳細表示で選択し、ファイル/情報を編集を選択します。 情報を編集画面が開きます。 次のオプションを選択し、**[!UICONTROL 送信]**&#x200B;を選択します。

* **[!UICONTROL フォント名]**：この名前は、公開時にフォントを識別します。

* **[!UICONTROL PostScript名]**：この名前は、フォントの完全なPostScript名です。 通常は、太さまたはスタイルを示します。

* **[!UICONTROL RTF名]**：この名前は、テンプレート テキスト レイヤーが作成されるRTF エディターのポップアップメニューに表示されます。

* **[!UICONTROL フォントファミリー名]**：この名前には、スタイル、重み、またはフォントタイプインジケーターが表示されません。

* **[!UICONTROL フォントスタイル]**：オプションは、プレーン、太字、斜体、太字 – 斜体です。

* **[!UICONTROL Font Type]**: オプションはTrueTypeとAdobe Type 1です。 これらのフォントを別の名前で呼び出す場合は、その名前を入力します。

* **[!UICONTROL フォントタイプの省略形]**：オプションは次のとおりです。

   * **[!UICONTROL TTF]**: PDF/PostScriptのレンダリングと画像の配信に使用されるTrueType フォントファイル。

   * **[!UICONTROL AFM]**: Adobe Font Metrics情報を含み、画像の配信に使用されるAdobe PostScript フォントファイル。

   * **[!UICONTROL PFM]**: バイナリ フォント メトリック情報を含むAdobe PostScript フォント ファイル。

   * **[!UICONTROL PFB]**: バイナリ フォントのアウトライン情報を含み、PDF/PostScriptのレンダリングと画像の処理に使用されるAdobe PostScript フォント ファイル。
