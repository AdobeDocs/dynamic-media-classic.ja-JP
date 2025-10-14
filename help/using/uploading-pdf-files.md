---
title: PDF ファイルのアップロード
description: eCatalog に関連付けられたPDF ファイルをAdobe Dynamic Media Classicにアップロードする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
topic: Integrations, Development
level: Experienced
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 30%

---

# PDF ファイルのアップロード{#uploading-the-pdf-files}

通常、Adobe PDF ファイルは eCatalog のソースです。 これらのファイルには、すべての画像情報、フォント、ベクターグラフィックが含まれています。 画像付きの eCatalog を作成することもできます。アップロード用のPDF ファイルの準備が整ったら、グローバルナビゲーションバーの「**[!UICONTROL アップロード]**」を選択して、PDF のアップロードを開始します。

ページ抽出用にPDFをアップロードすると、Adobeでは次の制限を適用します。

| PDFの制限タイプ | 適用される制限 | 2022 年 12 月 31 日の制限に変更 |
| --- | --- | --- |
| 抽出対象となるPDFの最大ページ数 | 5000 （新規アップロード用） | 100 （すべての PDF 用） |

[Dynamic Media の制限 &#x200B;](/help/using/limitations.md) も参照してください。

## PDF ファイルの準備

Adobe Dynamic Media Classicにアップロードする前にPDF ファイルを準備します。

* ファイルのアップロードを簡単にするには、すべてのファイルをコンピューターまたはネットワーク上の同じフォルダーに配置します。
* ページの順番と同じになるように、英数字の順にファイルの名前を付けます。ページの順番に合わせておけば、ファイルをアップロードした後に正しい順番でページを並べやすくなります。
* PDFのページに、クロップマーク、目標、カラーバーが含まれているかどうかを確認するには、ページを調べます。 このようなマークが入っていると、文書を印刷するときにこのマークに沿ってページが切り抜かれるため、Web に eCatalog を掲載する前に削除しておく必要があります。Adobe Dynamic Media Classicでは、PDF ファイルのアップロード時にマークを切り抜くためのオプションが用意されています。
* 閲覧者がキーワードで eCatalog を検索できるようにする場合は、PDF ファイルが「統合」されているかどうかを調べます。 画像化された PDF ファイルでは、検索語を抽出できなくなります。PDFが統合されているかどうかを確認するには、その中のテキストを選択してみてください。 テキストを選択できない場合、PDFは統合され、ビューアは eCatalog 内をキーワードで検索できなくなります。
* PDF ファイルは印刷を目的としたファイルなので、通常、CMYK 画像が含まれています。デフォルトでは、Adobe Dynamic Media Classicは、これらの CMYK 画像をインテリジェントに検出し、内部の CMYK カラープロファイルを使用して変換できます。 ただし、必要に応じて、カスタムカラープロファイルを使用して CMYK 画像を変換することもできます。

  [ICC （International Color Consortium）のプロファイル &#x200B;](icc-profiles.md#icc_profiles) を参照してください。

## ベストプラクティスの PDF アップロードオプション {#best-practice-pdf-upload-options}

各アップロード方法について詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

アップロードするファイルを選択し、次の *ベストプラクティス* PDF オプションを選択します。

* **切り抜きオプション**: アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL 切り抜きオプション]**」を選択します。 PDFページにトンボ、トンボなどのマークが含まれる場合は、「**[!UICONTROL 切り抜き]**」ドロップダウンリストで「**[!UICONTROL 手動]**」を選択します。 ページの上、右、下、左から切り抜くピクセル数を入力します。 トリミング マークは、多くの場合、5 インチの余白に設定されます。 インチあたりのピクセル数の解像度として **[!UICONTROL 150]** （推奨）を選択するとします。 次に、[ 上 ]、[ 右 ]、[ 下 ]、[ 左 ] の各テキスト ボックスに 75、75、75、75 と入力します。 このような場合、余白から半インチをトリミングします（150 ppi で、1 の半分は 75 ピクセルになります）。

* **処理中**: アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL PDFオプション]**」を選択します。 **[!UICONTROL 処理中]** ドロップダウンリストから「**[!UICONTROL ラスタライズ]**」を選択します。 すべてのページと画像を eCatalog で表示するためには、PDF ファイルをラスタライズする必要があります。

* **検索語を抽出（オプション）**: アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL PDFオプション]**」を選択します。 ビューアで eCatalog 内のキーワードで検索できるようにする場合は、抽出ドロップダウンリストで **[!UICONTROL 単語を検索]** を選択します。

* **複数ページのPDFから eCatalog を自動生成（オプション）**: アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL PDF オプション]**」を選択します。 **[!UICONTROL 複数ページのPDFから eCatalog を自動生成]** をクリックすると、アップロード時に eCatalog を自動生成できます。 PDF ファイルを選択してから「ビルド」コマンドを選択しなくても、eCatalog 画面が開き、eCatalog で作業できるようになります。eCatalog の名前は、PDF ファイルの名前をもとに付けられます。

* **解決策**: アップロードジョブオプション ダイアログボックスで、**[!UICONTROL PDF Options]** を選択します。 **[!UICONTROL 解像度]** テキストフィールドに値を入力します。 Adobe Dynamic Media Classicでは、1 インチあたり 150 ピクセルを推奨しています。

* **カラースペース**: アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL PDFオプション]**」を選択します。 「カラースペース」ドロップダウンリストで、「**[!UICONTROL 自動検出]**」を選択します。 一般的に PDF のカラースペースは、印刷出力が目的の場合には CMYK、オンライン表示が目的の場合には RGB になります。PDF に両方のカラースペースが含まれている場合は、「RGB としてレンダリング」または「CMYK としてレンダリング」のいずれかを選択して、一方のカラースペースを選択できます。例えば、ページのグラフィックに CMYK カラースペースが使用され、ピクチャに RGB カラースペースが使用されている場合には、両方のカラースペースが PDF に含まれます。ICC プロファイルをアップロードしておくと、カラースペースメニューにその名前が表示され、選択して使用できます。

  [ICC （International Color Consortium）のプロファイル &#x200B;](/help/using/icc-profiles.md) を参照してください。

* **カラープロファイルオプション**: アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL カラープロファイルオプション]**」を選択したあと、カラープロファイルオプションを選択します。

   * **元のカラースペースを保持**：元のカラースペースを保持します。

   * **カスタム開始/終了**：サブメニューが開き、「**[!UICONTROL 変換：開始]**」および「**[!UICONTROL 変換：終了]** カラースペースを選択できます。 標準のPhotoshop カラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。

<!-- * **Convert To SRGB**: Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on Web pages. -->

[ICC （International Color Consortium）のプロファイル &#x200B;](icc-profiles.md#icc_profiles) を参照してください。

>[!NOTE]
>
>すべての PDF オプションについて詳しくは、[PDF アップロードオプション](pdfs.md#pdf_upload_options)を参照してください。
