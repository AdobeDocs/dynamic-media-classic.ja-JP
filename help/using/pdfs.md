---
title: PDFの操作
description: Adobe Dynamic Media ClassicでPDFを使用する方法を説明します。
uuid: 26d70d28-9393-49b1-9051-d70456deca67
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 5a073de3-6b1d-4c3e-8c03-9182f9f3874a
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 02892514-61fe-48ba-a2e3-eeb30580a1e4
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 36%

---

# PDFの操作{#working-with-pdfs}

PDF(Portable Document Format) ファイルは、eCatalog を作成する際にAdobe Dynamic Media Classicで最もよく使用されます。 PDFファイル、Adobe Dynamic Media Classicラスタライズまたはリップをアップロードすると、デフォルトでは、ページを使用してリッチメディアを作成できるように、ページがラスタライズまたはリップされます。

ページ抽出用のPDFをアップロードする際、Adobeでは次の制限が適用されます。

| 制限タイプ | 制限が適用されました | 2022 年 12 月 31 日の制限に変更 |
| --- | --- | --- |
| 抽出対象となるPDFの最大ページ数 | 5000（新しいアップロード用） | 100( すべてのPDF) |

関連トピック [Dynamic Mediaの制限](/help/using/limitations.md).

## PDF アップロードオプション {#pdf-upload-options}

PDF ファイルをアップロードする際には、ページの切り抜き、検索語の抽出、ppi 解像度の入力、およびカラースペースの選択など、様々な方法でファイルをフォーマットできます。PDF ファイルには、通常、トリミングマージン、切り抜きマーク、登録マーク、および他の印刷記号が印字されます。PDF ファイルのアップロード時には、ページの端をマークに沿って切り抜くことができます。

PDFファイルをアップロードするためのオプションは、アップロードページの「PDFオプション」の下に表示されます。

### 処理オプション

**[!UICONTROL ラスタライズ]** - （デフォルト）PDFファイル内のページをリップし、ベクトルグラフィックをビットマップ画像に変換します。 eCatalog を作成するには、このオプションを選択します。

**[!UICONTROL 検索語を抽出]** - eCatalog ビューアでPDFで検索できるように、キーワードファイルから単語を抽出します。

**[!UICONTROL リンクを抽出]** -PDFファイルからリンクを抽出し、eCatalog ビューアで使用される画像マップに変換します。

**[!UICONTROL 複数ページPDFで eCatalog を自動生成]** - eCatalog をPDF・ファイルから自動的に作成 eCatalog は、アップロードした PDF ファイルに従って名前が付けられます（このオプションは、アップロード時に PDF ファイルをラスタライズする場合のみ利用可能です）。

### 解像度

解像度設定を指定します。この設定には、PDF ファイルで表示する ppi を指定します。初期設定値は 150 です。

### カラースペースオプション

カラースペースメニューを選択し、PDF ファイルのカラースペースを選択します。ほとんどの PDF ファイルには、RGB カラー画像と CMYK カラー画像の両方が含まれています。RGB カラースペースは、オンライン表示に適しています。

* **[!UICONTROL 自動検出]** -PDF・ファイルのカラー・スペースを保持します。

* **[!UICONTROL 強制RGB]**  — をRGBのカラースペースに変換します。

* **[!UICONTROL CMYK としてレンダリング]** - CMYK カラースペースに変換します。

* **[!UICONTROL グレースケールとして強制]**  — グレースケールカラースペースに変換します。

### カラープロファイルオプション

* **[!UICONTROL sRGB に変換]** - sRGB（標準赤緑青）に変換します。 Web ページに画像を表示する場合のカラースペースには sRGB が推奨されます。

* **[!UICONTROL 元のカラースペースを保持]**  — 元のカラースペースを保持します。

* **[!UICONTROL カスタム送信元]** > **[!UICONTROL 宛先]** - 「変換元」と「変換先」のカラースペースを選択できるメニューを開きます。 Photoshopの標準的なカラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。

詳しくは、[ICC プロファイル](/help/using/icc-profiles.md#icc_profiles)も参照してください。

## PDFファイルから空白を切り抜く {#cropping-white-space-from-a-pdf-file}

1. アップロード時に PDF ファイルの余白ピクセルを自動的に切り抜くには、切り抜きメニューを選択し、「トリミング」を選択します。
1. 次のオプションを指定します。

   * **[!UICONTROL トリミングする対象]**  — 色または透明度に基づいて切り抜くかどうかを選択します。

      * **[!UICONTROL カラー]** - 「カラー」オプションを選択します。 次に、 **[!UICONTROL 角]** メニューを開き、切り抜くPDFの隅に、切り抜く空白の色を最もよく表す色を選択します。

      * **[!UICONTROL 透明]** - 「透明度」オプションを選択します。
   * **[!UICONTROL 許容値]**  — スライダをドラッグして、0 ～ 1 の公差を指定します。

   * **[!UICONTROL 色に基づくトリミング]**  — ピクセルがPDFの隅で選択した色と完全に一致する場合にのみピクセルを切り抜く場合は、0 を指定します。 設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。

   * **[!UICONTROL 透明度に基づくトリミング]**  — ピクセルが透明の場合にのみ切り抜くには 0 を指定します。1 に近い値を指定すると、透明度が高くなります。


## PDFページの端からの切り抜き {#cropping-from-the-sides-of-pdf-pages}

アップロード時に、PDF ファイルのページの端から印刷マークまでを手動で削除できます。

1. 切り抜きメニューで、「 」を選択します。 **[!UICONTROL 手動]**.
1. 「上」、「右」、「下」、「左」の各テキストボックスに、ページの上下左右の端からそれぞれ切り抜くピクセル数を入力します。

ページから切り抜かれる長さは、PDF ファイルの ppi（ピクセル/インチ）設定によって異なります。例えば、「解像度 (PX/Inch) 」設定に 150（デフォルト）と入力したとします。 次に、ページの端から 75 ピクセル切り抜きます。 この場合、0.5 インチ が切り抜かれます。 150 ピクセル/インチでは、75 ピクセルは 1/2 インチに等しくなります。
