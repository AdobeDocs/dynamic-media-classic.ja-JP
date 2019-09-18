---
title: 「クイックスタート：eCatalogs"
seo-title: 「クイックスタート：eCatalogs"
description: 'null'
seo-description: eCatalogの操作方法をすばやく習得できるように、eCatalogの概要とクイックスタートガイドを参照してください。
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: 管理者
content-type: 参照
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
translation-type: tm+mt
source-git-commit: e1b74f30faab334453f941e9075910c8a8565462

---


# クイックスタート：eCatalog{#quick-start-ecatalogs}

eCatalog とは、カタログ、パンフレット、チラシ、製品マニュアル、広告用のビラのような印刷物をデジタル化し、Web で参照できるようにしたものです。eCatalog は、Web サイト上で eCatalog ビューアを使用して表示します。このビューアを使用すると、印刷物を読むときと同じ感覚で資料を読むことができます。eCatalogに対して選択した設定に応じて、Viewerでは次の操作を行うことができます。

* カタログでキーワードを検索します。 検索結果は、カタログの左側の検索パネルにサムネールのリストとして表示されます。 クリック可能な各サムネールは、ハイライト表示された検索語が見つかったカタログ見開きを表します。

* ソーシャルメディアを使用してカタログを共有する。カタログをダウンロードしてオフラインで表示する[お気に入り]を有効にすると、すばやく戻る項目をマークしたり、カタログを印刷したりできます。
* 目次またはページグリッドビューを使用してカタログ内を移動します。ページの中央端をクリックして、前または後に移動します。
* ズームイン、ズームアウト、およびパンを実行して、ページの項目を確認することができます。
* 画像マップと呼ばれるページ領域にポインタを合わせると、ポップアップウィンドウが開き、その項目に関する情報が表示されます。
* ページ領域をクリックすると、新しい Web ページが開き、その項目に関する詳細情報が表示されます。
* ノート注釈を書き、eCatalog のページに貼り付けることができます。
* 画像マップアイコンをタップし、関連する Web ページまたはコンテキスト内情報パネルを起動します。
* ピンチズームやスワイプによるページめくりなど、ジェスチャ操作を使用します。
* キーワードと一致する項目を検索することができます。

![eCatalog の外観。A) eCatalogの開始ページ B)eCatalog turned to page 2.](/help/assets/ec_cat_viewer_popup.png)

eCatalog を作成するときに、通常は、Adobe® Acrobat® やその他の印刷プログラムで作成した高解像度の PDF ファイルを使用しますが、画像ファイルから作成することもできます。

eCatalog を作成する際に、ページや見開きページの並び順を選択することができます。また、見開きページの表示単位を 1 ページにするのか、2 ページにするのか、または任意指定のページ数にするのかを選択することもできます。画像マップをページ領域として作成すれば、その領域をクリックしたときに、Web サイトの別のページを開くといった操作ができるようになります。eCatalog 画面内の情報パネル設定を使用して、表示するロールオーバーテキストを管理できます。eCatalog ビューアを設定する手段として、100 以上の様々な設定オプションが用意されています。また、閲覧者に合わせて、ビューアの機能や外観を変更することができます。

>[!NOTE]
>
>AEMダイナミックメディア — Scene7モードのユーザでeCatalogを使用する場合は、CRXDE Liteで値を編集する `pdfbrochure` 必要があります。 これを行うには、AEMでUICONTROLツール/一般/CRXDE Lite **[をクリックします]**。 左側のパネルナビゲーションツリーで、に移動しま `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`す。
右下のウィンドウの「 **Properties** 」タブで、行を選択し `jobParam` ます。 からに値を設 `pdfbrochure` 定し `false` ます `true`。 「CRXDE Lite `pdfbrochure=true`ページの左上隅にある「すべて保存」をクリッ **クします**。
これで、SPSでeCatalogをオーサリングできるようになります。

**クイックスタート**

ここでは、eCatalog の操作方法をすばやく習得できるように、手順について簡潔に説明します。手順 1 ～ 7 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

**1. PDF ファイルのアップロード**

eCatalog のもとになるファイルは、ほとんどの場合 Adobe PDF ファイルです。PDF ファイルは印刷を目的としたファイルなので、通常、CMYK 画像が含まれています。Scene7 Publishing System では、これらの画像が検出され、標準の CMYK カラープロファイルに従って変換されますが、ただし、カスタムカラープロファイルをアップロードして使用する必要があることも考えられます。

グローバルナビゲーションバーの「アップロード」をクリックして、eCatalog用のPDFファイルまたは画像のアップロードを開始します。 デスクトップからファイルをアップロードすることもできますが、ファイル数が多い、またはファイルのサイズが 100 MB を超える場合には、FTP を使用することをお勧めします。

「PDF オプション」を選択すると、アップロード画面に、適正な解像度とカラースペースで PDF ファイルをアップロードするためのオプションが表示されます。解像度の推奨値は 150 pixel/インチです。PDF ファイルをアップロードするときに eCatalog を作成する場合は、「複数ページの PDF から eCatalog を自動生成」オプションを選択します。

