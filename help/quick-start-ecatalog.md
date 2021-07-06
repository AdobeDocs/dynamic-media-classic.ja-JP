---
title: 「クイックスタート：eCatalogs"
description: eCatalogのテクニックをすぐに使い始めるのに役立つ、紹介とクイックスタートのeCatalogです。
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic，ビューア，eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 50%

---

# クイックスタート：eCatalogs{#quick-start-ecatalogs}

eCatalog とは、カタログ、パンフレット、チラシ、製品マニュアル、広告用のビラのような印刷物をデジタル化し、Web で参照できるようにしたものです。eCatalog は、Web サイト上で eCatalog ビューアを使用して表示します。このビューアを使用すると、印刷物を読むときと同じ感覚で資料を読むことができます。eCatalogに対して選択した設定に応じて、ビューアで次の操作を実行できます。

* キーワードまたはキーワードをカタログで検索します。 検索結果は、カタログの左側の検索パネルにサムネールのリストとして表示されます。 クリック可能な各サムネールは、ハイライト表示された検索語句が見つかったカタログ見開きを表します。

* ソーシャルメディアを介してカタログを共有するオフラインで表示するには、カタログをダウンロードします。お気に入りを有効にして、すばやく戻す項目をマークするか、カタログを印刷します。
* 目次またはページグリッドビューを使用してカタログを移動する。ページの中央をクリックして前または後に移動します。
* ズームイン、ズームアウト、およびパンを実行して、ページの項目を確認することができます。
* ポインターをページ領域（画像マップと呼ばれます）の上に移動して、項目に関する情報を含むポップアップウィンドウを表示します。
* ページ領域をクリックすると、新しいWebページが開き、項目の詳細が表示されます。
* ノート注釈を書き、eCatalog のページに貼り付けることができます。
* 関連するWebページまたはコンテキスト内情報パネルを起動する場合は、画像マップアイコンをタップします。
* ピンチズームやスワイプによるページめくりなど、ジェスチャ操作を使用します。
* キーワードと一致する項目を検索することができます。

![eCatalogがユーザーに表示される状態。A) eCatalogの開始ページ B) eCatalogが2ページ目に変わりました。](/help/assets/ec_cat_viewer_popup.png)

eCatalog を作成するときに、通常は、Adobe® Acrobat® やその他の印刷プログラムで作成した高解像度の PDF ファイルを使用しますが、画像ファイルから作成することもできます。

eCatalog を作成する際に、ページや見開きページの並び順を選択することができます。また、見開きページの表示単位を 1 ページにするのか、2 ページにするのか、または任意指定のページ数にするのかを選択することもできます。画像マップをページ領域として作成すれば、その領域をクリックしたときに、Web サイトの別のページを開くといった操作ができるようになります。eCatalog 画面内の情報パネル設定を使用して、表示するロールオーバーテキストを管理できます。eCatalog ビューアを設定する手段として、100 以上の様々な設定オプションが用意されています。また、閲覧者に合わせて、ビューアの機能や外観を変更することができます。

>[!NOTE]
>
>Dynamic Media - Scene7モードのユーザーで、eCatalogを使用する場合は、CRXDE Liteで`pdfbrochure`値を編集する必要があります。 これをおこなうには、Adobe Experience Managerで、**[!UICONTROL ツール]** / **[!UICONTROL 一般]** / **[!UICONTROL CRXDE Lite]**&#x200B;をクリックします。 左側のパネルのナビゲーションツリーで、`/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`に移動します。
>
>右下のウィンドウの「**[!UICONTROL プロパティ]**」タブで、`jobParam`行を選択します。 `pdfbrochure`の値を`false`から`true`に設定します。 `pdfbrochure=true`のように
>
>CRXDE Liteページの左上隅にある「**[!UICONTROL すべて保存]**」をクリックします。
>
>これで、Dynamic Media ClassicでeCatalogを作成できるようになりました。

ここでは、eCatalog の操作方法をすばやく習得できるように、手順について簡潔に説明します。手順 1 ～ 7 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

## 1. PDFファイルのアップロード

eCatalog のもとになるファイルは、ほとんどの場合 Adobe PDF ファイルです。PDF ファイルは印刷を目的としたファイルなので、通常、CMYK 画像が含まれています。Dynamic Media Classicは、これらの画像を検出し、標準のCMYKカラープロファイルを使用して変換します。 ただし、カスタムカラープロファイルをアップロードして使用する必要があります。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」をクリックして、eCatalog用のPDFファイルまたは画像のアップロードを開始します。 デスクトップからファイルをアップロードすることもできますが、ファイル数が多い、またはファイルのサイズが 100 MB を超える場合には、FTP を使用することをお勧めします。

「PDF オプション」を選択すると、アップロード画面に、適正な解像度とカラースペースで PDF ファイルをアップロードするためのオプションが表示されます。解像度の推奨値は 150 pixel/インチです。PDF ファイルをアップロードするときに eCatalog を作成する場合は、「複数ページの PDF から eCatalog を自動生成」オプションを選択します。

