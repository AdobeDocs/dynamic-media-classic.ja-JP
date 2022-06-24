---
title: PDFファイルのアップロード
description: Adobe Dynamic Media Classicで eCatalog に関連付けられたPDFファイルをアップロードする方法を説明します。
uuid: 9e178bb2-ac09-427a-b61a-aad4e87a5837
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 0097cba5-c886-4115-bc35-7ae7a500202f
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: a787d6b5-48c8-4cf7-b136-60ba3d3eb2f2
source-git-commit: 7c1dfa7382b6eaf746fe7f0ac426472180c0c70c
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 38%

---

# PDFファイルのアップロード{#uploading-the-pdf-files}

通常、Adobe PDFファイルは eCatalog のソースです。 これらのファイルには、すべての画像情報、フォント、およびベクトルグラフィックが含まれます。 画像付きの eCatalog を作成することもできます。アップロード用のPDFファイルを準備したら、グローバルナビゲーションバーで、 **[!UICONTROL アップロード]** をクリックして、PDFのアップロードを開始します。

ページ抽出用のPDFをアップロードする際、Adobeでは次の制限が適用されます。

| PDF制限タイプ | 制限が適用されました | 2022 年 12 月 31 日の制限に変更 |
| --- | --- | --- |
| 抽出対象となるPDFの最大ページ数 | 5000（新しいアップロード用） | 100( すべてのPDF) |

関連トピック [Dynamic Mediaの制限](/help/limitations.md).

## PDFファイルの準備 {#preparing-your-pdf-files}

PDFファイルをAdobe Dynamic Media Classicにアップロードする前に、次の手順で準備します。

* ファイルを簡単にアップロードするには、すべてのファイルをコンピューターまたはネットワーク上の同じフォルダーに配置します。
* ページの順番と同じになるように、英数字の順にファイルの名前を付けます。ページの順番に合わせておけば、ファイルをアップロードした後に正しい順番でページを並べやすくなります。
* PDFページに内トンボ、登録ターゲット、カラーバーのどれが含まれているかを確認するには、ページを調べます。 このようなマークが入っていると、文書を印刷するときにこのマークに沿ってページが切り抜かれるため、Web に eCatalog を掲載する前に削除しておく必要があります。Adobe Dynamic Media Classicには、PDFファイルをアップロードする際のトリミングマークのオプションが用意されています。
* eCatalog をキーワードで検索できるようにする場合は、PDF ファイルが画像化されていないかどうかを確認してください。画像化された PDF ファイルでは、検索語を抽出できなくなります。PDF ファイルが画像化されているかどうかを確認するには、PDF のテキストを選択できるかどうか試してみます。テキストを選択できない場合、PDFは統合され、ビューアは eCatalog 内のキーワードで検索できません。
* PDF ファイルは印刷を目的としたファイルなので、通常、CMYK 画像が含まれています。デフォルトでは、Adobe Dynamic Media Classicは、これらの CMYK 画像をインテリジェントに検出し、内部 CMYK カラープロファイルを使用して変換できます。 ただし、必要に応じて、カスタムカラープロファイルを使用して CMYK 画像を変換することもできます。

   詳しくは、 [ICC(International Color Consortium) プロファイル](icc-profiles.md#icc_profiles).

## ベストプラクティスの PDF アップロードオプション {#best-practice-pdf-upload-options}

各アップロード方法について詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

アップロードするファイルを選択し、次の&#x200B;*ベストプラクティス* PDF オプションを選択します。

* **切り抜きオプション**  — アップロードオプションを設定ダイアログボックスで、 **[!UICONTROL 切り抜きオプション]**. PDFページに内トンボ、トンボまたは他のマークが含まれている場合、 **[!UICONTROL 切り抜き]** ドロップダウンリストで、「 **[!UICONTROL 手動]**. ページの上下左右の端からそれぞれ切り抜くピクセル数を入力します。内トンボは、多くの場合、半インチのマージンに設定されます。 次を選択したとします。 **[!UICONTROL 150]** （推奨）ピクセル/インチの解像度として、「上」、「右」、「下」、「左」の各テキストボックスに 75、75、75、75 と入力します。 この場合、余白から半インチ（150 ppi、1 の半分は 75 ピクセルに等しい）を切り抜きます。

* **処理中**  — アップロードオプションを設定ダイアログボックスで、 **[!UICONTROL PDFオプション]**. 内 **[!UICONTROL 処理中]** ドロップダウンリストで、「 **[!UICONTROL ラスタライズ]**. すべてのページと画像を eCatalog で表示するためには、PDF ファイルをラスタライズする必要があります。

* **検索語を抽出（オプション）**  — アップロードオプションを設定ダイアログボックスで、 **[!UICONTROL PDFオプション]**. 「抽出」ドロップダウンリストで、「 」を選択します。 **[!UICONTROL 検索語]** 閲覧者が eCatalog 内のキーワードで検索できるようにする場合。

* **複数のページPDFから eCatalog を自動生成（オプション）**  — アップロードオプションを設定ダイアログボックスで、 **[!UICONTROL PDFオプション]**. 選択 **[!UICONTROL 複数のページから eCatalog を自動生成PDF]** を使用して、アップロード時に eCatalog を自動的に作成できます。 PDF ファイルを選択してから「ビルド」コマンドを選択しなくても、eCatalog 画面が開き、eCatalog で作業できるようになります。eCatalog の名前は、PDF ファイルの名前をもとに付けられます。

* **解像度**  — アップロードオプションを設定ダイアログボックスで、 **[!UICONTROL PDFオプション]**. 内 **[!UICONTROL 解像度]** テキストフィールドに値を入力します。 Adobe Dynamic Media Classicは 150 ピクセル/インチを推奨します。

* **カラースペース**  — アップロードオプションを設定ダイアログボックスで、 **[!UICONTROL PDFオプション]**. 「カラースペース」ドロップダウンリストで、「 **[!UICONTROL 自動検出]**. 一般的に PDF のカラースペースは、印刷出力が目的の場合には CMYK、オンライン表示が目的の場合には RGB になります。PDF に両方のカラースペースが含まれている場合は、「RGB としてレンダリング」または「CMYK としてレンダリング」のいずれかを選択して、一方のカラースペースを選択できます。例えば、ページのグラフィックに CMYK カラースペースが使用され、ピクチャに RGB カラースペースが使用されている場合には、両方のカラースペースが PDF に含まれます。ICC プロファイルをアップロードしておくと、カラースペースメニューにその名前が表示され、選択して使用できます。

   詳しくは、 [ICC(International Color Consortium) プロファイル](/help/icc-profiles.md).

* **カラープロファイルオプション**  — アップロードオプションを設定ダイアログボックスで、 **[!UICONTROL カラープロファイルオプション]**&#x200B;をクリックし、「カラープロファイル」オプションを選択します。

   * **元のカラースペースを保持**  — 元のカラースペースを保持します。

   * **カスタム開始日/終了日**  — サブメニューを開き、 **[!UICONTROL 変換元]** および **[!UICONTROL 変換先]** カラースペース。 Photoshopの標準的なカラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。

<!-- * **Convert To SRGB** - Converts to SRGB (Standard Red Green Blue). SRGB is the recommended color space for displaying images on web pages. -->

詳しくは、 [ICC(International Color Consortium) プロファイル](icc-profiles.md#icc_profiles).

>[!NOTE]
>
>すべての PDF オプションについて詳しくは、[PDF アップロードオプション](pdfs.md#pdf_upload_options)を参照してください。
