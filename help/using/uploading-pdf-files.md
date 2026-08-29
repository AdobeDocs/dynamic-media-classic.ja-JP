---
title: PDF ファイルのアップロード
description: Adobe Dynamic Media ClassicでeCatalogに関連付けられているPDF ファイルをアップロードする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T20:17:17.647Z'
TQID: 'https://experienceleague.adobe.com/SNoRYiCgjJK2TBx6X7HAzv3Xqet64-lm4oSOcat7DfM'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 4035cd307a13d1174f8b66fb1cd1ab39138d1310
workflow-type: tm+mt
source-wordcount: 838
ht-degree: 18%

---

# PDF ファイルのアップロード{#uploading-the-pdf-files}

Adobe PDF ファイルは、eCatalogのソースです。 これらのファイルには、すべての画像情報、フォント、ベクターグラフィックが含まれています。 画像付きの eCatalog を作成することもできます。 PDF ファイルのアップロードを準備したら、グローバルナビゲーションバーで「**[!UICONTROL アップロード]**」を選択して、PDFのアップロードを開始します。

ページ抽出用にPDFをアップロードする場合、Adobeでは次の制限が適用されます。

| PDF制限タイプ | 制限が適用されました | 2022年12月31日（PT）の上限への変更 |
| --- | --- | --- |
| 抽出に考慮するPDFの最大ページ数 | 5000 （新規アップロードの場合） | 100 （すべてのPDF） |

[Dynamic Mediaの制限](/help/using/limitations.md)も参照してください。

## PDF ファイルの準備

Adobe Dynamic Media Classicにアップロードする前に、PDF ファイルを準備します。

* ファイルのアップロードを簡単にするには、すべてのファイルをコンピューターまたはネットワーク上の同じフォルダーに配置します。
* ページの順番と同じになるように、英数字の順にファイルの名前を付けます。 ページを配置すると、ファイルをアップロードした後に適切な順序でページを配置しやすくなります。
* PDF ページにトンボ、レジストレーションターゲットまたはカラーバーが含まれているかどうかを確認するには、ページを調べます。 これらのマークは、文書を印刷する際の用紙の切り取り場所を決定します。eCatalogをオンラインで公開する前に、これらのマークを削除する必要があります。 Adobe Dynamic Media Classicには、PDF ファイルをアップロードするときにマークを切り抜くオプションが用意されています。
* ビューアがeCatalogをキーワードで検索する場合は、PDF ファイルが「統合」されているかどうかを確認します。 画像化された PDF ファイルでは、検索語を抽出できなくなります。 PDFが統合されているかどうかを判断するには、その中のテキストを選択してみてください。 テキストを選択できない場合、PDFは統合され、ビューアはeCatalog内のキーワードで検索できません。
* PDF ファイルは印刷用に作成されているため、通常はCMYK画像が含まれています。 デフォルトでは、Adobe Dynamic Media ClassicはこれらのCMYK画像を検出し、内部CMYK カラープロファイルを使用して変換します。 ただし、必要に応じて、カスタムカラープロファイルを使用して CMYK 画像を変換することもできます。

  [ICC （International Color Consortium） プロファイル &#x200B;](icc-profiles.md#icc_profiles)を参照してください。

## ベストプラクティスの PDF アップロードオプション {#best-practice-pdf-upload-options}

各アップロード方法について詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

アップロードするファイルを選択し、次の&#x200B;*ベストプラクティス* PDF オプションを選択します。

* **切り抜きオプション**: アップロードジョブオプションダイアログボックスで、**[!UICONTROL 切り抜きオプション]**&#x200B;を選択します。 PDF ページに切り抜きマーク、レジストレーションマーク、またはその他のマークが含まれている場合、**[!UICONTROL 切り抜き]** ドロップダウンリストで、**[!UICONTROL 手動]**&#x200B;を選択します。 ページの上、右、下、左から切り抜くピクセル数を入力します。 切り抜きマークは、多くの場合、0.5 インチの余白に設定されます。 ピクセル/インチの解像度として&#x200B;**[!UICONTROL 150]** （推奨）を選択したとします。 次に、「上」、「右」、「下」、「左」テキストボックスに「75」、「75」、「75」と入力します。 これにより、余白から0.5 インチが削除されます（150 ppiで、0.5 ピクセルは75 ピクセルに等しい）。

* **処理中**: アップロードジョブオプションダイアログボックスで、**[!UICONTROL PDF オプション]**&#x200B;を選択します。 「**[!UICONTROL 処理中]**」ドロップダウンリストで、「**[!UICONTROL ラスタライズ]**」を選択します。 すべてのページと画像を eCatalog で表示するためには、PDF ファイルをラスタライズする必要があります。

* **検索語を抽出（オプション）**: アップロードジョブオプションダイアログボックスで、**[!UICONTROL PDF オプション]**&#x200B;を選択します。 視聴者がeCatalogのキーワードで検索できるようにするには、**[!UICONTROL 抽出]** ドロップダウンリストで「**[!UICONTROL 単語を検索]**」を選択します。

* **複数ページのPDFからeCatalogを自動生成（オプション）**: アップロードジョブオプションダイアログボックスで、**[!UICONTROL PDF オプション]**&#x200B;を選択します。 「**[!UICONTROL 複数ページのPDF]**&#x200B;からeCatalogを自動生成」をクリックすると、アップロード時にeCatalogを自動作成できます。 eCatalog画面に直接移動し、eCatalogの作業を開始するには、最初にPDF ファイルを選択し、「ビルド」コマンドを選択する必要はありません。 eCatalog の名前は、PDF ファイルの名前をもとに付けられます。

* **解決策**: アップロードジョブオプションダイアログボックスで、**[!UICONTROL PDF オプション]**&#x200B;を選択します。 「**[!UICONTROL 解像度]**」テキストフィールドに値を入力します。 Adobe Dynamic Media Classicでは、1 インチあたり150 ピクセルを推奨しています。

* **Colorspace**: アップロードジョブオプションダイアログボックスで、**[!UICONTROL PDF オプション]**&#x200B;を選択します。 カラースペース ドロップダウンリストで、**[!UICONTROL 自動検出]**&#x200B;を選択します。 一般的に PDF のカラースペースは、印刷出力が目的の場合には CMYK、オンライン表示が目的の場合には RGB になります。 PDF に両方のカラースペースが含まれている場合は、「RGB としてレンダリング」または「CMYK としてレンダリング」のいずれかを選択して、一方のカラースペースを選択できます。 PDFは両方のカラースペースを使用します。例えば、ページグラフィックがCMYK カラースペースを使用し、画像がRGB カラースペースを使用する場合などです。 ICC プロファイルをアップロードしておくと、カラースペースメニューにその名前が表示され、選択して使用できます。

  [ICC （International Color Consortium） プロファイル &#x200B;](/help/using/icc-profiles.md)を参照してください。

* **カラープロファイルオプション**:「ジョブオプションをアップロード」ダイアログボックスで、「**[!UICONTROL カラープロファイルオプション]**」を選択し、次のカラープロファイルオプションを選択します。

  * **元のカラースペースを保持**：元のカラースペースを保持します。

  * **カスタム送信元/送信先**: サブメニューを開き、**[!UICONTROL 変換元]**&#x200B;および&#x200B;**[!UICONTROL 変換先]** カラースペースを選択できます。 標準のPhotoshop カラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

[ICC （International Color Consortium） プロファイル &#x200B;](icc-profiles.md#icc_profiles)を参照してください。

>[!NOTE]
>
>すべての PDF オプションについて詳しくは、[PDF アップロードオプション](pdfs.md#pdf_upload_options)を参照してください。
