---
title: Web サイトやモバイルサイトへのビデオの配信
seo-title: Web サイトやモバイルサイトへのビデオの配信
description: 'null'
seo-description: Webサイトやモバイルサイトにビデオを配信する方法について説明します。
uuid: 22bb4402-c0ab-4df0-89b9-99707d111927
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 0d006314-c4cc-4f6c-a51c-6075bb445e39
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1689'
ht-degree: 69%

---


# Web サイトやモバイルサイトへのビデオの配信{#deploying-video-to-your-websites-and-mobile-sites}

Webサイト、モバイルサイトおよびデスクトップアプリケーションは、URL文字列または埋め込みコードを使用して、ビデオなどのDynamic Media Classicサーバーコンテンツにアクセスします。 Dynamic Media Classicは、公開処理中に、これらのURL文字列をアクティブにします。 Webページ、モバイルページおよびデスクトップアプリケーションにビデオのURL文字列または埋め込みコードを設定するには、Dynamic Media ClassicからURL文字列または埋め込みコードをコピーします。

>[!NOTE]
>
>URL または埋め込みコードは、アセットを公開するまでアクティブになりません。

## ビデオの公開 {#publishing-video}

ビデオを公開すると、Dynamic Media Classic ServerはビデオをWebサイト、モバイルサイトまたはアプリケーションに配信できます。

ビデオの公開に使用できる方法は次の 2 つあります。

* **アップロード時にビデオを自動的に即時公開する**

   ビデオのアップロード処理の一環として、Dynamic Media Classicは、ビデオがアップロードされエンコードされたときに、自動的にビデオを公開できます。 この即時公開機能があることで、アップロードとエンコード後にビデオを個別に公開する必要がありません。

* **アップロード後にビデオを手動で公開する**

   ビデオをすぐに公開したくない場合は、いつでもビデオを手動で公開できます。

ビデオを公開すると、HTMLページやアプリケーションコードのURL文字列がアクティブになります。

**ビデオを公開するには**

1. 次のいずれかの操作を行います。

   * ビデオをアップロード時に自動的に即時公開するには、アップロード画面で、「**アップロード後に公開**」をクリックします。完了後は、それ以上の手順は必要ありません。
   * アップロード後にビデオを手動で公開するには、参照パネルでビデオを選択し、グローバルナビゲーションバーで「**公開**」をクリックします。

## ビデオ URL のモバイルサイトまたは Web サイトへのリンク {#linking-a-video-url-to-a-mobile-site-or-a-website}

ビデオの公開後、そのビデオの URL を取得して Web サイト、モバイルサイトまたはデスクトップアプリケーションで使用できます。このビデオ URL は、Web ページの上のポップアップウィンドウかモーダルウィンドウでビデオを再生する場合に使用します。

顧客がリンクをクリックすると、デバイス、帯域幅および画面サイズが自動的に検出されます。デスクトップの場合は、定義済みビューアでの再生に適したビデオが表示され、スマートフォンおよびタブレットの場合は、携帯端末のネイティブビデオプレーヤーでの再生に適したビデオが表示されます。

