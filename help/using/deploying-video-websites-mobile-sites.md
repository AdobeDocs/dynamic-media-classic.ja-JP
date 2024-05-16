---
title: Web サイトやモバイルサイトへのビデオの配信
description: Adobe Dynamic Media Classicから web サイトやモバイルサイトにビデオをデプロイする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 3df22d48-edb5-4927-aefb-104b53f81f1a
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 23%

---

# Web サイトやモバイルサイトへのビデオの配信{#deploying-video-to-your-websites-and-mobile-sites}

Web サイト、モバイルサイトおよびデスクトップアプリケーションは、URL 文字列または埋め込みコードを使用して、ビデオを含むAdobe Dynamic Media Classic サーバーコンテンツにアクセスします。 Adobe Dynamic Media Classicは、公開プロセス中にこれらの URL 文字列をアクティベートします。 Web ページ、モバイルページおよびデスクトップアプリケーションにビデオの URL 文字列または埋め込みコードを配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL または埋め込みコードは、アセットを公開するまでアクティブになりません。

## ビデオの公開 {#publishing-video}

ビデオを公開すると、Adobe Dynamic Media Classic サーバーは Web サイト、モバイルサイトまたはアプリケーションにビデオを配信できます。

ビデオの公開に使用できる方法は 2 つあります。

* **アップロード時にビデオを自動的かつ即座に公開**：ビデオのアップロードプロセスの一環として、Adobe Dynamic Media Classicでは、ビデオがアップロードおよびエンコードされる際にビデオを自動的に公開できます。 このインスタントパブリッシング機能により、事後にビデオを個別に公開する必要がなくなります。

* **アップロード後にビデオを手動で公開**：ビデオをすぐに公開しない場合は、いつでも手動で公開できます。

ビデオを公開すると、Adobe Dynamic Media ClassicによってHTMLページまたはアプリケーションコードの URL 文字列がアクティベートされます。

**ビデオを公開するには：**

1. 次のいずれかの操作を行います。

   * アップロード時にビデオを自動的かつ即座に公開するには、アップロードページで「」を選択します **[!UICONTROL アップロード後に公開]**. 完了後は、それ以上の手順は必要ありません。
   * アップロード後にビデオを手動で公開するには、参照パネルでビデオを選択して、グローバルナビゲーションバーでを選択します **公開**.

## ビデオ URL のモバイルサイトまたは web サイトへのリンク {#linking-a-video-url-to-a-mobile-site-or-a-website}

ビデオを公開すると、関連する URL を取得して、web サイト、モバイルサイト、デスクトップアプリケーションで使用できます。 Web ページの上部にあるポップアップウィンドウまたはモーダルウィンドウにビデオを表示する場合は、ビデオ URL を使用します。

顧客がリンクを選択すると、そのデバイス、帯域幅、画面サイズが自動的に検出されます。 デスクトップの場合は、定義済みビューアでの再生に適したビデオが表示され、スマートフォンおよびタブレットの場合は、携帯端末のネイティブビデオプレーヤーでの再生に適したビデオが表示されます。

関連トピック [Web ページへのビデオビューアの埋め込み](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page).

**ビデオ URL をモバイルサイトまたは web サイトにリンクするには：**