詳しくは、[PDF ファイルのアップロード](uploading-pdf-files.md#uploading_the_pdf_files)を参照してください。

## 2. eCatalogの作成

参照パネルでPDFファイルまたは画像ファイルを選択してeCatalogを作成します。 「**[!UICONTROL ビルド]**」をクリックし、「**[!UICONTROL eCatalogs]**」を選択します。

eCatalogページの「**[!UICONTROL ページの順序]**」タブで、「レイアウト」オプションを選択します。**[!UICONTROL 1 Up]**、**[!UICONTROL 2 Up]**、または&#x200B;**[!UICONTROL Custom]**。 ページや見開きページの配置変更は、それらをドラッグすることで行えますが、eCatalog のサイズが大きい場合には、移動先メニューでページ名を選択することでも行えます。

ページを追加するには、アセットライブラリのフォルダを選択してから、PDF ファイルまたは画像ファイルをページ順序画面にドラッグします。デフォルトのページ番号の代わりに、カスタムのページ名を指定したり、多くのページ名を読み込んだりできます。

「**[!UICONTROL 保存]**」をクリックし、eCatalogの名前を入力し、保存するDynamic Media Classicフォルダーを選択して、「**[!UICONTROL 保存]**」をクリックします。 ページの順序を変更したり、eCatalogを編集したりするたびに、「**[!UICONTROL 保存]**」をクリックして変更を保存します。

詳しくは、[eCatalog の作成](creating-ecatalog.md)を参照してください。

## 3.画像マップの作成

画像マップは、eCatalogページに別の縦横比を追加します。 画像マップとは、ページの中で、項目に関する詳細情報を表示できる領域を指します。画像マップにポインタを合わせると、その項目の説明が表示されます。また、画像マップをクリックすると、外部参照先の Web ページに移動し、項目に関する詳細情報を参照できます。

画像マップを作成するには、eCatalog 画面を開き、次に、eCatalog画面の「**[!UICONTROL ページをマップ]**」タブに移動し、長方形画像マップツールまたは多角形画像マップツールでマップをフレーム化します。 パンツール  を使用すると、画像マップの境界をドラッグしながら、位置とサイズを調整することができます。

画像マップのフレームを作成した後、画像マップをクリックしたときに表示するURLアドレスを入力します。 画像マップにポインタを合わせたときに表示するロールオーバーテキストを入力することもできます。

詳しくは、[eCatalog 画像マップの作成](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)を参照してください。

詳しくは、[画像マップを使用してリッチメディアを eCatalog に埋め込む](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)を参照してください。

eCatalog 画面内の情報パネル設定を使用して、画像マップのテキストを設定および管理できます。

詳しくは、[情報パネルのコンテンツの管理](info-panel-content.md#managing-info-panel-content)を参照してください。

## 4. eCatalogビューアプリセットの設定

エンドユーザは eCatalog ビューアで eCatalog を表示します。管理者には eCatalog ビューアを設定する権限があります。アウトラインカラーを変更したり、eCatalog 用の自社用「スキン」を選択したりできます。Dynamic Media Classicには、「ベストプラクティス」のeCatalogビューアプリセットがいくつか用意されています。 eCatalogを表示するために、これらのプリセットの1つを選択できます。 管理者であれば、独自の eCatalog ビューアプリセットを作成することもできます。

eCatalogビューアプリセットを作成するには、グローバルナビゲーションバーで「**[!UICONTROL 設定]**」をクリックし、「**[!UICONTROL ビューアプリセット]**」を選択します。 次に、「****&#x200B;を追加」をクリックし、プラットフォームを選択して、**[!UICONTROL eCatalog/ビューア]**&#x200B;をクリックします。

詳しくは、[eCatalog ビューアプリセットの設定](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)を参照してください。

## 5. eCatalogビューアでのeCatalogのプレビュー

eCatalog ビューアのスタイルと動作は、eCatalog ビューアプリセットによって設定されます。

eCatalogビューアプリセットでeCatalogがどのように表示されるかを確認するには、参照パネルでeCatalogを選択し、「**[!UICONTROL プレビュー]**」をクリックします。 初期設定のビューアが開き、プレビュー画面が表示されます。

向き、カラースキーム、ページ変更のコントロール、ページをめくったときの見た目を確認します。

詳しくは、[eCatalog ビューアによる eCatalog のプレビュー](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)を参照してください。

## 6. eCatalogと関連PDFの公開

eCatalogと関連するPDFを公開すると、Dynamic Media Image Serverに配置され、Webサイトやアプリケーションに配信できるようになります。 公開プロセスの一環として、Dynamic Media ClassicはeCatalogのURL文字列をアクティベートします。 このURLを使用して、Dynamic Media Image ServerからWebサイトまたはアプリケーションにeCatalogを呼び出します。

参照パネルでeCatalogとPDFを公開用にマークした後、グローバルナビゲーションバーの「公開」ボタンを選択して公開を開始します。 公開画面で、「**[!UICONTROL 公開を送信]**」をクリックします。

[eCatalogと関連するPDFの公開](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)を参照してください。

## 7. WebページへのeCatalogのリンク

Dynamic Media Classicは、eCatalogをDynamic Media Image Serverに公開する際に、eCatalogの表示に必要なURL引き出し線文字列をアクティブ化します。 プレビュー画面や参照パネル（詳細ビュー）でパネル内の URL を選択すれば、この URL 文字列をコピーすることができます。URL 文字列をコピーしておけば、Web サイトやアプリケーションでその URL を使用することができます。

Web ページのどの場所に eCatalog へのリンクを配置するのが適切か、IT 担当者と相談して決めてください。このリンクをユーザがクリックすると、eCatalog ビューアが開き、eCatalog が表示されます。

詳しくは、[Web ページへの eCatalog のリンク](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)を参照してください。
