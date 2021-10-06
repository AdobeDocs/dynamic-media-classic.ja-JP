---
title: 「クイックスタート：eCatalogs"
description: Adobe Dynamic Media Classicの eCatalog テクニックをすぐに使い始めるのに役立つ概要とクイックスタート eCatalog の概要です。
uuid: 1ec41927-3df6-4845-8d9d-bb92cf6dca08
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 781dacd0-ef0c-42b7-92e0-12791994874d
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '1558'
ht-degree: 38%

---

# クイックスタート：eCatalogs{#quick-start-ecatalogs}

eCatalog とは、カタログ、パンフレット、チラシ、製品マニュアル、広告用のビラのような印刷物をデジタル化し、Web で参照できるようにしたものです。eCatalog は、Web サイト上で eCatalog ビューアを使用して表示します。このビューアを使用すると、印刷物を読むときと同じ感覚で資料を読むことができます。

次のトレーニングビデオも参照してください。

* [クイックスタート 1:eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [クイックスタート 2:eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

eCatalog に対して選択した設定に応じて、ビューアで次の操作を実行できます。

* キーワードまたはキーワードをカタログで検索します。 検索結果は、カタログの左側の検索パネルにサムネールのリストとして表示されます。 クリック可能な各サムネールは、ハイライト表示された検索語句が見つかったカタログ見開きを表します。

* ソーシャルメディアを介してカタログを共有するオフラインで表示するには、カタログをダウンロードします。[ お気に入り ] を有効にして、すばやく戻す項目をマークするか、カタログを印刷します。
* 目次またはページグリッドビューを使用してカタログを移動する。ページの中央端をクリックして前または後に移動します。
* ズームイン、ズームアウト、およびパンを実行して、ページの項目を確認することができます。
* ポインターをページ領域（画像マップと呼ばれます）の上に移動して、項目に関する情報を含むポップアップウィンドウを表示します。
* ページ領域を選択すると、新しい Web ページが開き、項目に関する詳細情報が表示されます。
* ノート注釈を書き、eCatalog のページに貼り付けることができます。
* 関連する Web ページまたはコンテキスト内情報パネルを起動する場合は、画像マップアイコンをタップします。
* ピンチズームやスワイプによるページめくりなど、ジェスチャ操作を使用します。
* キーワードと一致する項目を検索することができます。

![ユーザーに表示される eCatalog。A) eCatalog を開くページ B) eCatalog が 2 ページ目に変わりました。](/help/assets/ec_cat_viewer_popup.png)

eCatalog を作成するときに、通常は、Adobe® Acrobat® やその他の印刷プログラムで作成した高解像度の PDF ファイルを使用しますが、画像ファイルから作成することもできます。

eCatalog を作成する際に、ページや見開きページの並び順を選択することができます。また、見開きページの表示単位を 1 ページにするのか、2 ページにするのか、または任意指定のページ数にするのかを選択することもできます。ページ領域の画像マップを作成して、例えばページ上の領域を選択し、Web サイト上で新しいページを開くことができます。 eCatalog 画面内の情報パネル設定を使用して、表示するロールオーバーテキストを管理できます。eCatalog ビューアを設定する手段として、100 以上の様々な設定オプションが用意されています。また、閲覧者に合わせて、ビューアの機能や外観を変更することができます。

>[!NOTE]
>
>Dynamic Media - Scene7モードのユーザーで、eCatalog を使用する場合は、「CRXDE Lite」で `pdfbrochure` 値を編集します。 そのためには、Adobe Experience Managerで、**[!UICONTROL ツール]** > **[!UICONTROL 一般]** > **[!UICONTROL CRXDE Lite]** に移動します。 左側のパネルナビゲーションツリーで、`/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf` に移動します。
>
>右下のウィンドウの「**[!UICONTROL プロパティ]**」タブで、`jobParam` 行を選択します。 `pdfbrochure` の値を `false` から `true` に設定します。 `pdfbrochure=true` のように
>
>CRXDE Liteページの左上隅で、「**[!UICONTROL すべて保存]**」を選択します。
>
>これで、Adobe Dynamic Media Classicで eCatalog を作成できるようになりました。

ここでは、eCatalog の操作方法をすばやく習得できるように、手順について簡潔に説明します。手順 1 ～ 7 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

## 1.PDFファイルのアップロード

eCatalog のもとになるファイルは、ほとんどの場合 Adobe PDF ファイルです。PDF ファイルは印刷を目的としたファイルなので、通常、CMYK 画像が含まれています。Adobe Dynamic Media Classicは、これらの画像を検出し、標準の CMYK カラープロファイルを使用して変換します。 ただし、カスタムカラープロファイルをアップロードして使用する必要があります。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」を選択して、eCatalog のPDFファイルまたは画像のアップロードを開始します。 デスクトップからファイルをアップロードすることもできますが、ファイル数が多い、またはファイルのサイズが 100 MB を超える場合には、FTP を使用することをお勧めします。

「PDF オプション」を選択すると、アップロード画面に、適正な解像度とカラースペースで PDF ファイルをアップロードするためのオプションが表示されます。解像度の推奨値は 150 pixel/インチです。PDF ファイルをアップロードするときに eCatalog を作成する場合は、「複数ページの PDF から eCatalog を自動生成」オプションを選択します。

