---
title: クイックスタート：eCatalog
description: Adobe Dynamic Media Classicで eCatalog テクニックをすぐに使い始めるのに役立つ、eCatalog の概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 25%

---

# クイックスタート：eCatalog{#quick-start-ecatalogs}

eCatalog は、デジタル版、Web 版の印刷資料です。例えば、カタログ、パンフレット、チラシ、製品マニュアル、広告の回覧などです。 eCatalog は、Web サイトの eCatalog ビューアに表示されます。 このビューアは、印刷物の読み取りエクスペリエンスをシミュレートします。

次のトレーニングビデオも参照してください。

* [ クイックスタート 1:eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [ クイックスタート 2:eCatalog](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

eCatalog に対して選択した設定に応じて、ビューアでは次の操作を実行できます。

* カタログで 1 つまたは複数のキーワードを検索します。 検索結果は、カタログの左側にある検索パネルに、サムネールのリストとして表示されます。 クリック可能な各サムネールは、ハイライト表示された検索語句が見つかったカタログスプレッドを表します。

* ソーシャルメディア経由でカタログを共有したり、カタログをダウンロードしてオフラインで表示したり、お気に入りを有効にして目的の項目をすばやく再来訪するようマークしたり、カタログを印刷したりできます。
* 目次またはページグリッド表示を使用してカタログを移動します。ページの中央の端を選択して、ページを前後に移動します。
* ズームイン、ズームアウト、およびパンを実行して、ページの項目を確認することができます。
* ポインターをページ領域（画像マップと呼ばれます）の上に移動すると、項目に関する情報を含むポップアップウィンドウが表示されます。
* ページ領域を選択すると、アイテムの詳細情報を含む新しい Web ページが開きます。
* ノート注釈を書き、eCatalog のページに貼り付けることができます。
* 関連する web ページやコンテキスト内情報パネルを起動する場合は、「画像マップのアイコン」をタップします。
* ピンチズームやスワイプによるページめくりなど、ジェスチャ操作を使用します。
* キーワードと一致する項目を検索することができます。

![ ユーザーに表示される eCatalog。 A） eCatalog 開始ページ B） eCatalog を 2.](/help/using/assets/ec_cat_viewer_popup.png) ページに変更

eCatalog を作成するには、通常、Adobe Acrobatまたは別の印刷プログラムで作成された高解像度のPDF ファイルを使用しますが、画像ファイルから eCatalog を作成することもできます。

eCatalog を作成する際に、ページや見開きページの並び順を選択することができます。また、見開きページの表示単位を 1 ページにするのか、2 ページにするのか、または任意指定のページ数にするのかを選択することもできます。ページ領域の画像マップを作成すると、たとえばページ上の領域を選択して Web サイトで新しいページを開くことができます。 eCatalog 画面内の情報パネル設定を使用して、表示するロールオーバーテキストを管理できます。eCatalog ビューアを設定する手段として、100 以上の様々な設定オプションが用意されています。また、閲覧者に合わせて、ビューアの機能や外観を変更することができます。

>[!NOTE]
>
>Dynamic Media:Scene7 モードのユーザーで eCatalog を使用する場合は、CRXDE Liteで `pdfbrochure` の値を編集します。 これを行うには、Adobe Experience Managerで、**[!UICONTROL ツール]**/**[!UICONTROL 一般]**/**[!UICONTROL 4}CRXDE Lite} に移動します。]**&#x200B;左側のパネルのナビゲーションツリーで、`/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf` に移動します。
>
>右下のウィンドウの「**[!UICONTROL プロパティ]**」タブで、`jobParam` の行を選択します。 `pdfbrochure` の値を `false` から `true` に設定します。 例：`pdfbrochure=true`
>
>CRXDE Liteページの左上隅にある「**[!UICONTROL すべて保存]**」を選択します。
>
>これで、Adobe Dynamic Media Classicで eCatalog を作成できるようになりました。

ここでは、eCatalog の操作方法をすばやく習得できるように、手順について簡潔に説明します。手順 1 ～ 7 に従ってください。各手順に続いて、詳細な情報を見つけることができるトピックの見出しへの相互参照があります。

## &#x200B;1. PDF ファイルをアップロードする

eCatalog のもとになるファイルは、ほとんどの場合 Adobe PDF ファイルです。PDF ファイルは印刷を目的としたファイルなので、通常、CMYK 画像が含まれています。Adobe Dynamic Media Classicはこれらの画像を検出し、標準の CMYK カラープロファイルを使用して変換します。 ただし、アップロードしてカスタムカラープロファイルを使用する必要があります。

グローバルナビゲーションバーの **[!UICONTROL アップロード]** を選択して、eCatalog 用のPDF ファイルまたは画像のアップロードを開始します。 デスクトップから、または FTP 経由でファイルをアップロードできます。アップロードするファイル数が多い場合や 100 MB を超えるファイルの場合は、FTP をお勧めします。

「PDF オプション」を選択すると、アップロード画面に、適正な解像度とカラースペースで PDF ファイルをアップロードするためのオプションが表示されます。解像度の推奨値は 150 pixel/インチです。「**[!UICONTROL eCatalog を自動生成]**」オプションを選択すると、PDF ファイルのアップロード時に eCatalog を作成できます。

