---
title: Web サイトやモバイルサイトへのビデオの配信
description: Adobe Dynamic Media Classicから Web サイトやモバイルサイトにビデオをデプロイする方法を説明します。
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '1706'
ht-degree: 33%

---

# Web サイトやモバイルサイトへのビデオの配信{#deploying-video-to-your-websites-and-mobile-sites}

Web サイト、モバイルサイト、デスクトップアプリケーションは、URL 文字列または埋め込みコードを使用して、ビデオなどのAdobe Dynamic Media Classicサーバーコンテンツにアクセスします。 Adobe Dynamic Media Classicは、公開プロセス中にこれらの URL 文字列をアクティベートします。 Web ページ、モバイルページおよびデスクトップアプリケーションにビデオの URL 文字列または埋め込みコードを配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL または埋め込みコードは、アセットを公開するまでアクティブになりません。

## ビデオの公開 {#publishing-video}

ビデオを公開すると、Adobe Dynamic Media Classic Servers はビデオを Web サイト、モバイルサイトまたはアプリケーションに配信できます。

ビデオの公開に使用できる方法は 2 つあります。

* **アップロード時にビデオを自動的かつ即時に公開**  — ビデオのアップロードプロセスの一環として、Adobe Dynamic Media Classicは、ビデオがアップロードされエンコードされる際に、自動的に公開できます。 この即時公開機能があることで、アップロードとエンコード後にビデオを個別に公開する必要がありません。

* **アップロード後にビデオを手動で公開する**  — ビデオをすぐに公開したくない場合は、いつでも手動でビデオを公開できます。

ビデオを公開すると、Adobe Dynamic Media Classicは、HTMLのページまたはアプリケーションコードの URL 文字列をアクティベートします。

**ビデオを公開するには:**

1. 次のいずれかの操作を行います。

   * アップロード時にビデオを自動的かつ即時に公開するには、アップロードページで **[!UICONTROL アップロード後に公開]**. 完了後は、それ以上の手順は必要ありません。
   * アップロード後にビデオを手動で公開するには、参照パネルでビデオを選択し、グローバルナビゲーションバーで **公開**.

## ビデオ URL をモバイルサイトまたは Web サイトにリンクする {#linking-a-video-url-to-a-mobile-site-or-a-website}

ビデオの公開後、そのビデオの URL を取得して Web サイト、モバイルサイトまたはデスクトップアプリケーションで使用できます。このビデオ URL は、Web ページの上のポップアップウィンドウかモーダルウィンドウでビデオを再生する場合に使用します。

顧客がリンクを選択すると、デバイス、帯域幅、画面サイズが自動的に検出されます。 デスクトップの場合は、定義済みビューアでの再生に適したビデオが表示され、スマートフォンおよびタブレットの場合は、携帯端末のネイティブビデオプレーヤーでの再生に適したビデオが表示されます。

関連トピック [Web ページにビデオビューアを埋め込む](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**ビデオ URL をモバイルサイトまたは Web サイトにリンクするには:**

1. アセット参照パネルで、 **[!UICONTROL 表示]** ドロップダウンリストで、「 **[!UICONTROL ビデオ]** または **[!UICONTROL アダプティブビデオセット]**.
1. 左側のアセットライブラリパネルで、リンクするビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]** または **[!UICONTROL リスト表示]**. アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。右側の URL と埋め込みコードパネルの「HTTP ストリーミング」で、「 **[!UICONTROL URL をコピー]** を選択します。 ベストプラクティスとして、 `Universal_HTML5_Video` 閲覧者
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**. ベストプラクティスとして、 `Universal_HTML5_Video` 閲覧者

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**. ベストプラクティスとして、 `Universal_HTML5_Video` 閲覧者

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**. ベストプラクティスとして、 `Universal_HTML5_Video` 閲覧者

1. HTML5 ビデオ URL のリンクを Web サイトおよびモバイルサイトに貼り付けます。

## Web ページにビデオビューアを埋め込む {#embedding-the-video-viewer-on-a-web-page}

Web ページにビデオを埋め込んで再生したい場合は、「埋め込みコード」機能を使用します。埋め込みコードをクリップボードにコピーして、Web ページに貼り付けることができます。埋め込みコードダイアログボックスでは、コードを編集することはできません。

関連トピック [ビデオ URL をモバイルサイトまたは Web サイトにリンクする](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**Web ページにビデオビューアを埋め込むには:**

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL ビデオ]** または **[!UICONTROL アダプティブビデオセット]**.
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーしたいビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]** または **[!UICONTROL リスト表示]**. アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。右側の URL と埋め込みコードパネルの「HTTP ストリーミング」で、「 **[!UICONTROL 埋め込みコード]** を選択します。 ベストプラクティスとして、「 」を選択します。 **[!UICONTROL 埋め込みコード]** が `Universal_HTML5_Video` 閲覧者
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで 1 つのアセットを選択し、ビデオサムネール画像の下でを選択します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**. ベストプラクティスとして、「 」を選択します。 **[!UICONTROL 埋め込みコード]** が `Universal_HTML5_Video` 閲覧者

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**. ベストプラクティスとして、「 」を選択します。 **[!UICONTROL 埋め込みコード]** が `Universal_HTML5_Video` 閲覧者

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**. ベストプラクティスとして、「 」を選択します。 **[!UICONTROL 埋め込みコード]** が `Universal_HTML5_Video` 閲覧者

1. 埋め込みコードダイアログボックスで、「 **[!UICONTROL クリップボードにコピー]**.

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. 選択 **[!UICONTROL 閉じる]**.
1. 埋め込みコードを Web ページに貼り付けます。

