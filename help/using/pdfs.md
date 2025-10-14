---
title: PDF の操作
description: Adobe Dynamic Media Classicで PDF を操作する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '726'
ht-degree: 26%

---

# PDF の操作{#working-with-pdfs}

PDF（Portable Document Format）ファイルは、eCatalog を作成するためにAdobe Dynamic Media Classicで最もよく使用されます。 PDF ファイル、Adobe Dynamic Media Classic ラスタライズ、リッピングをアップロードすると、デフォルトでは、ページを使用してリッチメディアを作成できるようにページが作成されます。

ページ抽出用にPDFをアップロードすると、Adobeでは次の制限を適用します。

| 制限タイプ | 適用される制限 | 2022 年 12 月 31 日の制限に変更 |
| --- | --- | --- |
| 抽出対象となるPDFの最大ページ数 | 5000 （新規アップロード用） | 100 （すべての PDF 用） |

[Dynamic Media の制限 &#x200B;](/help/using/limitations.md) も参照してください。

## PDF アップロードオプション {#pdf-upload-options}

PDF ファイルをアップロードする際には、ページの切り抜き、検索語の抽出、ppi 解像度の入力、およびカラースペースの選択など、様々な方法でファイルをフォーマットできます。PDF ファイルには、トリミング余白、トンボ、トンボ、その他のプリンターのマークなどが含まれる場合があります。 PDF ファイルのアップロード時には、ページの端をマークに沿って切り抜くことができます。

PDF ファイルのアップロードのオプションは、アップロード ページの「PDF オプション」にあります。

### 処理オプション

**[!UICONTROL ラスタライズ]**:（デフォルト）PDF ファイルのページをリッピングし、ベクターグラフィックをビットマップイメージに変換します。 eCatalog を作成するには、このオプションを選択します。

**[!UICONTROL 検索単語を抽出]**:PDF ファイルから単語を抽出し、eCatalog ビューア内でファイル内のキーワードを検索できるようにします。

**[!UICONTROL リンクを抽出]**:PDF ファイルからリンクを抽出し、eCatalog ビューアで使用できる画像マップに変換します。

**[!UICONTROL 複数ページのPDFを使用して eCatalog を自動生成]**:PDF ファイルから eCatalog を自動作成します。 eCatalog は、アップロードした PDF ファイルに従って名前が付けられます（このオプションは、アップロード時に PDF ファイルをラスタライズする場合のみ利用可能です）。

### 解像度

解像度設定を指定します。この設定には、PDF ファイルで表示する ppi を指定します。初期設定値は 150 です。

### カラースペースオプション

カラースペースメニューを選択し、PDF ファイルのカラースペースを選択します。ほとんどの PDF ファイルには、RGB カラー画像と CMYK カラー画像の両方が含まれています。RGB カラースペースは、オンライン表示に適しています。

* **[!UICONTROL 自動検出]**:PDF ファイルのカラースペースを保持します。

* **[!UICONTROL RGBとして強制]**:RGBのカラースペースに変換します。

* **[!UICONTROL CMYK として強制]**:CMYK カラースペースに変換します。

* **[!UICONTROL グレースケールとして強制]**：グレースケールカラースペースに変換します。

### カラープロファイルオプション

* **[!UICONTROL sRGB に変換]**:sRGB （標準の赤緑青）に変換します。 sRGB は、web ページに画像を表示するための推奨カラースペースです。

* **[!UICONTROL 元のカラースペースを保持]**：元のカラースペースを保持します。

* **[!UICONTROL カスタム開始]**/**[!UICONTROL 終了]**：メニューが開き、「変換元」および「変換先」カラースペースを選択できます。 標準のPhotoshop カラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。

詳しくは、[ICC プロファイル](/help/using/icc-profiles.md#icc_profiles)も参照してください。

## PDF ファイルからの空白の切り抜き {#cropping-white-space-from-a-pdf-file}

PDF ファイルをアップロードする際に、ファイルからホワイトスペースピクセルを自動的に切り抜くことができます。

1. 切り抜きメニューを選択し、「トリミング」を選択します。
1. 次のオプションを指定します。

   * **[!UICONTROL トリミング対象]**：カラーと透明度のどちらで切り抜くかを選択します。

      * **[!UICONTROL カラー]**:「カラー」オプションを選択します。 次に、**[!UICONTROL 隅]** メニューを選択し、切り抜きたいホワイトスペースの色を最も表現している色のPDFの隅を選択します。

      * **[!UICONTROL 透明度]**:「透明度」オプションを選択します。

   * **[!UICONTROL 公差]**: スライダーをドラッグして、0 ～ 1 の公差を指定します。

   * **[!UICONTROL カラーに基づくトリミング]**:0 を指定すると、PDFの隅で選択した色と完全に一致するピクセルのみが切り抜かれます。 設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。

   * **[!UICONTROL 透明度に基づくトリミング]**：切り抜くピクセルが透明な場合のみ、0 を指定します。1 に近い数値を指定すると、透明度が高くなります。

## PDFページの端から切り抜く {#cropping-from-the-sides-of-pdf-pages}

PDF ファイルをアップロードする際に、ページの端から手動でトンボを取り除くことができます。

1. 切り抜きメニューで、「**[!UICONTROL 手動]**」を選択します。
1. 「上」、「右」、「下」、「左」の各テキストボックスに、ページの上下左右の端からそれぞれ切り抜くピクセル数を入力します。

ページから切り抜かれる長さは、PDF ファイルの ppi（ピクセル/インチ）設定によって異なります。例えば、「解像度ピクセル/インチ」の設定に 150 （デフォルト）と入力したとします。 次に、ページの端から 75 ピクセルを切り抜きます。 この場合、0.5 インチになります。 は切り抜かれます。 1 インチあたり 150 ピクセルの場合、75 ピクセルは半インチに相当します。