1. アセットの参照パネルの **[!UICONTROL 表示]** ドロップダウンリストから「」を選択します **[!UICONTROL ビデオ]**、または **[!UICONTROL アダプティブビデオセット]**.
1. 左側のアセットライブラリパネルで、リンクするビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * を選択 **[!UICONTROL グリッド表示]** または **[!UICONTROL リスト表示]**. アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。右側の URL と埋め込みコード パネルの「HTTP ストリーミング」で、次の項目を選択します **[!UICONTROL URL をコピー]** をビューアの右側にクリックします。 ベストプラクティスとして、に関連付けられた URL をコピーします `Universal_HTML5_Video` ビューア。
   * を選択 **[!UICONTROL グリッド表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の下のに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**. ベストプラクティスとして、に関連付けられた URL をコピーします `Universal_HTML5_Video` ビューア。

   * を選択 **[!UICONTROL リスト表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の右側で、 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**. ベストプラクティスとして、に関連付けられた URL をコピーします `Universal_HTML5_Video` ビューア。

   * を選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**、または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**. ベストプラクティスとして、に関連付けられた URL をコピーします `Universal_HTML5_Video` ビューア。

1. HTML5 ビデオ URL のリンクを Web サイトおよびモバイルサイトに貼り付けます。

## Web ページへのビデオビューアの埋め込み {#embedding-the-video-viewer-on-a-web-page}

Web ページに埋め込んだビデオを再生する場合は、埋め込みコード機能を使用します。 埋め込みコードをクリップボードにコピーして、Web ページに貼り付けることができます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

関連トピック [ビデオ URL のモバイルサイトまたは web サイトへのリンク](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

**ビデオビューアを Web ページに埋め込むには：**

1. アセットの参照パネルの「表示」ドロップダウンリストで、を選択します **[!UICONTROL ビデオ]**、または **[!UICONTROL アダプティブビデオセット]**.
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーするビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * を選択 **[!UICONTROL グリッド表示]** または **[!UICONTROL リスト表示]**. アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。右側の URL と埋め込みコード パネルの「HTTP ストリーミング」で、次の項目を選択します **[!UICONTROL 埋め込みコード]** をビューアの右側にクリックします。 ベストプラクティスとして、を選択します **[!UICONTROL 埋め込みコード]** に関連付けられています `Universal_HTML5_Video` ビューア。
   * を選択 **[!UICONTROL グリッド表示]**. アセット参照パネルで、1 つのアセットを選択し、ビデオサムネール画像の下でを選択します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**. ベストプラクティスとして、を選択します **[!UICONTROL 埋め込みコード]** に関連付けられています `Universal_HTML5_Video` ビューア。

   * を選択 **[!UICONTROL リスト表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の右側で、 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**. ベストプラクティスとして、を選択します **[!UICONTROL 埋め込みコード]** に関連付けられています `Universal_HTML5_Video` ビューア。

   * を選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**、または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**. ベストプラクティスとして、を選択します **[!UICONTROL 埋め込みコード]** に関連付けられています `Universal_HTML5_Video` ビューア。

1. 埋め込みコード ダイアログボックスで、を選択します。 **[!UICONTROL クリップボードにコピー]**.

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. 選択 **[!UICONTROL 閉じる]**.
1. 埋め込みコードを Web ページに貼り付けます。

### MP4 ビデオアセットでHTML 5 ビデオを使用するための埋め込みコードの実装 {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

Adobe Dynamic Media Classic HTML5 ビデオプレーヤーを使用したくない場合があります。 代わりに、ネイティブHTMLを使用する場合は、次のようにします。5 `<video>` mp4 ビデオアセットのタグ付けでは、以下の埋め込みコードサンプルを使用できます。

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* 置換 `"S7 video thumbnail URL"` ビデオのサムネール URL は、ビデオを再生する前にユーザーに表示されるビデオのサムネール画像です。

  参照： [ビデオサムネール URL の取得](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls).

* 置換 `"S7 OGG video asset URL (no player)"` OGG ビデオ用のビデオのプログレッシブ URL を使用します。

  参照： [ビデオ URL のモバイルサイトまたは web サイトへのリンク](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

* 置換 `"S7 MP4 mobile progressive video asset URL (no player)"` ビデオのモバイルプログレッシブ URL を使用します。

  参照： [ビデオ URL のモバイルサイトまたは web サイトへのリンク](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website).

## サードパーティのビデオプレーヤーを使用したビデオのデプロイ {#deploying-video-using-a-third-party-video-player}

Dynamic Media Classic ビデオビューアではなく、サードパーティのビデオプレーヤーまたはカスタム組み込みのビデオプレーヤーを使用する場合は、HLS マルチビットレートのビデオストリーミングまたはプログレッシブダウンロードに適したダイレクトビデオ URL を取得します。

**サードパーティのビデオプレーヤーを使用してビデオをデプロイするには：**

1. Adobe Dynamic Media Classicのグローバルナビゲーションバーで、に移動します **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 一般設定]**.
1. 使用する URL のタイプに応じて、次のいずれかの操作を行います。

* ダイレクト HLS ストリーミングビデオ URL （マルチビットレート）を生成するには

  日 **[!UICONTROL アプリケーションの一般設定]** ページ （内） **[!UICONTROL サーバー]** グループ、内 **[!UICONTROL 公開先サーバー名]** テキストフィールドで、ダイレクト URL を作成します。 次の構文を使用します。 `server/is/content/company/folder/filename.m3u8`

  例えば、公開先サーバー名がであるとします `https://s7d9.scene7.com/.` 手順 2 の構文を使用すると、ダイレクト URL は次のようになります。
  `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* ダイレクト HLS ストリーミングビデオ URL （単一ビットレート）を生成するには

  日 **[!UICONTROL アプリケーションの一般設定]** ページ （内） **[!UICONTROL サーバー]** グループ、内 **[!UICONTROL HLS ストリーミング サーバー名]** テキストフィールドで、次の構文を使用してダイレクト URL を作成します。

  `server/company/folder/filename.ext.m3u8`

  例えば、HLS ストリーミングサーバー名がであるとします `https://s7mbrstream.scene7.com/hls-vod/`. 手順 2 の構文を使用すると、ダイレクト URL は次のようになります。
  `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* プログレッシブビデオのダイレクト URL を生成するには

  **[!UICONTROL アプリケーションの全般設定]**&#x200B;ページの「**[!UICONTROL サーバー]**」グループの「**[!UICONTROL プログレッシブビデオサーバー名]**」テキストフィールドで、次の構文を使用して eVideo のダイレクト URL を作成します。

  `server/company/folder/filename`

  例えば、プログレッシブビデオサーバー名がであるとします `https://s7d9.scene7.com/is/content/`. 手順 2 の構文を使用すると、ダイレクト URL は次のようになります。
  `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## ビデオサムネールの操作 {#working-with-video-thumbnails}

Adobe Dynamic Media Classicは、エンコードされたビデオと事前にエンコードされたビデオのサムネールを生成します。 ビデオサムネールは、画像アセットと同じように使用できます。さらに、Adobe Dynamic Media Classicが生成するビデオサムネールの URL を取得できます。 その後、これらの URL をAdobe Dynamic Media Classicの外部にデプロイできます。 例えば、Web サイト上の検索結果、関連するビデオリスト、ビデオ再生リストにサムネールを配信できます。

ビデオの最初の不均一のフレーム（真っ黒でないフレーム、真っ白でないフレームなど）に基づきサムネールが生成されます。

### ビデオサムネール URL の取得 {#obtaining-video-thumbnail-urls}

Adobe Dynamic Media Classicは、アップロード処理中にビデオサムネールを自動的に生成します。 サムネールは、リスト表示とグリッド表示の参照パネルに表示されます。

ビデオサムネールの URL を生成するには、公開操作を実行します。

参照： [ビデオを公開](deploying-video-websites-mobile-sites.md#publishing_video).

公開後、URL および埋め込みコードパネルの詳細ビューでビデオサムネールの URL を取得できます。を選択 **[!UICONTROL URL をコピー]** ビデオのサムネールの右側に表示されるので、関連する URL をコピーできます。

### ビデオビューアでのポスターフレームの変更 {#modifying-poster-frames-in-video-viewers}

*ポスターフレーム*&#x200B;は、ビデオの再生開始前にビデオビューアに表示される最初のフレームです。Adobe Dynamic Media Classicでは、ビデオサムネールをポスターフレームとして使用します。

ポスターフレームに画像修飾子を適用できます。例えば、ポスターフレームを切り抜いたり、透明にしたりすることができます。ポスターフレームを変更するには、ビデオビューアの設定画面を開いて、「ポスター画像修飾子」セクションに修飾子を入力します。

参照： [ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

参照： [画像サービングガイド](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-is-home#image-serving-api).

また、ビデオサムネールの URL に修飾子を追加して、ビデオサムネールを変更することもできます。

>[!MORELIKETHIS]
>
>* [ファイルを公開](publishing-files.md#publishing_files)