---
title: "クイックスタート： eCatalogs"
description: Adobe Dynamic Media Classicの eCatalog テクニックをすぐに使い始めるのに役立つ、概要とクイックスタート：eCatalog
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 597b7d6bd98c59a644984baeecb888f86a8975c9
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 33%

---

# クイックスタート： eCatalog{#quick-start-ecatalogs}

eCatalog とは、カタログ、パンフレット、チラシ、製品マニュアル、広告用のビラのような印刷物をデジタル化し、Web で参照できるようにしたものです。eCatalog は、Web サイト上で eCatalog ビューアを使用して表示します。このビューアを使用すると、印刷物を読むときと同じ感覚で資料を読むことができます。

次のトレーニングビデオも参照してください。

* [クイックスタート 1:eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [クイックスタート 2:eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

eCatalog に対して選択した設定に応じて、ビューアで次の操作を実行できます。

* キーワードまたはキーワードのカタログを検索します。 検索結果は、カタログの左側の検索パネルにサムネールのリストとして表示されます。 クリック可能な各サムネールは、ハイライト表示された検索語句が見つかったカタログ見開きを表します。

* ソーシャルメディアを介してカタログを共有する、カタログをダウンロードしてオフラインで表示する、お気に入りを有効にして、すばやく戻す項目をマークする、またはカタログを印刷する。
* 目次またはページグリッド表示を使用してカタログを移動します。ページの中央端を選択して前または後に移動します。
* ズームイン、ズームアウト、およびパンを実行して、ページの項目を確認することができます。
* ページ領域（画像マップと呼ばれます）の上にポインターを移動すると、項目に関する情報を含むポップアップウィンドウが表示されます。
* ページ領域を選択すると、新しい Web ページが開き、項目に関する詳細情報が表示されます。
* ノート注釈を書き、eCatalog のページに貼り付けることができます。
* 関連する Web ページまたはコンテキスト内情報パネルを起動する場合は、画像マップアイコンをタップします。
* ピンチズームやスワイプによるページめくりなど、ジェスチャ操作を使用します。
* キーワードと一致する項目を検索することができます。

![ユーザに表示される eCatalog。 A) eCatalog の開封ページ B)eCatalog を 2 ページ目に切り替えた。](/help/using/assets/ec_cat_viewer_popup.png)

eCatalog を作成する場合、通常はAdobe Acrobatまたは他の印刷プログラムで作成された高解像度PDFファイルを使用しますが、画像ファイルから eCatalog を作成することもできます。

eCatalog を作成する際に、ページや見開きページの並び順を選択することができます。また、見開きページの表示単位を 1 ページにするのか、2 ページにするのか、または任意指定のページ数にするのかを選択することもできます。ページ領域の画像マップを作成して、例えばページ上の領域を選択したり、Web サイト上で新しいページを開いたりできます。 eCatalog 画面内の情報パネル設定を使用して、表示するロールオーバーテキストを管理できます。eCatalog ビューアを設定する手段として、100 以上の様々な設定オプションが用意されています。また、閲覧者に合わせて、ビューアの機能や外観を変更することができます。

>[!NOTE]
>
>Dynamic Media - Scene7モードのユーザーで、eCatalog を使用する場合は、 `pdfbrochure` CRXDE Liteの値。 これをおこなうには、Adobe Experience Managerで、 **[!UICONTROL ツール]** > **[!UICONTROL 一般]** > **[!UICONTROL CRXDE Lite]**. 左側のパネルナビゲーションツリーで、に移動します。 `/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`.
>
>右下のウィンドウで、 **[!UICONTROL プロパティ]** タブで、 `jobParam` 行。 次の値を設定： `pdfbrochure` から `false` から `true`. 例： `pdfbrochure=true`
>
>CRXDE Liteページの左上隅で、「 **[!UICONTROL すべて保存]**.
>
>これで、Adobe Dynamic Media Classicで eCatalog を作成できるようになりました。

ここでは、eCatalog の操作方法をすばやく習得できるように、手順について簡潔に説明します。手順 1 ～ 7 に従ってください。各手順の後に、トピックの見出しへの相互参照があり、詳細を確認できます。

## 1.PDFファイルをアップロード

eCatalog のもとになるファイルは、ほとんどの場合 Adobe PDF ファイルです。PDF ファイルは印刷を目的としたファイルなので、通常、CMYK 画像が含まれています。Adobe Dynamic Media Classicは、これらの画像を検出し、標準の CMYK カラープロファイルを使用して変換します。 ただし、カスタムカラープロファイルをアップロードして使用する必要があります。

グローバルナビゲーションバーで、 **[!UICONTROL アップロード]** :eCatalog 用のPDFファイルまたは画像のアップロードを開始します。 ファイルは、デスクトップから、または FTP 経由でアップロードできます。多数のファイルまたは 100 MB を超えるファイルをアップロードする場合は、FTP を使用することをお勧めします。

「PDF オプション」を選択すると、アップロード画面に、適正な解像度とカラースペースで PDF ファイルをアップロードするためのオプションが表示されます。解像度の推奨値は 150 pixel/インチです。PDF ファイルをアップロードするときに eCatalog を作成する場合は、「複数ページの PDF から eCatalog を自動生成」オプションを選択します。

