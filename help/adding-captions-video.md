---
title: ビデオへのキャプションの追加
description: ビデオにキャプションを追加する方法を説明します
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic，ビューア，ビデオ
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
source-git-commit: 9ff171590c65f55cef8c9e5a2b4e77ddbbfa6895
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 51%

---

# ビデオへのキャプションの追加{#adding-captions-to-video}

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

Dynamic Media Classicでは、キャプションファイルをJSON(JavaScript™ Object Notation)形式に変換できます。 この変換によって、隠されたビデオ内容全文として、JSON テキストを Web ページに埋め込むことができます。その後、検索エンジンでコンテンツをクロールおよびインデックス付けして、ビデオを見つけやすくし、ビデオコンテンツに関する詳細を顧客に提供できます。

URLでJSON関数を使用する方法について詳しくは、*Adobe画像サービングAPIのヘルプ*&#x200B;の[静的（画像以外）コンテンツの提供](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api)を参照してください。

**ビデオにキャプションを追加するには**

1. Dynamic Media Classic以外のサードパーティアプリケーションを使用して、使用しているビューアタイプに基づいてビデオキャプションファイルを作成します。

   | ビューアタイプ | キャプションファイル |
   |--- |--- |
   | HTML5 | HTML5 ビデオビューアを使用している場合、作成するキャプションファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。キャプションのファイル名拡張子は .vtt です。WebVTT のキャプション規格について、さらに詳しく調べることができます。<br><br>[WebVTTを参照してください](https://w3c.github.io/webvtt/)。Webビデオテキストトラックの形式。<br><br>Dynamic Media Classic以外でキャプションファイルを作成する際に使用できるツールやサービスは、無料でも有料でも提供されています。例えば、スタイル設定のないシンプルなビデオキャプションファイルを作成するには、次の無料のオンラインキャプションオーサリングおよび編集ツールを使用できます。<br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>最適な結果を得るには、このツールをInternet Explorer 9以降、Google Chrome、Safariのいずれかで使用してください。 <br><br>このツールで、<b>「Enter URL of video file」</b>フィールドにビデオファイルの URL を貼り付けて、<b>「Load」</b>をクリックします。<br><br>例えば、ビデオファイルにDynamic Media Classic URLを使用している場合は、(アダプティブビデオセットやマスタービデオではなく)個々のビデオアセットをダブルクリックして詳細表示で開きます。詳細ビューの右側のパネルで、「URL と埋め込みコード」を展開します。次に、「モバイル」グループで、「モバイル (プログレッシブ)」の右にある「URL をコピー」をクリックします。このプロセスにより、ビデオファイル自体のURLが得られ、「<b>ビデオファイルのURLを入力</b>」フィールドに貼り付けることができます。 その後、Internet Explorer、Chrome、または Safari で、ビデオを再生できます。作成するサイトの画面に示される指示に従って、WebVTT ファイルを保存します。完了したら、キャプションファイルのコンテンツをコピーしてプレーンテキストエディターに貼り付け、.vtt のファイル名拡張子で保存します。<br><br><b>注意：</b> 英語以外の言語でビデオキャプションをグローバルにサポートする場合、WebVTT標準では、サポートする言語ごとに個別の.vttファイルを作成し呼び出す必要があります。<br><br>通常、キャプション VTT ファイルにはビデオファイルと同じ名前を指定し、captions を付加します。これにより、既存の Web コンテンツ管理システムを使用して、ビデオ URL の生成を自動化できます。 |

1. Dynamic Media Classicで、WebVTT、DFXP、またはSMPTE XMLキャプションファイルをアップロードします。

   詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたキャプションファイルに関連付けるビデオファイルを含んでいるアセットフォルダに移動します。
1. アセットの参照パネルで 1 つのビデオアセットを選択して、アセットのサムネール画像の下にある&#x200B;**[!UICONTROL プレビュー]**／**[!UICONTROL ビューアリスト]**&#x200B;をクリックします。
1. ビューアリストの表で、 **Univeral_HTML5_Video** 、 **Universal_HTML5_MixedMedia_dark**&#x200B;または&#x200B;**Universal_HTML5_MixedMedia_light**&#x200B;という名前のHTML5ビューアを探し、次のいずれかの操作を行います。

   * ポップアップビデオビューアの操作については、名前の最も右側にある&#x200B;**[!UICONTROL 「URL をコピー」]**&#x200B;をクリックします。

      コピーしたビデオの URL を次の構文と共に追加し、この URL とコピーしたキャプションファイルの URL を関連付けます。

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      キャプションURLパスの末尾に`,1`があることに注意してください。 パス内の.vttファイル名拡張子の直後で、オプションでビデオプレーヤーバーのクローズドキャプションボタンを有効または無効にできます。有効にするには、それぞれ`1`または`0`に設定します。

   * 埋め込まれたビデオビューアの操作については、名前の最も右側にある&#x200B;**[!UICONTROL 「埋め込みコード」]**&#x200B;をクリックします。

      埋め込みコードダイアログボックスで、**[!UICONTROL 「クリップボードにコピー」]**&#x200B;をクリックします。

      HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark`または`Universal_HTML5_MixedMedia_light`ビューアの場合は、コピーした埋め込みコードを次のように追加します。

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      URLパスの末尾に`,1`があることに注意してください。 URLパス内の.vttファイル名拡張子の直後で、オプションでビデオプレーヤーバーのキャプションボタンの有効と無効を切り替えることができます。それぞれを`1`または`0`に設定します。
