---
title: Web サイトやモバイルサイトへのビデオの配信
description: Adobe Dynamic Media Classicからweb サイトとモバイルサイトにビデオをデプロイする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:45:00.273Z'
TQID: 'https://experienceleague.adobe.com/lVQWshcgF66zFJ9pTVdrMaGNowclV5u6nxzqOSetns0'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 1735
ht-degree: 22%

---

# Web サイトやモバイルサイトへのビデオの配信{#deploying-video-to-your-websites-and-mobile-sites}

web サイト、モバイルサイト、デスクトップアプリケーションは、URL文字列や埋め込みコードを使用して、ビデオを含むAdobe Dynamic Media Classicサーバーコンテンツにアクセスできます。 Adobe Dynamic Media Classicは、公開プロセス中にこれらのURL文字列をアクティベートします。 Web ページ、モバイルページ、デスクトップアプリケーションにビデオのURL文字列または埋め込みコードを配置するには、Adobe Dynamic Media Classicからビデオをコピーします。

>[!NOTE]
>
>URLまたは埋め込みコードは、アセットを公開するまでアクティブになりません。

## ビデオの公開 {#publishing-video}

ビデオを公開すると、Adobe Dynamic Media Classic Serverがweb サイト、モバイルサイト、またはアプリケーションにビデオを配信できるようになります。

ビデオの公開に使用できる方法は2つあります。

* **アップロード時にビデオを自動的かつ即座に公開する**：ビデオのアップロードプロセスの一環として、Adobe Dynamic Media Classicはビデオのアップロードとエンコード時にビデオを自動的に公開できます。 このインスタントパブリッシング機能により、事後別にビデオを公開する必要がなくなります。

* **アップロード後にビデオを手動で公開**：ビデオをすぐに公開しない場合は、いつでも手動でビデオを公開できます。

ビデオを公開すると、Adobe Dynamic Media ClassicはHTML ページまたはアプリケーションコードのURL文字列をアクティベートします。

**ビデオを公開するには：**

1. 次のいずれかの操作を行います。

   * アップロード時にビデオを自動的かつ即座に公開するには、アップロードページで「**[!UICONTROL アップロード後に公開」を選択します]**。 完了後は、それ以上の手順は必要ありません。
   * アップロード後にビデオを手動で公開するには、参照パネルでビデオを選択し、グローバルナビゲーションバーで「**公開**」を選択します。

## モバイルサイトまたはweb サイトへのビデオ URLのリンク {#linking-a-video-url-to-a-mobile-site-or-a-website}

ビデオを公開する際に、web サイト、モバイルサイト、またはデスクトップアプリケーションで使用するための関連URLを取得できます。 Web ページの上にポップアップウィンドウまたはモーダルウィンドウでビデオを表示する場合は、ビデオ URLを使用します。

顧客がリンクを選択すると、デバイス、帯域幅、画面サイズが自動的に検出されます。 デスクトップの場合は、定義済みビューアでの再生に適したビデオが表示され、スマートフォンおよびタブレットの場合は、携帯端末のネイティブビデオプレーヤーでの再生に適したビデオが表示されます。

[Web ページへのビデオビューアの埋め込み](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page)も参照してください。

**モバイルサイトまたはweb サイトにビデオ URLをリンクするには：**

1. アセット参照パネルの&#x200B;**[!UICONTROL 表示]** ドロップダウンリストで、**[!UICONTROL ビデオ]**&#x200B;または&#x200B;**[!UICONTROL アダプティブビデオセット]**&#x200B;を選択します。
1. 左側のアセットライブラリパネルで、リンクするビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;または&#x200B;**[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。 右側の「URLと埋め込みコード」パネルの「HTTP ストリーミング」で、必要なビューアの右側にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video` ビューアに関連付けられているURLをコピーします。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video` ビューアに関連付けられているURLをコピーします。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video` ビューアに関連付けられているURLをコピーします。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video` ビューアに関連付けられているURLをコピーします。

1. HTML5 ビデオ URL のリンクを Web サイトおよびモバイルサイトに貼り付けます。

## Web ページにビデオビューアを追加する {#embedding-the-video-viewer-on-a-web-page}

Web ページに埋め込まれたビデオを再生する場合は、埋め込みコード機能を使用します。 埋め込まれたコードをクリップボードにコピーして、Web ページに貼り付けることができます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

[&#x200B; モバイルサイトまたはweb サイトへのビデオ URLのリンク &#x200B;](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)も参照してください。

**Web ページにビデオビューアーを埋め込むには：**

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL ビデオ]**」または「**[!UICONTROL アダプティブビデオセット]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーするビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;または&#x200B;**[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。 右側の「URLと埋め込みコード」パネルの「HTTP ストリーミング」で、必要なビューアの右側にある「**[!UICONTROL 埋め込みコード]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video` ビューアに関連付けられている&#x200B;**[!UICONTROL 埋め込みコード]**&#x200B;を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、ビデオサムネール画像の下にある「**[!UICONTROL プレビュー]**」 > 「**[!UICONTROL ビューアーリスト]**」を選択します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video` ビューアに関連付けられている&#x200B;**[!UICONTROL 埋め込みコード]**&#x200B;を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video` ビューアに関連付けられている&#x200B;**[!UICONTROL 埋め込みコード]**&#x200B;を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。 ベストプラクティスとして、`Universal_HTML5_Video` ビューアに関連付けられている&#x200B;**[!UICONTROL 埋め込みコード]**&#x200B;を選択します。

1. 埋め込みコードダイアログボックスで、**[!UICONTROL クリップボードにコピー]**&#x200B;を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. **[!UICONTROL 閉じる]**&#x200B;を選択します。
1. Web ページに埋め込まれたコードを貼り付けます。