詳しくは、 [PDFファイルのアップロード](uploading-pdf-files.md#uploading_the_pdf_files).

## 2. eCatalog を作成する

[ 参照 ] パネルで [PDF] または [ 画像ファイル ] を選択して eCatalog を作成します。 選択 **[!UICONTROL ビルド]**&#x200B;を選択し、次を選択します。 **[!UICONTROL eCatalogs]**.

eCatalog ページの **[!UICONTROL ページを並べ替え]** 「 」タブで、「レイアウト」オプションを選択します。 **[!UICONTROL 1 アップ]**, **[!UICONTROL 2 アップ]**&#x200B;または **[!UICONTROL カスタム]**. ページや見開きページの配置変更は、それらをドラッグすることで行えますが、eCatalog のサイズが大きい場合には、移動先メニューでページ名を選択することでも行えます。

ページを追加するには、アセットライブラリのフォルダを選択してから、PDF ファイルまたは画像ファイルをページ順序画面にドラッグします。デフォルトのページ番号の代わりに、カスタムのページ名を指定したり、多くのページ名を読み込んだりできます。

選択 **[!UICONTROL 保存]**、eCatalog の名前を入力し、保存するAdobe Dynamic Media Classicフォルダを選択して、 **[!UICONTROL 保存]**. ページの順序を変更したり eCatalog を編集したりするたびに、「 」を選択して変更を保存します。 **[!UICONTROL 保存]**.

詳しくは、 [eCatalog の作成](creating-ecatalog.md).

## 3.画像マップを作成する

画像マップは、eCatalog ページに別の縦横比を追加します。 画像マップとは、ページの中で、項目に関する詳細情報を表示できる領域を指します。画像マップにポインタを合わせると、その項目の説明が表示されます。また、画像マップをクリックすると、外部参照先の Web ページに移動し、項目に関する詳細情報を参照できます。

画像マップを作成するには、eCatalog 画面を開き、その後、 **[!UICONTROL ページをマッピング]** eCatalog 画面のタブに移動し、長方形画像マップツールまたは多角形画像マップツールでマップを囲みます。 パンツール  を使用すると、画像マップの境界をドラッグしながら、位置とサイズを調整することができます。

画像マップをフレーム化した後、画像マップを選択したときに表示する URL アドレスを入力します。 画像マップにポインタを合わせたときに表示するロールオーバーテキストを入力することもできます。

詳しくは、 [eCatalog 画像マップを作成](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps).

詳しくは、 [画像マップを使用した eCatalog へのリッチメディアの埋め込み](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog).

eCatalog 画面内の情報パネル設定を使用して、画像マップのテキストを設定および管理できます。

詳しくは、 [eCatalog 内の情報パネルのコンテンツを管理](/help/using/info-panel-content-ecatalog.md).

## 4. eCatalog ビューアプリセットを設定する

エンドユーザは eCatalog ビューアで eCatalog を表示します。管理者には eCatalog ビューアを設定する権限があります。アウトラインカラーを変更し、新しい「スキン」を選択して eCatalog にブランドを付けることができます。 Adobe Dynamic Media Classicには、「ベストプラクティス」の eCatalog ビューアプリセットがいくつか用意されています。 eCatalog を表示するために、これらのプリセットの 1 つを選択できます。 管理者であれば、独自の eCatalog ビューアプリセットを作成することもできます。

eCatalog ビューアプリセットを作成するには、グローバルナビゲーションバーで **[!UICONTROL 設定]**&#x200B;を選択し、次を選択します。 **[!UICONTROL ビューアプリセット]**. 選択 **[!UICONTROL 追加]**、プラットフォームを選択し、「 」を選択します。 **[!UICONTROL eCatalog]** > **[!UICONTROL 閲覧者]**.

詳しくは、 [eCatalog ビューアプリセットの設定](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets).

## 5. eCatalog ビューアで eCatalog をプレビューする

eCatalog ビューアのスタイルと動作は、eCatalog ビューアプリセットによって設定されます。

eCatalog ビューアプリセットで eCatalog がどのように表示されるかを確認するには、参照パネルで eCatalog を選択し、 **[!UICONTROL プレビュー]**. 初期設定のビューアが開き、プレビュー画面が表示されます。

向き、カラースキーム、ページ変更のコントロール、ページをめくったときの見た目を確認します。

詳しくは、 [eCatalog ビューアで eCatalog をプレビューする](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer).

## 6. eCatalog と関連PDFを公開

eCatalog と関連PDFを公開すると、Dynamic Media Image Server に配置され、Web サイトやアプリケーションに配信できるようになります。 公開プロセスの一環として、Adobe Dynamic Media Classicは eCatalog の URL 文字列をアクティベートします。 この URL を使用して、Dynamic Media Image Server から eCatalog を Web サイトまたはアプリケーションに呼び出します。

参照パネルで公開用の eCatalog とPDFをマークした後、グローバルナビゲーションバーの「公開」ボタンを選択して公開を開始します。 公開画面で、「 」を選択します。 **[!UICONTROL 公開を送信]**.

詳しくは、 [eCatalog と関連PDFを公開](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs).

## 7. eCatalog を Web ページにリンクする

Adobe Dynamic Media Classicは、eCatalog をDynamic Media Image Server に公開する際に、eCatalog の表示に必要な URL 引き出し線文字列をアクティベートします。 この URL 文字列は、プレビュー画面および（詳細ビューの）参照パネルから、パネルで「 URLs 」を選択することでコピーできます。 URL 文字列をコピーしておけば、Web サイトやアプリケーションでその URL を使用することができます。

Web ページのどの場所に eCatalog へのリンクを配置するのが適切か、IT 担当者と相談して決めてください。ユーザがリンクを選択すると、eCatalog ビューアが表示され、ユーザは eCatalog を参照できます。

詳しくは、 [eCatalog を Web ページにリンクする](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page).
