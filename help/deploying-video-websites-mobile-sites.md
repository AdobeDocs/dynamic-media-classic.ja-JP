---
title: Web サイトやモバイルサイトへのビデオの配信
description: AdobeDynamic Media ClassicからWebサイトやモバイルサイトにビデオをデプロイする方法を説明します。
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '1704'
ht-degree: 34%

---

# Web サイトやモバイルサイトへのビデオの配信{#deploying-video-to-your-websites-and-mobile-sites}

Webサイト、モバイルサイト、デスクトップアプリケーションは、URL文字列または埋め込みコードを使用して、ビデオを含むAdobeDynamic Media Classicサーバーコンテンツにアクセスします。 AdobeDynamic Media Classicは、公開プロセス中にこれらのURL文字列をアクティブ化します。 Webページ、モバイルページ、デスクトップアプリケーションにビデオのURL文字列または埋め込みコードを配置するには、AdobeDynamic Media Classicからコピーします。

>[!NOTE]
>
>URL または埋め込みコードは、アセットを公開するまでアクティブになりません。

## ビデオの公開 {#publishing-video}

ビデオを公開すると、AdobeDynamic Media Classic ServerはビデオをWebサイト、モバイルサイトまたはアプリケーションに配信できます。

ビデオの公開に使用できる方法は次の 2 つあります。

* **アップロード時にビデオを自動的に即時公開する**  — ビデオのアップロードプロセスの一環として、AdobeDynamic Media Classicは、ビデオをアップロードしてエンコードする際に、自動的に公開できます。 この即時公開機能があることで、アップロードとエンコード後にビデオを個別に公開する必要がありません。

* **アップロード後にビデオを手動で公開する**  — ビデオをすぐに公開しない場合は、いつでも手動でビデオを公開できます。

ビデオを公開すると、AdobeDynamic Media ClassicはHTMLページまたはアプリケーションコードのURL文字列をアクティベートします。

**ビデオを公開するには:**

1. 次のいずれかの操作を行います。

   * アップロード時にビデオを自動的かつ即座に公開するには、アップロードページで「**[!UICONTROL アップロード後に公開]**」を選択します。 完了後は、それ以上の手順は必要ありません。
   * アップロード後にビデオを手動で公開するには、参照パネルでビデオを選択し、グローバルナビゲーションバーで「**公開**」を選択します。

## ビデオURLをモバイルサイトまたはWebサイトにリンクする {#linking-a-video-url-to-a-mobile-site-or-a-website}

ビデオの公開後、そのビデオの URL を取得して Web サイト、モバイルサイトまたはデスクトップアプリケーションで使用できます。このビデオ URL は、Web ページの上のポップアップウィンドウかモーダルウィンドウでビデオを再生する場合に使用します。

顧客がリンクを選択すると、そのデバイス、帯域幅、画面サイズが自動的に検出されます。 デスクトップの場合は、定義済みビューアでの再生に適したビデオが表示され、スマートフォンおよびタブレットの場合は、携帯端末のネイティブビデオプレーヤーでの再生に適したビデオが表示されます。

[Webページへのビデオビューアの埋め込み](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page)も参照してください。

**ビデオ URL をモバイルサイトまたは Web サイトにリンクするには:**

