---
title: PDFの操作
description: Adobe Dynamic Media ClassicでPDFを操作する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:53:07.417Z'
TQID: 'https://experienceleague.adobe.com/yM24UnCiU64kLvHXjhX6S8ZJpWgoyAzQKuDHN02yUXs'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: a6f31cfc417aa908738642a9543ada88b4620c02
workflow-type: tm+mt
source-wordcount: 734
ht-degree: 21%

---

# PDFの操作{#working-with-pdfs}

PDF（Portable Document Format）ファイルは、eCatalogsの作成にAdobe Dynamic Media Classicで最もよく使用されます。 PDF ファイルをアップロードすると、Adobe Dynamic Media Classicはデフォルトでページをラスタライズして、ページをリッチメディアの作成に使用できるようにします。

ページ抽出用にPDFをアップロードする場合、Adobeでは次の制限が適用されます。

| 制限タイプ | 制限が適用されました | 2022年12月31日（PT）の上限への変更 |
| --- | --- | --- |
| 抽出に考慮するPDFの最大ページ数 | 5000 （新規アップロードの場合） | 100 （すべてのPDF） |

[Dynamic Mediaの制限](/help/using/limitations.md)も参照してください。

## PDF アップロードオプション {#pdf-upload-options}

PDF ファイルをアップロードする際には、 ページの切り抜き、検索語の抽出、インチ単位のピクセル単位の解像度の入力、カラースペースの選択を行うことができます。 PDF ファイルには、多くの場合、トリムマージン、トンボ、レジストレーションマーク、その他のプリントマークが含まれています。 PDF ファイルのアップロード時には、ページの端をマークに沿って切り抜くことができます。

PDF ファイルをアップロードするためのオプションは、PDF オプションの下のアップロードページにあります。

### 処理オプション

**[!UICONTROL ラスタライズ]**: （デフォルト） PDF ファイル内のページをラスタライズし、ベクターグラフィックをビットマップ画像に変換するには、このオプションを使用します。 eCatalogを作成するには、このオプションを選択します。

**[!UICONTROL 検索語を抽出]**: PDF ファイルから単語を抽出して、ファイル内のキーワードをeCatalog ビューアで検索できるようにします。

**[!UICONTROL リンクを抽出]**: PDF ファイルからリンクを抽出し、eCatalog Viewerで使用される画像マップに変換します。

**[!UICONTROL 複数ページのPDFを使用してeCatalogを自動生成]**: PDF ファイルからeCatalogを自動生成します。 eCatalog は、アップロードした PDF ファイルに従って名前が付けられます （このオプションは、アップロード時に PDF ファイルをラスタライズする場合のみ利用可能です）。

### 解像度

解像度設定を指定します。 この設定には、PDF ファイルで表示する ppi を指定します。 初期設定値は 150 です。

### カラースペースのオプション

カラースペースメニューを選択し、PDF ファイルのカラースペースを選択します。 ほとんどの PDF ファイルには、RGB カラー画像と CMYK カラー画像の両方が含まれています。 RGB カラースペースは、オンライン表示に適しています。

* **[!UICONTROL 自動検出]**: PDF ファイルのカラースペースを保持します。

* **[!UICONTROL RGBとして強制]**: RGBのカラースペースに変換します。

* **[!UICONTROL CMYKとして強制]**: CMYK カラースペースに変換します。

* **[!UICONTROL グレースケールとして強制]**: グレースケールのカラースペースに変換します。

### カラープロファイルオプション

* **[!UICONTROL sRGBに変換]**: sRGBに変換（標準の赤緑色の青）。 sRGBは、Web ページに画像を表示する際に推奨されるカラースペースです。

* **[!UICONTROL 元のカラースペースを保持]**：元のカラースペースを保持します。

* **[!UICONTROL カスタム開始]** > **[!UICONTROL から]**: メニューを開いて、`Convert From`と`Convert To`のカラースペースを選択できます。 標準のAdobe Photoshop カラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。

詳しくは、[ICC プロファイル](/help/using/icc-profiles.md#icc_profiles)も参照してください。

## PDF ファイルから空白を切り抜く {#cropping-white-space-from-a-pdf-file}

PDF ファイルをアップロードすると、空白のピクセルを自動的に切り抜くことができます。

1. 切り抜きメニューを選択し、「トリミング」を選択します。
1. 次のオプションを指定します。

   * **[!UICONTROL トリミングの基準]**：色または透明度に基づいてトリミングするかどうかを選択します。

     * **[!UICONTROL カラー]**:「カラー」オプションを選択します。 次に、**[!UICONTROL 角]** メニューを選択し、切り抜くホワイトスペースの色を最も表す色のPDFの角を選択します。

     * **[!UICONTROL 透明度]**: 「透明度」オプションを選択します。

   * **[!UICONTROL 許容値]**:0 ～ 1の許容値を指定するには、スライダーをドラッグします。

   * **[!UICONTROL カラーに基づくトリミング]**:PDFの隅で選択したカラーと完全に一致する場合にのみ、ピクセルを切り抜くには0を指定します。 設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。

   * **[!UICONTROL 透明度に基づくトリミング]**：透明なピクセルの場合のみ切り抜きピクセルに0を指定します。1に近い数値を指定すると、透明度が高くなります。

## PDF ページの側面から切り抜く {#cropping-from-the-sides-of-pdf-pages}

PDF ファイルのページの側面から印刷用マークを手動で削除してアップロードできます。

1. 切り抜きメニューから、**[!UICONTROL 手動]**&#x200B;を選択します。
1. 「上」、「右」、「下」、「左」の各テキストボックスに、ページの上下左右の端からそれぞれ切り抜くピクセル数を入力します。

切り抜かれるページの量は、PDF ファイルに入力する解像度PX/インチ設定によって異なります。 例えば、「解像度PX/インチ」設定に「150」（デフォルト）と入力するとします。 次に、ページの側面から75 ピクセルを切り抜きます。 この場合は0.5 インチです。 はトリミングされます。 150 ピクセル/インチでは、75 ピクセルは半インチに相当します。
