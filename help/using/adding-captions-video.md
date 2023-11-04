---
title: ビデオにキャプションを追加
description: Adobe Dynamic Media Classicでビデオにキャプションを追加する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 32%

---

# ビデオにキャプションを追加 {#adding-captions-to-video}

キャプションを単一のビデオまたはアダプティブビデオセットに追加することにより、ビデオの提供先をグローバルマーケットに拡張することができます。キャプションを追加することで、オーディオをダビングする必要がなくなります。また、異なる言語ごとにオーディオを再度録音する必要もなくなります。ビデオは録画されたときの言語で再生されます。外国語のサブタイトルが表示されるため、異なる言語のユーザもオーディオ部分を理解できます。

また、キャプションにより、耳の不自由なユーザや難聴者向けにクローズドキャプションを使用することで、高いアクセス性が可能になります。

>[!NOTE]
>
>使用されるビデオプレーヤーがキャプションの表示に対応している必要があります。

キャプション効果を設定し、キャプションメニュー自体を編集するには、次のビューアのメニューのテキストを含めます。

* `Universal_HTML5_Video` 閲覧者
* `Universal_HTML5_MixedMedia_dark` 閲覧者
* `Universal_HTML5_MixedMedia_light` 閲覧者

詳しくは、 [ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

関連トピック [ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classicでは、キャプションファイルを JSON(JavaScript Object Notation) 形式に変換できます。 この変換によって、隠されたビデオ内容全文として、JSON テキストを Web ページに埋め込むことができます。その後、検索エンジンでは、コンテンツをクロールおよびインデックス付けして、ビデオを見つけやすくし、顧客にビデオコンテンツの詳細を提供できます。

詳しくは、 [静的（画像以外の）コンテンツを提供する](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api) （内） *Adobe画像サービング API のヘルプ* を参照してください。

**ビデオにキャプションを追加するには:**

1. Adobe Dynamic Media Classicの外部でサードパーティのアプリケーションを使用して、使用しているビューアタイプに基づいてビデオキャプションファイルを作成します。

   | ビューアタイプ | キャプションファイル |
   |--- |--- |
   | HTML5 | HTML5 ビデオビューアを使用している場合、作成するキャプションファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。キャプションのファイル名拡張子は .vtt です。WebVTT のキャプション規格について、さらに詳しく調べることができます。<br><br>[WebVTT を参照](https://w3c.github.io/webvtt/):Web Video Text Tracks 形式。 <br><br>Adobe Dynamic Media Classicの外部でキャプションファイルを作成する際に使用できる、無料および有料のツールおよびサービスが用意されています。 例えば、スタイルのないシンプルなビデオキャプションファイルを作成するには、次の無料のオンラインキャプションオーサリングおよび編集ツールを使用できます。 <br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>最適な結果を得るには、このツールを Internet Explorer 9 以降、Google Chrome、Safari のいずれかで使用してください。 <br><br>ツールの <b>ビデオファイルの URL を入力</b> 「 」フィールドにビデオファイルの URL を貼り付け、「 」を選択します。 <b>読み込み</b>. <br><br>例えば、ビデオファイルにAdobe Dynamic Media Classic URL を使用している場合は、( アダプティブビデオセットやプライマリビデオではなく ) 個々のビデオアセットをダブルクリックして、詳細ビューで開きます。 詳細ビューの右側のパネルで、「URL と埋め込みコード」を展開します。次に、「モバイル」グループの「モバイル（プログレッシブ） 」の右にある「 」を選択します。 <b>URL をコピー</b>. このプロセスにより、ビデオファイル自体の URL が得られ、その URL を <b>ビデオファイルの URL を入力</b> フィールドに入力します。 その後、Internet Explorer、Chrome または Safari でビデオをネイティブに再生できます。作成するサイトの画面に示される指示に従って、WebVTT ファイルを保存します。完了したら、キャプションファイルの内容をコピーしてプレーンテキストエディターに貼り付け、ファイル名の拡張子を VTT にして保存します。 <br><br><b>注意：</b> 英語以外の言語でビデオキャプションをグローバルにサポートする場合、WebVTT 標準では、サポートする言語ごとに個別の.vtt ファイルを作成して呼び出す必要があります。 <br><br>通常、キャプション VTT ファイルにはビデオファイルと同じ名前を指定し、captions を付加します。これにより、既存の Web コンテンツ管理システムを使用して、ビデオ URL の生成を自動化できます。 |

1. Adobe Dynamic Media Classicで、WebVTT、DFXP、または SMPTE XML キャプションファイルをアップロードします。

   詳しくは、 [ファイルをアップロード](uploading-files.md#uploading_files).

1. 左側のアセットライブラリパネルで、アップロードしたキャプションファイルに関連付けるビデオファイルを含んでいるアセットフォルダに移動します。
1. アセットの参照パネルで 1 つのビデオアセットを選択し、アセットのサムネール画像の下でを選択します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
1. 「ビューアリスト」テーブルで、「HTML5 ビューア」という名前を探します。 **Univeral_HTML5_Video**, **Universal_HTML5_MixedMedia_dark**&#x200B;または **Universal_HTML5_MixedMedia_light**&#x200B;次のいずれかの操作を行います。

   * ポップアップビデオビューアエクスペリエンスの場合は、 **[!UICONTROL URL をコピー]** を名前の右端にドラッグします。

     コピーしたビデオの URL を次の構文で追加して、コピーした URL とキャプションファイルを関連付けることができます。

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     次の点に注意してください。 `,1` キャプション URL パスの末尾に配置する。 パス内の VTT ファイル名拡張子の直後で、オプションで、をに設定して、ビデオプレーヤーバーのクローズドキャプションボタンの有効/無効を切り替えることができます。 `1` または `0`、それぞれ。

   * 埋め込みビデオビューアエクスペリエンスの場合、 **[!UICONTROL 埋め込みコード]** を名前の右端にドラッグします。

     埋め込みコードダイアログボックスで、「 **[!UICONTROL クリップボードにコピー]**.

     HTML5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`または `Universal_HTML5_MixedMedia_light` ビューアでは、コピーした埋め込みコードを次のように追加します。

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     次の点に注意してください。 `,1` URL パスの末尾に配置されます。 URL パス内の VTT ファイル名拡張子の直後で、オプションで、ビデオプレーヤーバーのキャプションボタンの有効/無効を切り替えることができます。そのためには、をに設定します。 `1` または `0`、それぞれ。