詳しくは、[PDF ファイルのアップロード](uploading-pdf-files.md#uploading_the_pdf_files)を参照してください。

**2．eCatalog の作成**

eCatalog を作成するには、参照パネルで PDF ファイルまたは画像ファイルを選択してから、「ビルド」ボタンをクリックし、「eCatalog」を選択します。eCatalog 画面が開きます。

「ページ順序」タブで、レイアウト用ボタンの 1 アップ、2 アップ、カスタムのいずれかを選択して、見開きページの単位を 1 ページにするのか、2 ページにするのか、または任意指定のページ数にするのかを決めます。ページや見開きページの配置変更は、それらをドラッグすることで行えますが、eCatalog のサイズが大きい場合には、移動先メニューでページ名を選択することでも行えます。

ページを追加するには、アセットライブラリのフォルダを選択してから、PDF ファイルまたは画像ファイルをページ順序画面にドラッグします。初期設定でページ番号が付けられますが、カスタムページ名を付けることもできます。また、ページ名が多い場合には、ページ名を読み込むこともできます。

「保存」ボタンをクリックし、eCatalog の名前を入力し、保存先の SPS フォルダを選択し、「保存」ボタンを選択します。ページの順番を変えたり、eCatalog を編集したときは、「保存」ボタンをクリックして変更内容を保存してください。

詳しくは、[eCatalog の作成](creating-ecatalog.md)を参照してください。

**3. 画像マップの作成**

画像マップを使用すると、eCatalog のページに便利な機能を追加できます。画像マップとは、ページの中で、項目に関する詳細情報を表示できる領域を指します。画像マップにポインタを合わせると、その項目の説明が表示されます。また、画像マップをクリックすると、外部参照先の Web ページに移動し、項目に関する詳細情報を参照できます。

画像マップを作成するには、eCatalog 画面を開き、eCatalog 画面の「ページをマップ」タブを選択し、長方形画像マップツール  または多角形画像マップツール  を使用して画像マップを描画します。パンツール  を使用すると、画像マップの境界をドラッグしながら、位置とサイズを調整することができます。

画像マップの描画後、画像マップをクリックしたときの移動先となる URL アドレスを入力します。画像マップにポインタを合わせたときに表示するロールオーバーテキストを入力することもできます。

詳しくは、[eCatalog 画像マップの作成](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)を参照してください。

詳しくは、[画像マップを使用してリッチメディアを eCatalog に埋め込む](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)を参照してください。

eCatalog 画面内の情報パネル設定を使用して、画像マップのテキストを設定および管理できます。

詳しくは、[情報パネルのコンテンツの管理](info-panel-content.md#managing-info-panel-content)を参照してください。

**4. eCatalog のビューアプリセットの設定**

エンドユーザは eCatalog ビューアで eCatalog を表示します。管理者には eCatalog ビューアを設定する権限があります。アウトラインカラーを変更したり、eCatalog 用の自社用「スキン」を選択したりできます。ダイナミックMedia Classicには、eCatalogビューアプリセットがいくつか用意されています。 eCatalogの表示に使用するプリセットを選択できます。 管理者であれば、独自の eCatalog ビューアプリセットを作成することもできます。

eCatalog ビューアプリセットを作成するには、グローバルナビゲーションバーの「設定」ボタンをクリックして、「ビューアプリセット」を選択します。Then click Add, choose a platform, and choose **[UICONTROL eCatalog &gt; Viewer]**.

詳しくは、[eCatalog ビューアプリセットの設定](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)を参照してください。

**5. eCatalog ビューアによる eCatalog のプレビュー**

eCatalog ビューアのスタイルと動作は、eCatalog ビューアプリセットによって設定されます。

eCatalog ビューアプリセットで eCatalog がどのように表示されるかを確認するには、参照パネルで eCatalog を選択し、「プレビュー」をクリックします。初期設定のビューアが開き、プレビュー画面が表示されます。

向き、カラースキーム、ページ変更のコントロール、ページをめくったときの見た目を確認します。

詳しくは、[eCatalog ビューアによる eCatalog のプレビュー](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)を参照してください。

**6. eCatalogと関連PDFの公開**

公開したeCatalogと関連PDFは、Dynamic Media Image Serverに保存され、Webサイトやアプリケーションに配信できるようになります。 公開処理中に、eCatalog の URL 文字列がアクティブになります。このURLを使用して、eCatalogをダイナミックメディアイメージサーバからWebサイトやアプリケーションに呼び出します。

参照パネルでeCatalogとPDFを公開用にマークした後、グローバルナビゲーションバーの「公開」ボタンを選択して公開を開始します。 公開画面で、「公開を開始」をクリックします。

詳しくは、 [eCatalogと関連PDFの公開を参照してください](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)。

**7. Web ページへの eCatalog のリンク**

Dynamic Media Classicは、eCatalogをダイナミックメディアイメージサーバに公開する際にeCatalogを表示するのに必要なURL呼び出し文字列をアクティブにします。 プレビュー画面や参照パネル（詳細ビュー）でパネル内の URL を選択すれば、この URL 文字列をコピーすることができます。URL 文字列をコピーしておけば、Web サイトやアプリケーションでその URL を使用することができます。

Web ページのどの場所に eCatalog へのリンクを配置するのが適切か、IT 担当者と相談して決めてください。このリンクをユーザがクリックすると、eCatalog ビューアが開き、eCatalog が表示されます。

詳しくは、[Web ページへの eCatalog のリンク](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)を参照してください。