### MP4 ビデオアセットでHTML5 ビデオを使用するための埋め込みコードの実装 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Adobe Dynamic Media Classic HTML5 ビデオプレーヤーを使用しない場合があります。 代わりに、ネイティブのHTML5 `<video>` タグをMP4 ビデオアセットで使用する場合は、次の埋め込みコードサンプルを使用できます。

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* `"S7 video thumbnail URL"`を、ユーザーがビデオを再生する前に表示されるビデオのサムネール画像であるビデオのサムネール URLに置き換えます。

  [&#x200B; ビデオサムネール URLの取得](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls)を参照してください。

* `"S7 OGG video asset URL (no player)"`をOGG ビデオのビデオのプログレッシブ URLに置き換えます。

  [&#x200B; モバイルサイトまたはweb サイトへのビデオ URLのリンク &#x200B;](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)を参照してください。

* `"S7 MP4 mobile progressive video asset URL (no player)"`をビデオのモバイル プログレッシブ URLに置き換えます。

  [&#x200B; モバイルサイトまたはweb サイトへのビデオ URLのリンク &#x200B;](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)を参照してください。

## サードパーティのビデオプレーヤーを使用してビデオをデプロイ {#deploying-video-using-a-third-party-video-player}

Dynamic Media Classic ビデオビューアの代わりにサードパーティ製のビデオプレーヤーまたはカスタムビルドのビデオプレーヤーを使用する場合は、HLS マルチビットレートのビデオストリーミングまたはプログレッシブダウンロードに使用できるダイレクトビデオ URLを取得します。

**サードパーティのビデオ プレーヤーを使用してビデオをデプロイするには：**

1. Adobe Dynamic Media Classicのグローバルナビゲーションバーで、**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**&#x200B;に移動します。
1. 使用する URL のタイプに応じて、次のいずれかの操作を行います。

* ダイレクト HLS ストリーミングビデオ URL （マルチビットレート）を生成するには

  **[!UICONTROL アプリケーション一般設定]** ページの&#x200B;**[!UICONTROL サーバー]** グループの&#x200B;**[!UICONTROL 公開サーバー名]** テキストフィールドで、直接URLを作成します。 次の構文を使用します：`server/is/content/company/folder/filename.m3u8`

  例えば、公開済みサーバー名が`https://s7d9.scene7.com/.`であるとします。手順2の構文を使用すると、ダイレクト URLは次のようになります。
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* HLSのストリーミングビデオのダイレクト URL （シングルビットレート）を生成するには

  **[!UICONTROL Application General Settings]** ページの&#x200B;**[!UICONTROL Servers]** グループの&#x200B;**[!UICONTROL HLS Streaming Server Name]** テキストフィールドで、次の構文を使用してダイレクト URLを作成します。

  `server/company/folder/filename.ext.m3u8`

  例えば、HLS ストリーミングサーバー名が`https://s7mbrstream.scene7.com/hls-vod/`であるとします。 手順2の構文を使用すると、ダイレクト URLは次のようになります。
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* プログレッシブビデオのダイレクト URL を生成するには

  **[!UICONTROL アプリケーションの全般設定]**&#x200B;ページの「**[!UICONTROL サーバー]**」グループの「**[!UICONTROL プログレッシブビデオサーバー名]**」テキストフィールドで、次の構文を使用して eVideo のダイレクト URL を作成します。

  `server/company/folder/filename`

  例えば、プログレッシブビデオサーバー名が`https://s7d9.scene7.com/is/content/`であるとします。 手順2の構文を使用すると、ダイレクト URLは次のようになります。
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## ビデオサムネールの操作 {#working-with-video-thumbnails}

Adobe Dynamic Media Classicは、エンコードされたビデオと事前にエンコードされたビデオのサムネールを生成します。 ビデオサムネールは、画像アセットと同じように使用できます。 さらに、Adobe Dynamic Media Classicが生成するビデオサムネールのURLを取得することもできます。 次に、これらのURLをAdobe Dynamic Media Classicの外部にデプロイします。 例えば、Web サイト上の検索結果、関連するビデオリスト、ビデオ再生リストにサムネールを配信できます。

ビデオの最初の不均一のフレーム（真っ黒でないフレーム、真っ白でないフレームなど）に基づきサムネールが生成されます。

### ビデオサムネール URLの取得 {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classicは、アップロードプロセス中に自動的にビデオサムネールを生成します。 サムネールは、リストビューとグリッドビューの参照パネルに表示されます。

ビデオサムネールの URL を生成するには、公開操作を実行します。

[&#x200B; ビデオの公開](deploying-video-websites-mobile-sites.md#publishing_video)を参照してください。

公開後、URL および埋め込みコードパネルの詳細ビューでビデオサムネールの URL を取得できます。 ビデオサムネールの右側にある「**[!UICONTROL URLをコピー]**」を選択すると、関連するURLをコピーできます。

### ビデオビューアでのポスターフレームの変更 {#modifying-poster-frames-in-video-viewers}

*ポスターフレーム*&#x200B;は、ビデオの再生開始前にビデオビューアに表示される最初のフレームです。 Adobe Dynamic Media Classicでは、ビデオのサムネールをポスターフレームとして使用します。

ポスターフレームに画像修飾子を適用できます。 例えば、ポスターフレームを切り抜いたり、透明にしたりすることができます。 ポスターフレームを変更するには、ビデオビューアの設定画面を開いて、「ポスター画像修飾子」セクションに修飾子を入力します。

[&#x200B; ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)を参照してください。

[画像サービングガイド &#x200B;](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home#image-serving-api)を参照してください。

また、ビデオサムネールの URL に修飾子を追加して、ビデオサムネールを変更することもできます。

>[!MORELIKETHIS]
>
>* [&#x200B; ファイルを公開](publishing-files.md#publishing_files)