[PDF ファイルのアップロード ](uploading-pdf-files.md#uploading_the_pdf_files) を参照してください。

## &#x200B;2. eCatalog の作成

参照パネルでPDFまたは画像ファイルを選択して、eCatalog を作成します。 「**[!UICONTROL ビルド]**」を選択し、「**[!UICONTROL eCatalog]**」を選択します。

eCatalog ページの「**[!UICONTROL ページを並べ替え]**」タブで、**[!UICONTROL 1 アップ]**、**[!UICONTROL 2 アップ]**、**[!UICONTROL カスタム]** のいずれかのレイアウトオプションを選択します。 ページや見開きページの配置変更は、それらをドラッグすることで行えますが、eCatalog のサイズが大きい場合には、移動先メニューでページ名を選択することでも行えます。

ページを追加するには、アセットライブラリのフォルダを選択してから、PDF ファイルまたは画像ファイルをページ順序画面にドラッグします。デフォルトのページ番号の代わりに、カスタムページ名を指定したり、多数のページ名を読み込んだりできます。

「**[!UICONTROL 保存]**」を選択し、eCatalog の名前を入力します。次に、この eCatalog を保存するAdobe Dynamic Media Classic フォルダーを選択して、「**[!UICONTROL 保存]**」を選択します。 ページの順序を変更したり eCatalog を編集したりするたびに、「**[!UICONTROL 保存]**」を選択して変更を保存します。

[eCatalog の作成 ](creating-ecatalog.md) を参照してください。

## 3.画像マップの作成

画像マップは、eCatalog ページに別の側面を追加します。 画像マップとは、ページの中で、項目に関する詳細情報を表示できる領域を指します。画像マップにポインタを合わせると、その項目の説明が表示されます。画像マップをクリックすると、外部参照がアクティブになり、新しい web ページが開いて項目の詳細を確認できます。

画像マップを作成するには、eCatalog 画面を開き、次に、eCatalog 画面の **[!UICONTROL ページをマップ]** タブに移動し、長方形画像マップツールまたはポリゴン画像マップツールを使用してマップをフレーム化します。 画像マップの位置とサイズは、パン ツールでマップの境界線をドラッグして調整できます。

画像マップをフレーム化した後、画像マップを選択する際に移動する URL アドレスを入力します。 画像マップにポインタを合わせたときに表示するロールオーバーテキストを入力することもできます。

[eCatalog 画像マップの作成 ](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps) を参照してください。

[ 画像マップを使用して eCatalog にリッチメディアを埋め込む ](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog) を参照してください。

eCatalog 画面の情報パネル設定を使用して、画像マップのテキストを設定および管理できます。

[eCatalog の情報パネルコンテンツの管理 ](/help/using/info-panel-content-ecatalog.md) を参照してください。

## &#x200B;4. eCatalog ビューアプリセットの設定

エンドユーザは eCatalog ビューアで eCatalog を表示します。管理者には eCatalog ビューアを設定する権限があります。アウトラインの色を変更し、新しい「スキン」を選択して eCatalog をブランディングできます。 Adobe Dynamic Media Classicには、いくつかの「ベストプラクティス」 eCatalog ビューアプリセットが付属しています。 eCatalog を表示するためのプリセットを 1 つ選択できます。 管理者であれば、独自の eCatalog ビューアプリセットを作成することもできます。

eCatalog ビューアプリセットを作成するには、グローバルナビゲーションバーで **[!UICONTROL 設定]**/「**[!UICONTROL ビューアプリセット]** の順に選択します。 **[!UICONTROL 追加]** を選択し、プラットフォームを選択して、**[!UICONTROL eCatalog]**/**[!UICONTROL ビューア]** を選択します。

[eCatalog ビューアプリセットの設定 ](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets) を参照してください。

## &#x200B;5. eCatalog ビューアでの eCatalog のプレビュー

eCatalog ビューアのスタイルと動作は、eCatalog ビューアプリセットによって設定されます。

eCatalog ビューアプリセットで eCatalog がどのように表示されるかを確認するには、参照パネルで eCatalog を選択して **[!UICONTROL プレビュー]** を選択します。 初期設定のビューアが開き、プレビュー画面が表示されます。

向き、カラースキーム、ページ変更のコントロール、ページをめくったときの見た目を確認します。

[eCatalog ビューアでの eCatalog のプレビュー ](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer) を参照してください。

## &#x200B;6. eCatalog と関連 PDF の公開

eCatalog および関連するPDFを公開すると、Web サイトやアプリケーションに配信できるように、Dynamic Media Image Server に公開されます。 公開プロセスの一環として、Adobe Dynamic Media Classicは eCatalog の URL 文字列をアクティベートします。 この URL を使用して、Dynamic Media Image Server から Web サイトまたはアプリケーションに eCatalog を呼び出します。

参照パネルで eCatalog とPDFを公開用にマークした後、グローバルナビゲーションバーの「公開」ボタンを選択して公開を開始します。 公開ページで、「**[!UICONTROL 公開を送信]**」を選択します。

[eCatalog と関連 PDF の公開 ](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs) を参照してください。

## &#x200B;7. web ページへの eCatalog のリンク

Adobe Dynamic Media Classicは、Dynamic Media Image Server に公開する際、eCatalog を表示するために必要な URL コールアウト文字列をアクティブ化します。 （詳細表示の） プレビュー画面と参照パネルで URL を選択すると、この URL 文字列をコピーできます。 URL 文字列をコピーすると、web サイトやアプリケーションで使用できます。

IT チームと協力して、web ページの適切な場所に eCatalog へのリンクを配置します。 ユーザーがリンクを選択すると、eCatalog ビューアが表示され、ユーザーは eCatalog を参照できます。

[Web ページへの eCatalog のリンク ](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page) を参照してください。
