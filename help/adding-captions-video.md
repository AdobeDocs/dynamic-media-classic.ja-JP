---
title: ビデオへのキャプションの追加
description: ビデオにキャプションを追加する方法を説明します。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Mediaクラシック，ビューア，ビデオ
role: 開業医
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 51%

---


# ビデオへのキャプションの追加{#adding-captions-to-video}

キャプションを単一のビデオまたはアダプティブビデオセットに追加することにより、ビデオの提供先をグローバルマーケットに拡張することができます。キャプションを追加することで、オーディオをダビングする必要がなくなります。また、異なる言語ごとにオーディオを再度録音する必要もなくなります。ビデオは録画されたときの言語で再生されます。外国語のサブタイトルが表示されるため、異なる言語のユーザもオーディオ部分を理解できます。

また、キャプションにより、耳の不自由なユーザや難聴者向けにクローズドキャプションを使用することで、高いアクセス性が可能になります。

>[!NOTE]
>
>使用されるビデオプレーヤーがキャプションの表示に対応している必要があります。

キャプション効果の設定や、次のビューアのメニューテキストを含むキャプションメニュー自体の編集については、[ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)を参照してください。

* `Universal_HTML5_Video` 閲覧者.
* `Universal_HTML5_MixedMedia_dark` 閲覧者.
* `Universal_HTML5_MixedMedia_light` 閲覧者.

[ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets)も参照してください。

Dynamic Mediaクラシックでは、キャプションファイルをJSON(JavaScript™ Object Notation)形式に変換できます。 この変換によって、隠されたビデオ内容全文として、JSON テキストを Web ページに埋め込むことができます。検索エンジンは、コンテンツをクロールしてインデックスを付けることで、ビデオが見つかりやすくなり、顧客にビデオコンテンツに関する詳細を示すことができます。

URLでのJSON関数の使用について詳しくは、*Adobe画像サービングAPIヘルプ*&#x200B;の[静的な（画像以外の）コンテンツ](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents.html?lang=en#image-serving-api)の提供を参照してください。

**ビデオにキャプションを追加するには**

1. Dynamic Mediaクラシック以外のサードパーティアプリケーションを使用して、使用しているビューアタイプに基づいてビデオキャプションファイルを作成します。

   | ビューアタイプ | キャプションファイル |
   |--- |--- |
   | HTML5 | HTML5 ビデオビューアを使用している場合、作成するキャプションファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。キャプションのファイル名拡張子は .vtt です。WebVTT のキャプション規格について、さらに詳しく調べることができます。<br><br>[WebVTT](https://dev.w3.org/html5/webvtt/):Webビデオテキストトラックの形式です。<br><br>Dynamic Mediaクラシック以外でキャプションファイルを作成する際に使用できるツールやサービスは、無料と有料の両方です。例えば、スタイル設定のない単純なビデオキャプションファイルを作成する場合、次の無料のオンラインでのキャプション作成および編集ツールを使用できます。<br><br>[WebVTT Caption Maker](https://testdrive-archive.azurewebsites.net/Graphics/CaptionMaker/Default.html) <br><br>最良の結果を得るには、Internet Explorer 9以上、Google ChromeまたはSafariのツールを使用してください。 <br><br>このツールで、<b>「Enter URL of video file」</b>フィールドにビデオファイルの URL を貼り付けて、<b>「Load」</b>をクリックします。<br><br>例えば、ビデオファイルにDynamic MediaクラシックURLを使用している場合、(アダプティブビデオセットやマスタービデオではなく)個々のビデオアセットを重複クリックして詳細表示で開きます。詳細ビューの右側のパネルで、「URL と埋め込みコード」を展開します。次に、「モバイル」グループで、「モバイル (プログレッシブ)」の右にある「URL をコピー」をクリックします。この処理により、ビデオファイル自体のURLが得られ、それを<b>「Enter URL of video file</b>」フィールドに貼り付けることができます。 その後、Internet Explorer、Chrome、または Safari で、ビデオを再生できます。作成するサイトの画面に示される指示に従って、WebVTT ファイルを保存します。完了したら、キャプションファイルのコンテンツをコピーしてプレーンテキストエディターに貼り付け、.VTTのファイル名拡張子で保存します。 <br><br><b>注意：英語以外の言語のビデオキャプションをグローバルサポートする</b> ために、WebVTT規格では、サポートする言語ごとに個別の.vttファイルを作成して呼び出す必要があります。<br><br>通常、キャプション VTT ファイルにはビデオファイルと同じ名前を指定し、captions を付加します。これにより、既存の Web コンテンツ管理システムを使用して、ビデオ URL の生成を自動化できます。 |

1. Dynamic Mediaクラシックで、WebVTT、DFXPまたはSMPTEのXMLキャプションファイルをアップロードします。

   詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたキャプションファイルに関連付けるビデオファイルを含んでいるアセットフォルダに移動します。
1. アセットの参照パネルで 1 つのビデオアセットを選択して、アセットのサムネール画像の下にある&#x200B;**[!UICONTROL プレビュー]**／**[!UICONTROL ビューアリスト]**&#x200B;をクリックします。
1. ビューアリストの表で、**Univeral_HTML5_Video**、**Universal_HTML5_MixedMedia_dark**&#x200B;または&#x200B;**Universal_HTML5_MixedMedia_light**&#x200B;という名前のHTML5ビューアを探し、次のいずれかを実行します。

   * ポップアップビデオビューアの操作については、名前の最も右側にある&#x200B;**[!UICONTROL 「URL をコピー」]**&#x200B;をクリックします。

      コピーしたビデオの URL を次の構文と共に追加し、この URL とコピーしたキャプションファイルの URL を関連付けます。

      `&caption=<full Copy URL path to the caption file .vtt>,1`

      キャプションURLパスの末尾の`,1`に注意してください。 パス内のファイル名拡張子.VTTの直後に、ビデオプレーヤーバーのクローズドキャプションボタンの有効（オプション）または無効（オプション）を、それぞれ`1`または`0`に設定できます。

   * 埋め込まれたビデオビューアの操作については、名前の最も右側にある&#x200B;**[!UICONTROL 「埋め込みコード」]**&#x200B;をクリックします。

      埋め込みコードダイアログボックスで、**[!UICONTROL 「クリップボードにコピー」]**&#x200B;をクリックします。

      HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark`または`Universal_HTML5_MixedMedia_light`ビューアの場合、コピーした埋め込みコードを次の構文と共に追加します。

      `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1”`

      URLパスの末尾の`,1`をメモしておきます。 URLパス内のファイル名拡張子.VTTの直後に、ビデオプレーヤーバーのキャプションボタンの有効（オプション）と無効（オプション）を、それぞれ`1`または`0`に設定します。

