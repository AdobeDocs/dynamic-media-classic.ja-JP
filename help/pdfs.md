---
title: PDFの操作
description: Dynamic Media ClassicでのPDFの操作方法について説明します。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 3185824deca4d4b3c5549bda2e47f179094110e7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# PDFの操作{#working-with-pdfs}

PDF(Portable Document Format)ファイルは、eCatalogの作成にDynamic Media ClassicAdobeで最もよく使用されます。 PDFファイルをアップロードすると、AdobeDynamic Media Classicは、デフォルトでページをラスタライズまたはリップし、リッチメディアの作成にページを使用できるようにします。

## PDF アップロードオプション {#pdf-upload-options}

PDF ファイルをアップロードする際には、ページの切り抜き、検索語の抽出、ppi 解像度の入力、およびカラースペースの選択など、様々な方法でファイルをフォーマットできます。PDF ファイルには、通常、トリミングマージン、切り抜きマーク、登録マーク、および他の印刷記号が印字されます。PDF ファイルのアップロード時には、ページの端をマークに沿って切り抜くことができます。

PDFファイルをアップロードするためのオプションは、アップロードページの「PDFオプション」の下に表示されます。

### 処理オプション

**[!UICONTROL ラスタライズ]**  - （デフォルト）PDFファイルのページをリップし、ベクトルグラフィックをビットマップ画像に変換します。eCatalogを作成するには、このオプションを選択します。

**[!UICONTROL 検索語を抽出]**  - PDFファイルから単語を抽出し、eCatalogビューアでキーワードを使用してファイルを検索できるようにします。

**[!UICONTROL リンクを抽出]**  - PDFファイルからリンクを抽出し、eCatalogビューアで使用される画像マップに変換します。

**[!UICONTROL 複数ページのPDFを使用してeCatalogを自動生成]**  - PDFファイルからeCatalogを自動的に作成します。eCatalog は、アップロードした PDF ファイルに従って名前が付けられます（このオプションは、アップロード時に PDF ファイルをラスタライズする場合のみ利用可能です）。

### 解像度

解像度設定を指定します。この設定には、PDF ファイルで表示する ppi を指定します。初期設定値は 150 です。

### カラースペースオプション

カラースペースメニューを選択し、PDF ファイルのカラースペースを選択します。ほとんどの PDF ファイルには、RGB カラー画像と CMYK カラー画像の両方が含まれています。RGB カラースペースは、オンライン表示に適しています。

* **[!UICONTROL 自動検出]**  - PDFファイルのカラースペースを保持します。

* **[!UICONTROL RGBとしてレンダリング]**  - RGBカラースペースに変換します。

* **[!UICONTROL CMYKとして強制]**  - CMYKカラースペースに変換します。

* **[!UICONTROL グレースケールとしてレンダリング]**  — グレースケールカラースペースに変換します。

### カラープロファイルオプション

* **[!UICONTROL sRGBに変換]**  - sRGB（標準の赤緑青）に変換します。Web ページに画像を表示する場合のカラースペースには sRGB が推奨されます。

* **[!UICONTROL 元のカラースペースを保持]**  — 元のカラースペースを保持します。

* **[!UICONTROL カスタムの変換元]** / **[!UICONTROL 変換先]**  - 「変換元」と「変換先」のカラースペースを選択できるメニューを開きます。標準のPhotoshopカラースペースまたはDynamic Media ClassicにアップロードしたAdobeのカラースペースを選択できます。

詳しくは、[ICC プロファイル](/help/icc-profiles.md#icc_profiles)も参照してください。

## PDFファイルからの空白の切り抜き {#cropping-white-space-from-a-pdf-file}

1. アップロード時に PDF ファイルの余白ピクセルを自動的に切り抜くには、切り抜きメニューを選択し、「トリミング」を選択します。
1. 次のオプションを指定します。

   * **[!UICONTROL トリミングする部分を基準]**  — 色と透明度のどちらで切り抜くかを選択します。

      * **[!UICONTROL カラー]**  - 「カラー」オプションを選択します。次に、**[!UICONTROL 角]**&#x200B;メニューを選択し、切り抜く白のスペースの色を最も表す色のPDFの角を選択します。

      * **[!UICONTROL 透明度]**  - 「透明度」オプションを選択します。
   * **[!UICONTROL 許容値]**  — スライダをドラッグして、許容値を0 ～ 1の範囲で指定します。

   * **[!UICONTROL 色に基づくトリミング]**  - PDFの隅で選択した色と完全に一致するピクセルのみを切り抜く場合は、0を指定します。設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。

   * **[!UICONTROL 透明度に基づくトリミング]**  — 透明なピクセルのみを切り抜く場合は0を指定します。1に近い値を指定すると、透明度が高くなります。


## PDFページの端からの切り抜き {#cropping-from-the-sides-of-pdf-pages}

アップロード時に、PDF ファイルのページの端から印刷マークまでを手動で削除できます。

1. 切り抜きメニューから、**[!UICONTROL 手動]**&#x200B;を選択します。
1. 「上」、「右」、「下」、「左」の各テキストボックスに、ページの上下左右の端からそれぞれ切り抜くピクセル数を入力します。

ページから切り抜かれる長さは、PDF ファイルの ppi（ピクセル/インチ）設定によって異なります。例えば、「解像度（PX/インチ） 」設定に150（デフォルト）と入力し、ページの端から75ピクセルの切り抜きを行うと、半分のインチが切り抜かれます。150ピクセル/インチの場合、75ピクセルは1/2インチに等しくなります。
