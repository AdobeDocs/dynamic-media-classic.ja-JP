---
title: クイックスタート：eCatalogs
description: Adobe Dynamic Media ClassicのeCatalog テクニックを使用して、すばやく立ち上げて実行するのに役立つ概要とeCatalogのクイックスタート。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 9e2df814-465d-412a-a032-ef3e8cb462ba
topic: Integrations
level: Experienced
autotag-review: '2026-05-13T19:55:49.663Z'
TQID: 'https://experienceleague.adobe.com/EFy8tVdGv5q5mmQQS-m0Mb8AuphJHEDHzspsPWNxMlI'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 1572
ht-degree: 25%

---

# クイックスタート：eCatalogs{#quick-start-ecatalogs}

e カタログとは、web版の印刷物（カタログ、パンフレット、チラシ、製品マニュアル、広告回覧など）です。 eCatalogは、Web サイトのeCatalog Viewerに表示されます。 このビューアを使用すると、印刷物を読むときと同じ感覚で資料を読むことができます。

次のトレーニングビデオも参照してください。

* [ クイックスタート 1: eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/561_Quick%20Start%20-%20Part%201_converted%20renamed_eCatalogs-AVS)
* [ クイックスタート 2: eCatalogs](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/562_Quick%20Start%20-%20Part%202_converted%20renamed_eCatalogs-AVS)

eCatalogで選択した設定に応じて、ビューアで次の操作を実行できます。

* カタログでキーワードまたはキーワードを検索します。 検索結果は、カタログの左側にある検索パネルにサムネールのリストとして表示されます。 クリック可能な各サムネールは、強調表示された検索語句が見つかったカタログのスプレッドを表します。

* ソーシャルメディア経由でカタログを共有する、オフラインで表示するカタログをダウンロードする、お気に入りにすばやく戻すアイテムをマークする、カタログを印刷する、などの方法があります。
* 目次またはページグリッドビューを使用してカタログを移動します。ページの中央のエッジを選択して、ページを前後に移動します。
* ズームイン、ズームアウト、およびパンを実行して、ページの項目を確認することができます。
* ページ領域（画像マップと呼ばれる）の上にポインターを移動すると、アイテムに関する情報を含むポップアップウィンドウが表示されます。
* ページ領域を選択して、項目に関する詳細情報が記載された新しいWeb ページを開きます。
* ノート注釈を書き、eCatalog のページに貼り付けることができます。
* 関連するWeb ページまたはコンテキスト内の情報パネルを起動する場合は、「画像マップ」アイコンをタップします。
* ピンチズームやスワイプによるページめくりなど、ジェスチャ操作を使用します。
* キーワードと一致する項目を検索することができます。

![ ユーザーに表示されるe カタログ。 A） eCatalog開封ページ。 B） eCatalogが2 ページ目になりました。](/help/using/assets/ec_cat_viewer_popup.png)

eCatalogを作成するには、通常、Adobe Acrobatまたは他の印刷プログラムで作成された高解像度のPDF ファイルを使用しますが、画像ファイルからeCatalogを作成することもできます。

eCatalog を作成する際に、ページや見開きページの並び順を選択することができます。 また、見開きページの表示単位を 1 ページにするのか、2 ページにするのか、または任意指定のページ数にするのかを選択することもできます。 ページ領域の画像マップを作成して、例えば、閲覧者がページ上の領域を選択し、Web サイト上で新しいページを開くことができるようにすることができます。 eCatalog 画面内の情報パネル設定を使用して、表示するロールオーバーテキストを管理できます。 eCatalog ビューアを設定する手段として、100 以上の様々な設定オプションが用意されています。 また、閲覧者に合わせて、ビューアの機能や外観を変更することができます。