[Web ページへのビデオビューアの埋め込み](deploying-video-websites-mobile-sites.md#embedding_the_video_viewer_on_a_web_page)も参照してください。

**ビデオ URL をモバイルサイトまたは Web サイトにリンクするには**

1. アセットの参照パネルの「表示」ドロップダウンリストで「**ビデオ**」または「**アダプティブビデオセット**」をクリックします。
1. 左側のアセットライブラリパネルで、リンクするビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **「グリッドビュー」**&#x200B;または&#x200B;**「リストビュー」**&#x200B;をクリックします。アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。右側の URL と埋め込みコードパネルの「HTTP ストリーミング」で、目的のビューアの右側の「**URL をコピー**」をクリックします。As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.
   * **「グリッドビュー」**&#x200B;をクリックします。アセットの参照パネルで 1 つのアセットを選択して、サムネール画像の下にある&#x200B;**プレビュー**／**ビューアリスト**&#x200B;をクリックします。

      ビューアリストページの表の「アクション」列にある「**URL をコピー**」をクリックします。As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * **「リストビュー」**&#x200B;をクリックします。アセットの参照パネルで 1 つのアセットを選択して、サムネール画像の右側にある&#x200B;**プレビュー**／**ビューアリスト**&#x200B;をクリックします。

      ビューアリストページの表の「アクション」列にある「**URL をコピー**」をクリックします。As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

   * **「グリッドビュー」**、**「リストビュー」**、または&#x200B;**「詳細ビュー」**&#x200B;をクリックします。同じツールバーにある&#x200B;**プレビュー**／**ビューアリスト**&#x200B;をクリックします。

      ビューアリストページの表の「アクション」列にある「**URL をコピー**」をクリックします。As a best practice, copy the URL associated with the `Universal_HTML5_Video` viewer.

1. HTML5 ビデオ URL のリンクを Web サイトおよびモバイルサイトに貼り付けます。

## Web ページへのビデオビューアの埋め込み {#embedding-the-video-viewer-on-a-web-page}

Web ページにビデオを埋め込んで再生したい場合は、「埋め込みコード」機能を使用します。埋め込みコードをクリップボードにコピーして、Web ページに貼り付けることができます。埋め込みコードダイアログボックスでは、コードの編集はできません。

[ビデオ URL のモバイルサイトまたは Web サイトへのリンク](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)も参照してください。

**Web ページにビデオビューアを埋め込むには**

1. アセットの参照パネルの「表示」ドロップダウンリストで「**ビデオ**」または「**アダプティブビデオセット**」をクリックします。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーしたいビデオまたはアダプティブビデオセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **「グリッドビュー」**&#x200B;または&#x200B;**「リストビュー」**&#x200B;をクリックします。アセットの参照パネルで、単一アセットのビデオサムネールをダブルクリックして、詳細ビューで開きます。右側の URL と埋め込みコードパネルの「HTTP ストリーミング」で、目的のビューアの右側の「**埋め込みコード**」をクリックします。As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.
   * 「**グリッドビュー**」をクリックします。アセットの参照パネルで 1 つのアセットを選択して、ビデオサムネール画像の下にある&#x200B;**プレビュー**／**ビューアリスト**&#x200B;をクリックします。

      ビューアリストページの表の「アクション」列にある「**埋め込みコード**」をクリックします。As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * **「リストビュー」**&#x200B;をクリックします。アセットの参照パネルで 1 つのアセットを選択して、サムネール画像の右側にある&#x200B;**プレビュー**／**ビューアリスト**&#x200B;をクリックします。

      ビューアリストページの表の「アクション」列にある「**埋め込みコード**」をクリックします。As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

   * **「グリッドビュー」**、**「リストビュー」**、または&#x200B;**「詳細ビュー」**&#x200B;をクリックします。同じツールバーにある&#x200B;**プレビュー**／**ビューアリスト**&#x200B;をクリックします。

      ビューアリストページの表の「アクション」列にある「**埋め込みコード**」をクリックします。As a best practice, click **Embed Code** that is associated with the `Universal_HTML5_Video` viewer.

1. 埋め込みコードダイアログボックスで、**「クリップボードにコピー」**&#x200B;をクリックします。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. 「**閉じる**」をクリックします。
1. 埋め込みコードを Web ページに貼り付けます。

### Implementing embed code for using HTML5 video with MP4 video assets {#implementing-embed-code-for-using-html-video-with-mp-video-assets}

If you do not use the Dynamic Media Classic HTML5 video player, but instead want to use the native HTML5 `<video>` tag with MP4 video assets, you can use the following embed code sample:

```as3
<video poster="S7 video thumbnail URL" controls> 
        <source src="S7 OGG video asset URL (no player)" type='video/ogg; codecs="theora, vorbis"'/> 
        <source src="S7 MP4 mobile progressive video asset URL (no player)" type='video/mp4; codecs="avc1.4D401E, mp4a.40.2"'/> 
        <p>This is fallback content</p> 
</video>
```

* Replace `"S7 video thumbnail URL"` with the video’s thumbnail URL. これは、ビデオを再生する前にユーザに表示されるビデオサムネールの画像です。

   [ビデオサムネールの URL の取得](deploying-video-websites-mobile-sites.md#obtaining_video_thumbnail_urls)を参照してください。

* Replace `"S7 OGG video asset URL (no player)"` with the video’s progressive URL for OGG video.

   詳しくは、[ビデオ URL のモバイルサイトまたは Web サイトへのリンク](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)を参照してください。

* ビデオ `"S7 MP4 mobile progressive video asset URL (no player)"` のモバイルプログレッシブURLに置き換えます。

   詳しくは、[ビデオ URL のモバイルサイトまたは Web サイトへのリンク](deploying-video-websites-mobile-sites.md#linking_a_video_url_to_a_mobile_site_or_a_website)を参照してください。

## サードパーティのビデオプレーヤーを使用したビデオの配信 {#deploying-video-using-a-third-party-video-player}

Dynamic Media Classicビデオビューアの代わりに、サードパーティのビデオプレーヤーまたはカスタムに組み込まれたビデオプレーヤーを使用する場合、HLSマルチビットレートビデオストリーミングまたはプログレッシブダウンロードで機能するダイレクトビデオURLを取得できます。

**サードパーティのビデオプレーヤーを使用してビデオを配信するには**

1. In Dynamic Media Classic, on the Global Navigation bar, click **Setup** > **Application Setup** > **General Settings**.
1. 使用する URL のタイプに応じて、次のいずれかの操作を行います。
* HLSストリーミングビデオのダイレクトURL（マルチビットレート）を生成するには

   ア **プリケーションの全般設定** ページの「 **サーバ** 」グループの「 **公開先サーバー名** 」テキストフィールドで、次の構文を使用してダイレクトURLを作成します。 `server/is/content/company/folder/filename.m3u8`
例えば、公開済みサーバー名が手順2の構文を `https://s7d9.scene7.com/.` 使用している場合、ダイレクトURLは次のようになります。
   `https://s7d9.scene7.com/is/content/GeoRetail/AdobeRIA-AVS.m3u8`

* HLSストリーミングビデオのダイレクトURL（シングルビットレート）を生成するには

   On the **Application General Settings** page, in the **Servers** group, in the **HLS Streaming Server Name** text field, construct the direct URL using the following syntax:
   `server/company/folder/filename.ext.m3u8`
例えば、HLSストリーミングサーバー名が次のと `https://s7mbrstream.scene7.com/hls-vod/`します。 手順 2 の構文を使用して、次のようなダイレクト URL を作成できます。
   `https://s7mbrstream.scene7.com/hls-vod/GeoRetail/MBR/ToyStory3\_Teaser1\_High\_iPad\_768x432\_1296K.mp4.m3u8`

* プログレッシブビデオのダイレクト URL を生成するには

   **アプリケーションの全般設定**&#x200B;ページの「**サーバー**」グループの「**プログレッシブビデオサーバー名**」テキストフィールドで、次の構文を使用して eVideo のダイレクト URL を作成します。 `server/company/folder/filename`
For example, suppose the progressive video server name is `https://s7d9.scene7.com/is/content/`. 手順 2 の構文を使用して、次のようなダイレクト URL を作成できます。
   `https://s7d9.scene7.com/e2/GeoRetail/SourceVideo/outdoors.mp4`

## ビデオサムネールの操作 {#working-with-video-thumbnails}

Dynamic Media Classicは、エンコードされたビデオおよび事前にエンコードされたビデオのサムネールを生成します。 ビデオサムネールは、画像アセットと同じように使用できます。また、Dynamic Media Classicが生成するビデオサムネールのURLを取得し、これらのURLをDynamic Media Classicの外部にデプロイできます。 例えば、Web サイト上の検索結果、関連するビデオリスト、ビデオ再生リストにサムネールを配信できます。

ビデオの最初の不均一のフレーム（真っ黒でないフレーム、真っ白でないフレームなど）に基づきサムネールが生成されます。

### ビデオサムネールの URL の取得 {#obtaining-video-thumbnail-urls}

Dynamic Media Classicは、アップロード処理中にビデオサムネールを自動的に生成します。 サムネールは、リストビューとグリッドビューの参照パネルに表示されます。

ビデオサムネールの URL を生成するには、公開操作を実行します。

詳しくは、[ビデオの公開](deploying-video-websites-mobile-sites.md#publishing_video)を参照してください。

公開後、URL および埋め込みコードパネルの詳細ビューでビデオサムネールの URL を取得できます。ビデオサムネールの右側の&#x200B;**「URL をコピー」**&#x200B;をクリックすると、URL をコピーできます。

### ビデオビューアでのポスターフレームの変更 {#modifying-poster-frames-in-video-viewers}

*ポスターフレーム*&#x200B;は、ビデオの再生開始前にビデオビューアに表示される最初のフレームです。ダイナミックMedia Classicでは、ビデオサムネールがポスターフレームとして使用されます。

ポスターフレームに画像修飾子を適用できます。例えば、ポスターフレームを切り抜いたり、透明にしたりすることができます。ポスターフレームを変更するには、ビデオビューアの設定画面を開いて、「ポスター画像修飾子」セクションに修飾子を入力します。

詳しくは、[ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)を参照してください。

www.adobe.com/go/learn_s7_image_server_guide_enを参照し [てください](https://www.adobe.com/go/learn_s7_image_server_guide_en)。

また、ビデオサムネールの URL に修飾子を追加して、ビデオサムネールを変更することもできます。

>[!MORELIKETHIS]
>
>* [ファイルの公開 ](publishing-files.md#publishing_files)

