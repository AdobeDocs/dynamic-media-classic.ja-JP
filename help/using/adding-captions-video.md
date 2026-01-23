---
title: ビデオへのキャプションの追加
description: Adobe Dynamic Media Classicでビデオにキャプションを追加する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 66a1ab20-6036-4c3d-bb66-dd06d917c7f2
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '703'
ht-degree: 15%

---

# ビデオへのキャプションの追加 {#add-captions-to-video}

ビデオの提供範囲をグローバル市場に拡大する。 そのためには、1 つのビデオまたはアダプティブビデオセットにキャプションを追加します。 キャプションを追加することで、オーディオをダビングする必要がなくなります。また、異なる言語ごとにオーディオを再度録音する必要もなくなります。ビデオは録画されたときの言語で再生されます。外国語のサブタイトルが表示されるため、異なる言語のユーザもオーディオ部分を理解できます。

また、キャプションにより、耳の不自由なユーザや難聴者向けにクローズドキャプションを使用することで、高いアクセス性が可能になります。

>[!NOTE]
>
>使用するビデオプレーヤーがキャプションの表示に対応する必要があります。

次のいずれかのビューアでキャプション効果を設定し、メニューのテキストを含むキャプションメニュー自体を編集するには：

* `Universal_HTML5_Video` ビューア
* `Universal_HTML5_MixedMedia_dark` ビューア
* `Universal_HTML5_MixedMedia_light` ビューア

詳しくは [&#x200B; ビデオビューアプリセットの追加または編集 &#x200B;](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) を参照してください。

[&#x200B; ビューアプリセットの追加と編集 &#x200B;](application-setup.md#adding_and_editing_viewer_presets) も参照してください。

Adobe Dynamic Media Classicでは、キャプションファイルを JSON （JavaScript Object Notation）形式に変換できます。 このように変換できるので、JSON テキストを、ビデオの完全なトランスクリプトとして表示せずに web ページに埋め込むことができます。 その後、検索エンジンがコンテンツをクロールしてインデックスを作成します。これにより、ビデオを見つけやすくなるとともに、ビデオコンテンツの詳細がユーザーに提供されます。

URL で JSON 関数を使用する方法について詳しくは、[&#x200B; の静的コンテンツ（画像以外）の提供 &#x200B;](https://experienceleague.adobe.com/ja/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) を参照してください。

**ビデオにキャプションを追加するには：**

1. Adobe Dynamic Media Classic以外のサードパーティアプリケーションを使用して、使用しているビューアのタイプに基づいてビデオキャプションファイルを作成します。

   | ビューアタイプ | キャプションファイル |
   |--- |--- |
   | HTML5 | HTML5 ビデオビューアを使用している場合、作成するキャプションファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。キャプションファイルの拡張子は `.VTT` です。 WebVTT のキャプション規格について、さらに詳しく調べることができます。<br><br>[WebVTT を参照 &#x200B;](https://w3c.github.io/webvtt/):Web ビデオテキストトラック形式。 <br><br>WebVTT キャプションファイルの作成に使用できる、無料および有料のツールやサービスを提供する web サイトは多くあります。 <br><br> サイトの画面上の指示に従って、WebVTT ファイルを作成して保存します。 完了したら、キャプションファイルの内容をコピーしてプレーンテキストエディターに貼り付け、ファイル拡張子 VTT を付けて保存します。 <br><br><b> 注意：</b> 英語以外の言語のビデオキャプションをグローバルサポートする場合、WebVTT 標準では、サポートする言語ごとに個別の `.VTT` ファイルを作成して呼び出す必要があります。 <br><br> 通常、キャプションの VTT ファイルには、ビデオファイルと同じ名前を付けて、キャプションを追加します。 そうしておくと、既存の web コンテンツ管理システムを使用してビデオの URL を自動的に生成する際に役立ちます。 |

1. Adobe Dynamic Media Classicで、WebVTT、DFXP または SMPTE XML キャプションファイルをアップロードします。

   [&#x200B; ファイルのアップロード &#x200B;](uploading-files.md#uploading_files) を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたキャプションファイルに関連付けるビデオファイルを含むアセットフォルダーに移動します。
1. アセット参照パネルで、1 つのビデオアセットを選択し、アセットのサムネール画像の下で **[!UICONTROL プレビュー]**/ **[!UICONTROL ビューアリスト]** を選択します。
1. 「ビューアリスト」テーブルで、**Universal_HTML5_Video**、**Universal_HTML5_MixedMedia_dark** または **Universal_HTML5_MixedMedia_light** という名前のHTML5 ビューアを探し、次のいずれかの操作を行います。

   * ポップアップビデオビューアエクスペリエンスの場合は、名前の右端にある **[!UICONTROL URL をコピー]** を選択します。

     ビデオのコピー済み URL を次の構文で追加すると、キャプションファイルのコピー済み URL に関連付けることができます。

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     キャプションの URL パスの末尾に `,1` が付いていることに注意してください。 パスの VTT ファイル名拡張子の直後で、ビデオプレーヤーバーのクローズドキャプションボタンの有効と無効を任意に切り替えることができます。それには、それぞれ `1` または `0` を設定します。

   * 埋め込みビデオビューアエクスペリエンスの場合は、名前の右端にある「**[!UICONTROL 埋め込みコード]**」を選択します。

     埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

     HTML5 `Universal_HTML5_Video`、`Universal_HTML5_MixedMedia_dark` または `Universal_HTML5_MixedMedia_light` ビューアの場合は、コピーした埋め込みコードに次のコードを追加します。

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     URL パスの末尾にある `,1` に注意してください。 URL パスの VTT ファイル名拡張子の直後で、ビデオプレーヤーバーのキャプションボタンの有効と無効を任意に切り替えることができます。それぞれ、`1` または `0` を設定します。