>[!NOTE]
>
>Dynamic Media: Scene7 モードのユーザーで、eCatalogsを使用する場合は、CRXDE Liteで`pdfbrochure`値を編集します。 これを行うには、Adobe Experience Managerで、**[!UICONTROL ツール]** > **[!UICONTROL 一般]** > **[!UICONTROL CRXDE Lite]**&#x200B;に移動します。 左側のパネルナビゲーションツリーで、`/conf/global/settings/cloudconfigs/dmscene7/jcr:content/mimeTypes/application_pdf`に移動します。
>
>右下のペインの「**[!UICONTROL プロパティ]**」タブで、`jobParam`行を選択します。 `pdfbrochure`の値を`false`から`true`に設定します。 `pdfbrochure=true`と同様
>
>CRXDE Lite ページの左上隅にある「**[!UICONTROL すべて保存]**」を選択します。
>
>Adobe Dynamic Media Classicでe カタログを作成できるようになりました。

ここでは、eCatalog の操作方法をすばやく習得できるように、手順について簡潔に説明します。 手順 1 ～ 7 に従ってください。 各ステップの後、トピック見出しへの相互参照があり、詳細を確認できます。

## &#x200B;1. PDF ファイルのアップロード

eCatalog のもとになるファイルは、ほとんどの場合 Adobe PDF ファイルです。 PDF ファイルは印刷を目的としたファイルなので、通常、CMYK 画像が含まれています。 Adobe Dynamic Media Classicは、これらの画像を検出し、標準のCMYK カラープロファイルを使用して変換します。 ただし、カスタムカラープロファイルをアップロードして使用する必要があります。

グローバルナビゲーションバーで「**[!UICONTROL アップロード]**」を選択して、eCatalog用のPDF ファイルまたは画像のアップロードを開始します。 デスクトップから、またはFTP経由でファイルをアップロードできます。100 MBを超えるファイルやファイルを多数アップロードする場合は、FTPをお勧めします。

「PDF オプション」を選択すると、アップロード画面に、適正な解像度とカラースペースで PDF ファイルをアップロードするためのオプションが表示されます。 解像度の推奨値は 150 pixel/インチです。 PDF ファイルをアップロードするときにeCatalogを作成するには、「**[!UICONTROL eCatalogを自動生成]**」オプションを選択します。

