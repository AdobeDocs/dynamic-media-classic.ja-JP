---
title: フォント
description: Dynamic Mediaクラシックのフォントの使い方を学びます。
uuid: bddec9c2-8530-4bbd-8db7-1562a347e482
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 97cecd6a-30aa-44fe-a611-fd71b02fd5ae
feature: Dynamic Mediaクラシック
role: Business Practitioner
exl-id: 186f4c7f-16f6-42f5-bc0e-55362c55e794
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 36%

---

# フォント{#fonts}

場合によっては、Dynamic Mediaクラシックでは、特定のフォントでテキストを入力したりレンダリングしたりするために、フォントファイルのアップロードが必要になることがあります。 例えば、テンプレートレイヤー上のテキストの特定のフォントを使用するには、フォントファイルをアップロードします。eCatalog ビューアページ番号を特定のフォントで表示するには、フォントファイルをアップロードします。

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

フォントのID名と種類の情報を変更できます。 フォントファイルを編集することで、フォントを容易に検索および識別できるようになります。

参照パネルで、詳細ビューで編集するフォントファイルを選択して、ファイル／情報を編集を選択します。情報を編集画面が開きます。次のオプションを選択して、「送信」ボタンを選択します。

* **フォント名**  — この名前は、公開時のフォントを識別します。

* **PostScript名**  — フォントの完全なPostScript名です。通常は、太さまたはスタイルを示します。

* **RTF名**  — この名前は、テンプレートテキストレイヤーを作成するRTFエディタのポップアップメニューに表示されます。

* **フォントファミリー名**  — この名前は、スタイル、重み付け、フォントタイプのインジケーターを除いたフォント名をリストします。

* **フォントスタイル**  — 標準、太字、斜体、太字斜体を選択できます。

* **フォントの種類** - TrueTypeとAdobe Type1を指定します。これらのフォントを別の名前で呼び出す場合は、その名前を入力します。

* **フォントタイプの省略形**  — オプションは次のとおりです。

   * **PDF/PostScriptのレンダリングと画像サービングに使用される** TTFTrueTypeフォントファイル。

   * **Adobeフォントメトリクス情報が含まれ、画像サービングに使用される** AFMAdobe PostScriptフォントファイル。

   * **バイナリフォントメトリック情報を含む** PFMAdobe PostScriptフォントファイル。

   * **バイナリフォントのアウトライン情報が含まれ、PDF/PostScriptのレンダリングと画像サービングに使用される** PFBAdobe PostScriptフォントファイル。
