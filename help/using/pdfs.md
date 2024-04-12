---
title: PDFの操作
description: Adobe Dynamic Media ClassicでPDFを使用する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 29%

---

# PDFの操作{#working-with-pdfs}

PDF（Portable Document Format）ファイルは、eCatalog を作成するためにAdobe Dynamic Media Classicで最もよく使用されます。 PDFファイル、Adobe Dynamic Media Classicのラスタライズまたはリッピングをアップロードすると、デフォルトで、ページを使用してリッチメディアを作成できるようにページが作成されます。

ページ抽出用のPDFをアップロードする場合、Adobeでは次の制限を適用します。

| 制限タイプ | 適用される制限 | 2022 年 12 月 31 日の制限に変更 |
| --- | --- | --- |
| PDFの抽出対象となる最大ページ数 | 5000 （新規アップロード用） | 100 （すべてのPDF用） |

関連トピック [Dynamic Mediaの制限](/help/using/limitations.md).

## PDF アップロードオプション {#pdf-upload-options}

PDF ファイルをアップロードする際には、ページの切り抜き、検索語の抽出、ppi 解像度の入力、およびカラースペースの選択など、様々な方法でファイルをフォーマットできます。PDFファイルには、トリミング余白、トリミング マーク、登録マーク、その他のプリンタ マークなどが含まれる場合があります。 PDF ファイルのアップロード時には、ページの端をマークに沿って切り抜くことができます。

PDFファイルのアップロードのオプションは、「アップロード」ページの「PDFオプション」の下にあります。

### 処理オプション

**[!UICONTROL ラスタライズ]** - （デフォルト）PDFファイルのページをリッピングし、ベクターグラフィックをビットマップイメージに変換します。 eCatalog を作成するには、このオプションを選択します。

**[!UICONTROL 検索語を抽出]** - PDFファイルから単語を抽出し、eCatalog ビューア内でこのファイルをキーワード検索できるようにします。

**[!UICONTROL リンクを抽出]** -PDFファイルからリンクを抽出し、eCatalog ビューアで使用できる画像マップに変換します。

**[!UICONTROL 複数ページのPDFによる eCatalog の自動生成]** -PDFファイルから eCatalog を自動作成します。 eCatalog は、アップロードした PDF ファイルに従って名前が付けられます（このオプションは、アップロード時に PDF ファイルをラスタライズする場合のみ利用可能です）。

### 解像度

解像度設定を指定します。この設定には、PDF ファイルで表示する ppi を指定します。初期設定値は 150 です。

### カラースペースオプション

カラースペースメニューを選択し、PDF ファイルのカラースペースを選択します。ほとんどの PDF ファイルには、RGB カラー画像と CMYK カラー画像の両方が含まれています。RGB カラースペースは、オンライン表示に適しています。

* **[!UICONTROL 自動検出]** -PDFファイルのカラースペースを保持します。

* **[!UICONTROL RGBとして強制]** -RGBのカラースペースに変換します。

* **[!UICONTROL CMYK としてレンダリング]** - CMYK カラースペースに変換します。

* **[!UICONTROL グレースケールとして強制]** - グレースケールカラースペースに変換します。

### カラープロファイルオプション

* **[!UICONTROL sRGB に変換]** - sRGB （標準赤緑青）に変換します。 sRGB は、web ページに画像を表示するための推奨カラースペースです。

* **[!UICONTROL 元のカラースペースを維持]**  – 元のカラースペースを保持します。

* **[!UICONTROL カスタムの送信元]** > **[!UICONTROL 終了]** - メニューが開き、「変換元」と「変換先」のカラースペースを選択できます。 標準のPhotoshop カラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。

詳しくは、[ICC プロファイル](/help/using/icc-profiles.md#icc_profiles)も参照してください。

## PDFファイルから空白を切り抜く {#cropping-white-space-from-a-pdf-file}

1. アップロード時に PDF ファイルの余白ピクセルを自動的に切り抜くには、切り抜きメニューを選択し、「トリミング」を選択します。
1. 次のオプションを指定します。

   * **[!UICONTROL トリミング対象カラー]**  – 色または透明度に基づいて切り抜くかどうかを選択します。

      * **[!UICONTROL カラー]** - 「カラー」オプションを選択します。 次に、 **[!UICONTROL Corner]** をクリックし、切り抜きたいホワイトスペースの色を最も表現している色のPDFの角を選びます。

      * **[!UICONTROL 透明度]** - 「透明度」オプションを選択します。

   * **[!UICONTROL 許容値]** - スライダーをドラッグして、0 ～ 1 の公差を指定します。

   * **[!UICONTROL カラーに基づくトリミング]** - 0 を指定すると、PDFの隅で選択した色と完全に一致するピクセルのみが切り抜かれます。 設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。

   * **[!UICONTROL 透明度に基づくトリミング]** - 0 を指定すると、ピクセルが透明な場合にのみ切り抜かれます。1 に近い数値を指定すると、透明度が高くなります。

## PDFページの端から切り抜く {#cropping-from-the-sides-of-pdf-pages}

PDFファイルをアップロードするときに、ページの端から手動でトンボを取り除くことができます。

1. 切り抜きメニューで、を選択します。 **[!UICONTROL 手動]**.
1. 「上」、「右」、「下」、「左」の各テキストボックスに、ページの上下左右の端からそれぞれ切り抜くピクセル数を入力します。

ページから切り抜かれる長さは、PDF ファイルの ppi（ピクセル/インチ）設定によって異なります。例えば、「解像度ピクセル/インチ」の設定に 150 （デフォルト）と入力したとします。 次に、ページの端から 75 ピクセルを切り抜きます。 この場合、0.5 インチになります。 は切り抜かれます。 1 インチあたり 150 ピクセルの場合、75 ピクセルは半インチに相当します。