[PDF ファイルのアップロード ](uploading-pdf-files.md#uploading_the_pdf_files)を参照してください。

## &#x200B;2. eCatalogの作成

参照パネルでPDFまたは画像ファイルを選択して、eCatalogを作成します。 **[!UICONTROL ビルド]**&#x200B;を選択してから、**[!UICONTROL eCatalogs]**&#x200B;を選択します。

eCatalog ページの「**[!UICONTROL 注文ページ]**」タブで、「**[!UICONTROL 1 Up]**」、「**[!UICONTROL 2 Up]**」または「**[!UICONTROL Custom]**」のレイアウトオプションを選択します。 ページや見開きページの配置変更は、それらをドラッグすることで行えますが、eCatalog のサイズが大きい場合には、移動先メニューでページ名を選択することでも行えます。

ページを追加するには、アセットライブラリのフォルダを選択してから、PDF ファイルまたは画像ファイルをページ順序画面にドラッグします。 デフォルトのページ番号の代わりに、カスタムページ名を指定したり、多数のページ名をインポートしたりできます。

**[!UICONTROL 保存]**&#x200B;を選択し、eCatalogの名前を入力して、保存するAdobe Dynamic Media Classic フォルダーを選択し、**[!UICONTROL 保存]**&#x200B;を選択します。 ページの順序を変更したり、eCatalogを編集したりするたびに、**[!UICONTROL 保存]**&#x200B;を選択して変更を保存します。

[eCatalogの作成](creating-ecatalog.md)を参照してください。

## &#x200B;3. 画像マップの作成

画像マップは、e カタログページに別の側面を追加します。 画像マップとは、ページの中で、項目に関する詳細情報を表示できる領域を指します。 画像マップにポインタを合わせると、その項目の説明が表示されます。 画像マップをクリックすると、外部参照がアクティブ化され、新しいWeb ページが開き、項目の詳細を確認できます。

画像マップを作成するには、eCatalog 画面を開き、 次に、eCatalog画面の&#x200B;**[!UICONTROL マップページ]** タブに移動し、長方形画像マップツールまたは多角形の画像マップツールを使用してマップをフレーム化します。 パンツールを使用してマップの境界線をドラッグすることで、画像マップの位置とサイズを調整できます。

画像マップをフレーム化した後、画像マップを選択するときに使用するURL アドレスを入力します。 画像マップにポインタを合わせたときに表示するロールオーバーテキストを入力することもできます。

[eCatalog画像マップの作成](creating-ecatalog-image-maps.md#creating-ecatalog-image-maps)を参照してください。

[画像マップを使用してeCatalogにリッチメディアを埋め込む](creating-ecatalog-image-maps.md#embedding-rich-media-in-an-ecatalog)を参照してください。

eCatalog画面の情報パネル設定を使用して、画像マップのテキストを設定および管理できます。

eCatalogs](/help/using/info-panel-content-ecatalog.md)の[情報パネルのコンテンツの管理を参照してください。

## &#x200B;4. eCatalog ビューアプリセットの設定

エンドユーザは eCatalog ビューアで eCatalog を表示します。 管理者には eCatalog ビューアを設定する権限があります。 アウトラインの色を変更し、新しい「スキン」を選択してeCatalogのブランディングを行うことができます。 Adobe Dynamic Media Classicには、いくつかの「ベストプラクティス」のe カタログビューアプリセットが付属しています。 eCatalogsを表示するプリセットの1つを選択できます。 管理者であれば、独自の eCatalog ビューアプリセットを作成することもできます。

eCatalog ビューアプリセットを作成するには、グローバルナビゲーションバーで「**[!UICONTROL 設定]**」を選択し、「**[!UICONTROL ビューアプリセット]**」を選択します。 **[!UICONTROL 追加]**&#x200B;を選択し、プラットフォームを選択してから、**[!UICONTROL eCatalog]** > **[!UICONTROL Viewer]**&#x200B;を選択します。

「[eCatalog ビューアプリセットの設定](setting-ecatalog-viewer-presets.md#setting-up-ecatalog-viewer-presets)」を参照してください。

## &#x200B;5. eCatalog ビューアでのeCatalogのプレビュー

eCatalog ビューアのスタイルと動作は、eCatalog ビューアプリセットによって設定されます。

eCatalog ビューアプリセットでのeCatalogの表示方法を確認するには、参照パネルでeCatalogを選択し、**[!UICONTROL プレビュー]**&#x200B;を選択します。 初期設定のビューアが開き、プレビュー画面が表示されます。

向き、カラースキーム、ページ変更のコントロール、ページをめくったときの見た目を確認します。

eCatalog Viewer](previewing-ecatalogs-ecatalog-viewer.md#previewing-ecatalogs-in-the-ecatalog-viewer)の「[eCatalogのプレビュー」を参照してください。

## &#x200B;6. eCatalogと関連するPDFの公開

eCatalogと関連するPDFを公開すると、Dynamic Media Image Serversに配置され、Web サイトやアプリケーションに配信できるようになります。 公開プロセスの一環として、Adobe Dynamic Media ClassicはeCatalogのURL文字列をアクティベートします。 このURLを使用して、Dynamic Media Image ServerからWeb サイトまたはアプリケーションにeCatalogを呼び出します。

参照パネルでeCatalogとPDFの公開用にマークを付けた後、グローバルナビゲーションバーの「公開」ボタンを選択して公開を開始します。 公開ページで、**[!UICONTROL 公開を送信]**&#x200B;を選択します。

[電子カタログと関連するPDFの公開](publishing-ecatalogs-associated-pdfs.md#publishing-ecatalogs-and-associated-pdfs)を参照してください。

## &#x200B;7. eCatalogをWeb ページにリンクする

Adobe Dynamic Media Classicは、eCatalogをDynamic Media Image Serverに公開するときに、eCatalogの表示に必要なURL コールアウト文字列をアクティブにします。 このURL文字列は、パネルでURLを選択することで、プレビュー画面および参照パネル（詳細表示）からコピーできます。 URL文字列をコピーすると、Web サイトとアプリケーションで使用できるようになります。

IT チームと協力して、eCatalogへのリンクをWeb ページの適切な場所に配置します。 ユーザーがリンクを選択すると、eCatalog Viewerが表示され、ユーザーはeCatalogを参照できます。

「[eCatalogをWeb ページにリンクする](linking-ecatalog-web-page.md#linking-an-ecatalog-to-a-web-page)」を参照してください。
