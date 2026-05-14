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
autotag-review: '2026-05-13T17:36:57.321Z'
TQID: 'https://experienceleague.adobe.com/wFvWrYRUlCvHwaZFcCcHVDS3ApzUEX2AkFD3EovQJ1g'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: cc72dcf1-72e1-48cc-b434-e7c27d62d67c
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 730
ht-degree: 15%

---

# ビデオにキャプションを追加 {#add-captions-to-video}

動画のリーチをグローバル市場に拡大。 これは、単一のビデオまたはアダプティブビデオセットにキャプションを追加することで可能です。 キャプションを追加することで、オーディオをダビングする必要がなくなります。また、異なる言語ごとにオーディオを再度録音する必要もなくなります。 ビデオは録画されたときの言語で再生されます。 外国語のサブタイトルが表示されるため、異なる言語のユーザもオーディオ部分を理解できます。

また、キャプションにより、耳の不自由なユーザや難聴者向けにクローズドキャプションを使用することで、高いアクセス性が可能になります。

>[!NOTE]
>
>使用するビデオプレーヤーは、キャプションの表示をサポートしている必要があります。

キャプションエフェクトを設定し、次のいずれかのビューアのメニューのテキストを含むキャプションメニュー自体を編集するには：

* `Universal_HTML5_Video`人の閲覧者
* `Universal_HTML5_MixedMedia_dark`人の閲覧者
* `Universal_HTML5_MixedMedia_light`人の閲覧者

[&#x200B; ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)を参照してください。

[&#x200B; ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets)も参照してください。

Adobe Dynamic Media Classicでは、キャプションファイルをJSON （JavaScript Object Notation）形式に変換できます。 この変換により、JSON テキストをWeb ページに埋め込み、ビデオの隠れた完全なトランスクリプトとして使用できます。 そして、検索エンジンがコンテンツをクロールしてインデックスを作成することで、動画をより見つけやすくし、動画コンテンツに関する詳細を提供します。

URLでJSON関数を使用する方法について詳しくは、の[静的（画像でない）コンテンツの提供](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api)を参照してください。

**ビデオにキャプションを追加するには：**

1. Adobe Dynamic Media Classic以外のサードパーティアプリケーションを使用して、使用しているビューアータイプに基づいてビデオキャプションファイルを作成します。

   | ビューアタイプ | キャプションファイル |
   |--- |--- |
   | HTML5 | HTML5 ビデオビューアを使用している場合、作成するキャプションファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。 キャプション ファイル名拡張子は`.VTT`です。 WebVTT のキャプション規格について、さらに詳しく調べることができます。<br><br>[WebVTT](https://w3c.github.io/webvtt/)を参照：Web ビデオのテキスト形式を追跡します。 <br><br>WebVTT キャプションファイルの作成に使用できる無料および有料のツールとサービスを提供しているWeb サイトは数多くあります。 <br><br>WebVTT ファイルを作成して保存するには、サイトの画面の指示に従います。 終了したら、キャプションファイルの内容をコピーしてプレーンテキストエディターに貼り付け、VTT ファイル名拡張子を付けて保存します。 <br><br><b>注意：</b>英語以外の言語でビデオキャプションをグローバルにサポートするには、WebVTT標準で、サポートする言語ごとに`.VTT` ファイルと呼び出しを個別に作成する必要があります。 <br><br>一般的に、キャプション VTT ファイルにビデオ ファイルと同じ名前を付け、キャプションを付けて追加します。 これにより、既存のWeb コンテンツ管理システムを使用してビデオ URLの生成を自動化できます。 |

1. Adobe Dynamic Media Classicで、WebVTT、DFXP、またはSMPTE XML キャプションファイルをアップロードします。

   [&#x200B; ファイルのアップロード &#x200B;](uploading-files.md#uploading_files)を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたキャプションファイルに関連付けるビデオファイルを含むアセットフォルダーに移動します。
1. アセット参照パネルで、1つのビデオアセットを選択し、アセットのサムネール画像の下にある「**[!UICONTROL プレビュー]**」 > 「**[!UICONTROL ビューアーリスト]**」を選択します。
1. ビューア リスト テーブルで、**Universal_HTML5_Video**、**Universal_HTML5_MixedMedia_dark**&#x200B;または&#x200B;**Universal_HTML5_MixedMedia_light**&#x200B;という名前のHTML5 ビューアを見つけ、次のいずれかの操作を行います。

   * ポップアップビデオのビューアエクスペリエンスの場合は、名前の右端にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。

     次の構文を使用してビデオのコピーURLを追加し、コピーしたURLとキャプションファイルに関連付けることができます。

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     キャプション URL パスの末尾に`,1`をメモします。 パス内のVTT ファイル名拡張子の直後に、ビデオプレーヤーバーのクローズドキャプションボタンをオプションで有効または無効にできます。それぞれ`1`または`0`に設定します。

   * 埋め込みビデオビューアエクスペリエンスの場合は、名前の右端にある「**[!UICONTROL 埋め込みコード]**」を選択します。

     埋め込みコードダイアログボックスで、**[!UICONTROL クリップボードにコピー]**&#x200B;を選択します。

     HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark`、または`Universal_HTML5_MixedMedia_light`のビューアの場合は、コピーした埋め込みコードを次の形式で追加します。

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     URL パスの末尾に`,1`をメモします。 URL パスのVTT ファイル名拡張子の直後に、ビデオプレーヤーバーのキャプションボタンをオプションで有効または無効にできます。それぞれ`1`または`0`に設定します。
