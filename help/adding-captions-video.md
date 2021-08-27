---
title: 'ビデオへのキャプションの追加 '
description: AdobeDynamic Media Classicでビデオにキャプションを追加する方法を説明します。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '904'
ht-degree: 32%

---

# ビデオへのキャプションの追加 {#adding-captions-to-video}

キャプションを単一のビデオまたはアダプティブビデオセットに追加することにより、ビデオの提供先をグローバルマーケットに拡張することができます。キャプションを追加することで、オーディオをダビングする必要がなくなります。また、異なる言語ごとにオーディオを再度録音する必要もなくなります。ビデオは録画されたときの言語で再生されます。外国語のサブタイトルが表示されるため、異なる言語のユーザもオーディオ部分を理解できます。

また、キャプションにより、耳の不自由なユーザや難聴者向けにクローズドキャプションを使用することで、高いアクセス性が可能になります。

>[!NOTE]
>
>使用されるビデオプレーヤーがキャプションの表示に対応している必要があります。

キャプション効果を設定し、キャプションメニュー自体（以下のビューアのメニューのテキストを含む）を編集するには：

* `Universal_HTML5_Video` 閲覧者
* `Universal_HTML5_MixedMedia_dark` 閲覧者
* `Universal_HTML5_MixedMedia_light` 閲覧者

[ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)を参照してください。

[ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets)も参照してください。

AdobeDynamic Media Classicでは、キャプションファイルをJSON(JavaScript Object Notation)形式に変換できます。 この変換によって、隠されたビデオ内容全文として、JSON テキストを Web ページに埋め込むことができます。その後、検索エンジンでコンテンツをクロールおよびインデックス付けして、ビデオを見つけやすくし、ビデオコンテンツに関する詳細を顧客に提供できます。

URLでのJSON関数の使用について詳しくは、*Adobe画像サービングAPIのヘルプ*&#x200B;の[静的（画像以外）コンテンツ](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api)を参照してください。

**ビデオにキャプションを追加するには:**

1. Dynamic Media Classic以外のサードパーティAdobeを使用して、使用しているビューアタイプに基づいてビデオキャプションファイルを作成します。

   | ビューアタイプ | キャプションファイル |
   |--- |--- |
   | HTML5 | HTML5 ビデオビューアを使用している場合、作成するキャプションファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。キャプションのファイル名拡張子は .vtt です。WebVTT のキャプション規格について、さらに詳しく調べることができます。<br><br>[WebVTTを参照してください](https://w3c.github.io/webvtt/)。Webビデオテキストトラックの形式。<br><br>AdobeDynamic Media Classicの外部でキャプションファイルを作成する際に使用できるツールやサービスは、無料でも有料でも提供されています。例えば、スタイル設定のないシンプルなビデオキャプションファイルを作成するには、次の無料のオンラインキャプションオーサリングおよび編集ツールを使用できます。<br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>最適な結果を得るには、このツールをInternet Explorer 9以降、Google Chrome、Safariのいずれかで使用してください。 <br><br>ツールの「ビデオファイ <b>ルのURLを入力」</b> フィールドにビデオファイルのURLを貼り付けて、「読み込 <b>み</b>」を選択します。<br><br>例えば、ビデオファイルにDynamic Media ClassicのAdobeURLを使用している場合は、(アダプティブビデオセットやマスタービデオではなく)個々のビデオアセットをダブルクリックして詳細ビューで開きます。詳細ビューの右側のパネルで、「URL と埋め込みコード」を展開します。次に、「モバイル」グループの「モバイル（プログレッシブ）」の右側にある「<b>URLをコピー</b>」を選択します。 このプロセスにより、ビデオファイル自体のURLが得られ、「<b>ビデオファイルのURLを入力</b>」フィールドに貼り付けることができます。 その後、Internet Explorer、Chrome、または Safari で、ビデオを再生できます。作成するサイトの画面に示される指示に従って、WebVTT ファイルを保存します。完了したら、キャプションファイルの内容をコピーしてプレーンテキストエディターに貼り付け、ファイル名拡張子VTTを付けて保存します。 <br><br><b>注意：</b> 英語以外の言語でビデオキャプションをグローバルにサポートする場合、WebVTT標準では、サポートする言語ごとに個別の.vttファイルを作成し呼び出す必要があります。<br><br>通常、キャプション VTT ファイルにはビデオファイルと同じ名前を指定し、captions を付加します。これにより、既存の Web コンテンツ管理システムを使用して、ビデオ URL の生成を自動化できます。 |

1. AdobeDynamic Media Classicで、WebVTT、DFXP、またはSMPTE XMLキャプションファイルをアップロードします。

   [ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたキャプションファイルに関連付けるビデオファイルを含んでいるアセットフォルダに移動します。
1. アセットの参照パネルで1つのビデオアセットを選択し、アセットのサムネール画像の下で&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;を選択します。
1. ビューアリストの表で、 **Univeral_HTML5_Video** 、 **Universal_HTML5_MixedMedia_dark**&#x200B;または&#x200B;**Universal_HTML5_MixedMedia_light**&#x200B;という名前のHTML5ビューアを探し、次のいずれかの操作を行います。

   * ポップアップビデオビューアエクスペリエンスの場合、名前の右端にある「URL ]**をコピー」を選択します。**[!UICONTROL 

      コピーしたビデオのURLを次の構文で追加し、コピーしたURLにキャプションファイルを関連付けることができます。

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      キャプションURLパスの末尾に`,1`があることに注意してください。 パス内のVTTファイル名拡張子の直後で、オプションでビデオプレーヤーバーのクローズドキャプションボタンの有効と無効を切り替えることができます。それぞれを`1`または`0`に設定します。

   * 埋め込みビデオビューアエクスペリエンスの場合、名前の右端にある「**[!UICONTROL 埋め込みコード]**」を選択します。

      埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

      HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark`または`Universal_HTML5_MixedMedia_light`ビューアの場合は、コピーした埋め込みコードを次のように追加します。

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      URLパスの末尾に`,1`があることに注意してください。 URLパス内のVTTファイル名拡張子の直後で、オプションでビデオプレーヤーバーのキャプションボタンの有効と無効を切り替えることができます。それぞれを`1`または`0`に設定します。