1. アセットの参照パネルの&#x200B;**[!UICONTROL 表示]**&#x200B;ドロップダウンリストで、「**[!UICONTROL ビデオ]**」または「**[!UICONTROL アダプティブビデオセット]**」を選択します。
1. 左側のアセットライブラリパネルで、リンクするビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 「**[!UICONTROL グリッドビュー]**」または「**[!UICONTROL リストビュー]**」を選択します。 アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。右側のURLと埋め込みコードパネルの「HTTPストリーミング」で、目的のビューアの右側にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video`ビューアに関連付けられたURLをコピーします。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の下にある「**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]**」に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL &#x200B;ベストプラクティスとして、`Universal_HTML5_Video`ビューアに関連付けられたURLをコピーします。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の右側にある&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL &#x200B;ベストプラクティスとして、`Universal_HTML5_Video`ビューアに関連付けられたURLをコピーします。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細ビュー]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** /**[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL &#x200B;ベストプラクティスとして、`Universal_HTML5_Video`ビューアに関連付けられたURLをコピーします。

1. HTML5 ビデオ URL のリンクを Web サイトおよびモバイルサイトに貼り付けます。

## Webページにビデオビューアを埋め込む {#embedding-the-video-viewer-on-a-web-page}

Web ページにビデオを埋め込んで再生したい場合は、「埋め込みコード」機能を使用します。埋め込みコードをクリップボードにコピーして、Web ページに貼り付けることができます。埋め込みコードダイアログボックスでは、コードの編集はできません。

[ビデオURLをモバイルサイトまたはWebサイトにリンクする](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)も参照してください。

**Web ページにビデオビューアを埋め込むには:**

1. アセットの参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL ビデオ]**」または「**[!UICONTROL アダプティブビデオセット]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーしたいビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 「**[!UICONTROL グリッドビュー]**」または「**[!UICONTROL リストビュー]**」を選択します。 アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。右側のURLと埋め込みコードパネルの「HTTPストリーミング」で、必要なビューアの右側にある「**[!UICONTROL 埋め込みコード]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video`ビューアに関連付けられている「**[!UICONTROL 埋め込みコード]**」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、ビデオサムネール画像の下で&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;を選択します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video`ビューアに関連付けられている「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の右側にある&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video`ビューアに関連付けられている「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細ビュー]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** /**[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video`ビューアに関連付けられている「**[!UICONTROL 埋め込みコード]**」を選択します。

1. 埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. **[!UICONTROL 閉じる]**&#x200B;を選択します。
1. 埋め込みコードを Web ページに貼り付けます。

### MP4ビデオアセットでHTML5ビデオを使用するための埋め込みコードの実装 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Dynamic Media Classic HTML5ビデオAdobeを使用せず、MP4ビデオアセットでネイティブのHTML5 `<video>`タグを使用する場合は、次の埋め込みコードのサンプルを使用できます。

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* `"S7 video thumbnail URL"`をビデオのサムネールURLに置き換えます。このURLは、ユーザーがビデオを再生する前に確認するビデオのサムネール画像です。

   [ビデオサムネールのURL](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls)の取得を参照してください。

* `"S7 OGG video asset URL (no player)"`をOGGビデオのプログレッシブURLに置き換えます。

   [ビデオURLをモバイルサイトまたはWebサイトにリンクする](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)を参照してください。

* `"S7 MP4 mobile progressive video asset URL (no player)"`をビデオのモバイルプログレッシブURLに置き換えます。

   [ビデオURLをモバイルサイトまたはWebサイトにリンクする](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)を参照してください。

## サードパーティのビデオプレーヤーを使用したビデオのデプロイ {#deploying-video-using-a-third-party-video-player}

AdobeのDynamic Media Classicビデオビューアの代わりにサードパーティのビデオプレーヤーまたはカスタムビルドビデオプレーヤーを使用している場合、HLSマルチビットレートビデオストリーミングまたはプログレッシブダウンロードで機能する直接ビデオURLを取得します。

**サードパーティのビデオプレーヤーを使用してビデオを配信するには:**

1. AdobeDynamic Media Classicで、グローバルナビゲーションバーの&#x200B;**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL 一般設定]**&#x200B;に移動します。
1. 使用する URL のタイプに応じて、次のいずれかの操作を行います。

* 直接HLSストリーミングビデオURL（マルチビットレート）を生成するには

   **[!UICONTROL アプリケーションの一般設定]**&#x200B;ページの&#x200B;**[!UICONTROL サーバー]**&#x200B;グループの「**[!UICONTROL 公開先サーバー名]**」テキストフィールドで、ダイレクトURLを作成します。 次の構文を使用します。`server/is/content/company/folder/filename.m3u8`

   例えば、公開先サーバー名が`https://s7d9.scene7.com/.`であるとします。手順2の構文を使用すると、ダイレクトURLは次のようになります。
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* 直接HLSストリーミングビデオURL（シングルビットレート）を生成するには

   **[!UICONTROL アプリケーションの一般設定]**&#x200B;ページの&#x200B;**[!UICONTROL Servers]**&#x200B;グループの&#x200B;**[!UICONTROL HLS Streaming Server Name]**&#x200B;テキストフィールドで、次の構文を使用して直接URLを作成します。

   `server/company/folder/filename.ext.m3u8`

   例えば、HLSストリーミングサーバ名が`https://s7mbrstream.scene7.com/hls-vod/`であるとします。 手順2の構文を使用して、ダイレクトURLは次のようになります。
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* プログレッシブビデオのダイレクト URL を生成するには

   **[!UICONTROL アプリケーションの全般設定]**&#x200B;ページの「**[!UICONTROL サーバー]**」グループの「**[!UICONTROL プログレッシブビデオサーバー名]**」テキストフィールドで、次の構文を使用して eVideo のダイレクト URL を作成します。

   `server/company/folder/filename`

   例えば、プログレッシブビデオサーバ名が`https://s7d9.scene7.com/is/content/`であるとします。 手順2の構文を使用して、ダイレクトURLは次のようになります。
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## ビデオサムネールの操作 {#working-with-video-thumbnails}

AdobeDynamic Media Classicは、エンコードされたビデオおよび事前にエンコードされたビデオのサムネールを生成します。 ビデオサムネールは、画像アセットと同じように使用できます。さらに、Dynamic Media Classicが生成し、AdobeDynamic Media Classic以外でデプロイするビデオサムネールのURLを取得できます。 例えば、Web サイト上の検索結果、関連するビデオリスト、ビデオ再生リストにサムネールを配信できます。

ビデオの最初の不均一のフレーム（真っ黒でないフレーム、真っ白でないフレームなど）に基づきサムネールが生成されます。

### ビデオサムネールのURLの取得 {#obtaining-video-thumbnail-urls}

AdobeDynamic Media Classicは、アップロードプロセス中にビデオサムネールを自動的に生成します。 サムネールは、リスト表示とグリッド表示の参照パネルに表示されます。

ビデオサムネールの URL を生成するには、公開操作を実行します。

[ビデオの公開](deploying-video-websites-mobile-sites.md#publishing_video)を参照してください。

公開後、URL および埋め込みコードパネルの詳細ビューでビデオサムネールの URL を取得できます。ビデオサムネールの右側にある「**[!UICONTROL URLをコピー]**」を選択して、URLをコピーできます。

### ビデオビューアでのポスターフレームの変更 {#modifying-poster-frames-in-video-viewers}

*ポスターフレーム*&#x200B;は、ビデオの再生開始前にビデオビューアに表示される最初のフレームです。AdobeDynamic Media Classicは、ビデオサムネールをポスターフレームとして使用します。

ポスターフレームに画像修飾子を適用できます。例えば、ポスターフレームを切り抜いたり、透明にしたりすることができます。ポスターフレームを変更するには、ビデオビューアの設定画面を開いて、「ポスター画像修飾子」セクションに修飾子を入力します。

[ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)を参照してください。

[画像サービングガイド](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home.html?lang=en#image-serving-api)を参照してください。

また、ビデオサムネールの URL に修飾子を追加して、ビデオサムネールを変更することもできます。

>[!MORELIKETHIS]
>
>* [ファイルの公開](publishing-files.md#publishing_files)