[PDFファイルのアップロード ](uploading-pdf-files.md#uploading_the_pdf_files) を参照してください。

## 2. eCatalog を作成する

参照パネルで「PDF」または「画像ファイル」を選択して、eCatalog を作成します。 「**[!UICONTROL ビルド]**」を選択し、「**[!UICONTROL eCatalogs]**」を選択します。

eCatalog ページの「**[!UICONTROL ページの並べ替え]**」タブで、「レイアウト」オプションを選択します。**[!UICONTROL 1 上]**、**[!UICONTROL 2 上]**、または **[!UICONTROL カスタム]**。 ページや見開きページの配置変更は、それらをドラッグすることで行えますが、eCatalog のサイズが大きい場合には、移動先メニューでページ名を選択することでも行えます。

ページを追加するには、アセットライブラリのフォルダを選択してから、PDF ファイルまたは画像ファイルをページ順序画面にドラッグします。デフォルトのページ番号の代わりに、カスタムのページ名を指定したり、多くのページ名を読み込んだりできます。

「**[!UICONTROL 保存]**」を選択し、eCatalog の名前を入力し、保存するAdobe Dynamic Media Classicフォルダーを選択して、「**[!UICONTROL 保存]**」を選択します。 ページの順序を変更したり、eCatalog を編集したりするたびに、「**[!UICONTROL 保存]**」をクリックして変更を保存します。

[eCatalog の作成 ](creating-ecatalog.md) を参照してください。

## 3.画像マップの作成

画像マップは、eCatalog ページに別の縦横比を追加します。 画像マップとは、ページの中で、項目に関する詳細情報を表示できる領域を指します。画像マップにポインタを合わせると、その項目の説明が表示されます。また、画像マップをクリックすると、外部参照先の Web ページに移動し、項目に関する詳細情報を参照できます。

画像マップを作成するには、eCatalog 画面を開き、次に、eCatalog 画面の「**[!UICONTROL ページをマップ]**」タブに移動し、長方形画像マップツールまたは多角形画像マップツールでマップをフレーム化します。 パンツール  を使用すると、画像マップの境界をドラッグしながら、位置とサイズを調整することができます。

画像マップのフレームを作成した後、画像マップを選択する際に表示する URL アドレスを入力します。 画像マップにポインタを合わせたときに表示するロールオーバーテキストを入力することもできます。

[eCatalog 画像マップの作成 ](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps) を参照してください。

[ 画像マップを使用して eCatalog にリッチメディアを埋め込む ](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog) を参照してください。

eCatalog 画面内の情報パネル設定を使用して、画像マップのテキストを設定および管理できます。

[eCatalog の情報パネルのコンテンツの管理 ](/help/info-panel-content-ecatalog.md) を参照してください。

## 4. eCatalog ビューアプリセットの設定

エンドユーザは eCatalog ビューアで eCatalog を表示します。管理者には eCatalog ビューアを設定する権限があります。アウトラインカラーを変更したり、eCatalog 用の自社用「スキン」を選択したりできます。Adobe Dynamic Media Classicには、eCatalog ビューアプリセットがいくつか用意されています。 eCatalog を表示するために、これらのプリセットの 1 つを選択できます。 管理者であれば、独自の eCatalog ビューアプリセットを作成することもできます。

eCatalog ビューアプリセットを作成するには、グローバルナビゲーションバーで「**[!UICONTROL 設定]**」を選択し、「**[!UICONTROL ビューアプリセット]**」を選択します。 「**** を追加」を選択し、プラットフォームを選択して、**[!UICONTROL eCatalog]**/**[!UICONTROL ビューア]** を選択します。

[eCatalog ビューアプリセットの設定 ](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets) を参照してください。

## 5. eCatalog ビューアで eCatalog をプレビューする

eCatalog ビューアのスタイルと動作は、eCatalog ビューアプリセットによって設定されます。

eCatalog ビューアプリセットで eCatalog がどのように表示されるかを確認するには、参照パネルで eCatalog を選択し、**[!UICONTROL プレビュー]** を選択します。 初期設定のビューアが開き、プレビュー画面が表示されます。

向き、カラースキーム、ページ変更のコントロール、ページをめくったときの見た目を確認します。

[eCatalog ビューアでの eCatalog のプレビュー ](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer) を参照してください。

## 6. eCatalog と関連PDFの公開

eCatalog と関連PDFを公開すると、Dynamic Media Image Server に配置され、Web サイトやアプリケーションに配信できるようになります。 公開プロセスの一環として、Adobe Dynamic Media Classicは eCatalog の URL 文字列をアクティベートします。 この URL を使用して、Dynamic Media Image Server から Web サイトまたはアプリケーションに eCatalog を呼び出します。

参照パネルで eCatalog とPDFを公開用にマークした後、グローバルナビゲーションバーの「公開」ボタンを選択して公開を開始します。 公開画面で、「**[!UICONTROL 公開を送信]**」を選択します。

[eCatalog と関連するPDFの公開 ](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs) を参照してください。

## 7. eCatalog を Web ページにリンクする

Adobe Dynamic Media Classicは、eCatalog をDynamic Media Image Server に公開する際に、eCatalog の表示に必要な URL 引き出し線文字列をアクティブにします。 この URL 文字列は、プレビュー画面および（詳細表示の）参照パネルから、パネルで URL を選択してコピーできます。 URL 文字列をコピーしておけば、Web サイトやアプリケーションでその URL を使用することができます。

Web ページのどの場所に eCatalog へのリンクを配置するのが適切か、IT 担当者と相談して決めてください。ユーザーがリンクを選択すると、eCatalog ビューアが表示され、ユーザーは eCatalog を参照できます。

[eCatalog を Web ページにリンクする ](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page) を参照してください。