### MP4 ビデオアセットでHTML5 ビデオを使用するための埋め込みコードの実装 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Adobe Dynamic Media Classic Player を使用せずに、ネイティブのHTML5 を使用したい場合。 `<video>` タグに MP4 ビデオアセットを追加すると、次の埋め込みコードのサンプルを使用できます。

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* 置換 `"S7 video thumbnail URL"` ビデオのサムネール URL（ユーザーがビデオを再生する前に確認するビデオのサムネール画像）が表示されます。

  詳しくは、 [ビデオサムネールの URL の取得](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* 置換 `"S7 OGG video asset URL (no player)"` に含まれます。

  詳しくは、 [ビデオ URL をモバイルサイトまたは Web サイトにリンクする](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* 置換 `"S7 MP4 mobile progressive video asset URL (no player)"` に含まれるビデオのモバイルプログレッシブ URL を入力します。

  詳しくは、 [ビデオ URL をモバイルサイトまたは Web サイトにリンクする](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## サードパーティのビデオプレーヤーを使用してビデオをデプロイする {#deploying-video-using-a-third-party-video-player}

Dynamic Media Classicビデオビューアの代わりにサードパーティのビデオプレーヤーまたはカスタム構築のビデオプレーヤーを使用する場合、HLS マルチビットレートビデオストリーミングまたはプログレッシブダウンロードで機能する直接ビデオ URL を取得します。

**サードパーティのビデオプレーヤーを使用してビデオを配信するには:**

1. Adobe Dynamic Media Classicのグローバルナビゲーションバーで、 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 一般設定]**.
1. 使用する URL のタイプに応じて、次のいずれかの操作を行います。

* 直接 HLS ストリーミングビデオ URL（マルチビットレート）を生成するには

  の **[!UICONTROL アプリケーションの一般設定]** ページの **[!UICONTROL サーバー]** グループ、 **[!UICONTROL 公開先サーバー名]** テキストフィールドで、ダイレクト URL を作成します。 次の構文を使用します。 `server/is/content/company/folder/filename.m3u8`

  例えば、公開先サーバー名が `https://s7d9.scene7.com/.` 手順 2 の構文を使用すると、ダイレクト URL は次のようになります。
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 直接 HLS ストリーミングビデオの URL（シングルビットレート）を生成するには

  の **[!UICONTROL アプリケーションの一般設定]** ページの **[!UICONTROL サーバー]** グループ、 **[!UICONTROL HLS ストリーミングサーバ名]** テキストフィールドで、次の構文を使用してダイレクト URL を作成します。

  `server/company/folder/filename.ext.m3u8`

  例えば、HLS ストリーミングサーバー名が `https://s7mbrstream.scene7.com/hls-vod/`. 手順 2 の構文を使用すると、ダイレクト URL は次のようになります。
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* プログレッシブビデオのダイレクト URL を生成するには

  **[!UICONTROL アプリケーションの全般設定]**&#x200B;ページの「**[!UICONTROL サーバー]**」グループの「**[!UICONTROL プログレッシブビデオサーバー名]**」テキストフィールドで、次の構文を使用して eVideo のダイレクト URL を作成します。

  `server/company/folder/filename`

  例えば、プログレッシブビデオサーバ名が `https://s7d9.scene7.com/is/content/`. 手順 2 の構文を使用すると、ダイレクト URL は次のようになります。
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## ビデオサムネールの操作 {#working-with-video-thumbnails}

Adobe Dynamic Media Classicは、エンコードされたビデオと、事前にエンコードされたビデオのサムネールを生成します。 ビデオサムネールは、画像アセットと同じように使用できます。さらに、Adobe Dynamic Media Classicが生成するビデオサムネールの URL を取得できます。 その後、これらの URL をAdobe Dynamic Media Classicの外部にデプロイできます。 例えば、Web サイト上の検索結果、関連するビデオリスト、ビデオ再生リストにサムネールを配信できます。

ビデオの最初の不均一のフレーム（真っ黒でないフレーム、真っ白でないフレームなど）に基づきサムネールが生成されます。

### ビデオサムネールの URL の取得 {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classicは、アップロードプロセス中にビデオサムネールを自動的に生成します。 サムネールは、リスト表示とグリッド表示の参照パネルに表示されます。

ビデオサムネールの URL を生成するには、公開操作を実行します。

詳しくは、 [ビデオを公開](deploying-video-websites-mobile-sites.md#publishing_video).

公開後、URL および埋め込みコードパネルの詳細ビューでビデオサムネールの URL を取得できます。選択 **[!UICONTROL URL をコピー]** をクリックして、ビデオのサムネールの右側に表示されます。

### ビデオビューアでのポスターフレームの変更 {#modifying-poster-frames-in-video-viewers}

*ポスターフレーム*&#x200B;は、ビデオの再生開始前にビデオビューアに表示される最初のフレームです。Adobe Dynamic Media Classicは、ビデオサムネールをポスターフレームとして使用します。

ポスターフレームに画像修飾子を適用できます。例えば、ポスターフレームを切り抜いたり、透明にしたりすることができます。ポスターフレームを変更するには、ビデオビューアの設定画面を開いて、「ポスター画像修飾子」セクションに修飾子を入力します。

詳しくは、 [ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

詳しくは、 [画像サービングガイド](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api).

また、ビデオサムネールの URL に修飾子を追加して、ビデオサムネールを変更することもできます。

>[!MORELIKETHIS]
>
>* [ファイルを公開](publishing-files.md#publishing_files)