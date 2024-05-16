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
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 17%

---

# ビデオへのキャプションの追加 {#add-captions-to-video}

ビデオの提供範囲をグローバル市場に拡大する。 そのためには、1 つのビデオまたはアダプティブビデオセットにキャプションを追加します。 キャプションを追加することで、オーディオをダビングする必要がなくなります。また、異なる言語ごとにオーディオを再度録音する必要もなくなります。ビデオは録画されたときの言語で再生されます。外国語のサブタイトルが表示されるため、異なる言語のユーザもオーディオ部分を理解できます。

また、キャプションにより、耳の不自由なユーザや難聴者向けにクローズドキャプションを使用することで、高いアクセス性が可能になります。

>[!NOTE]
>
>使用されるビデオプレーヤーがキャプションの表示に対応している必要があります。

次のいずれかのビューアでキャプション効果を設定し、メニューのテキストを含むキャプションメニュー自体を編集するには：

* `Universal_HTML5_Video` ビューア
* `Universal_HTML5_MixedMedia_dark` ビューア
* `Universal_HTML5_MixedMedia_light` ビューア

参照： [ビデオビューアプリセットを追加または編集する](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset).

関連トピック [ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets).

Adobe Dynamic Media Classicでは、キャプションファイルを JSON （JavaScript Object Notation）形式に変換できます。 このように変換できるので、JSON テキストを、ビデオの完全なトランスクリプトとして表示せずに web ページに埋め込むことができます。 その後、検索エンジンがコンテンツをクロールしてインデックスを作成します。これにより、ビデオを見つけやすくなるとともに、ビデオコンテンツの詳細がユーザーに提供されます。

参照： [静的（画像以外）コンテンツを提供する](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/c-serving-static-nonimage-contents#image-serving-api) URL で JSON 関数を使用する方法について詳しくは、を参照してください。

**ビデオにキャプションを追加するには：**

1. Adobe Dynamic Media Classic以外のサードパーティアプリケーションを使用して、使用しているビューアのタイプに基づいてビデオキャプションファイルを作成します。

   | ビューアタイプ | キャプションファイル |
   |--- |--- |
   | HTML5 | HTML5 ビデオビューアを使用している場合、作成するキャプションファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。キャプションファイルの拡張子は `.VTT`. WebVTT のキャプション規格について、さらに詳しく調べることができます。<br><br>[WebVTT を参照](https://w3c.github.io/webvtt/):Web ビデオのテキストで形式をトラッキングします。 <br><br>WebVTT キャプションファイルの作成に使用できる、無料および有料のツールやサービスを提供する web サイトは多数あります。 <br><br>画面に表示されるサイトの指示に従って、WebVTT ファイルを作成して保存します。 完了したら、キャプションファイルの内容をコピーしてプレーンテキストエディターに貼り付け、ファイル拡張子 VTT を付けて保存します。 <br><br><b>注意：</b> 英語以外の言語のビデオキャプションをグローバルサポートする場合、WebVTT 標準では個別に作成する必要があります `.VTT` サポート対象の各言語のファイルと呼び出し。 <br><br>一般に、キャプションの VTT ファイルには、ビデオファイルと同じ名前を付けて、名前の末尾にキャプションを追加します。 そうしておくと、既存の web コンテンツ管理システムを使用してビデオの URL を自動的に生成する際に役立ちます。 |

1. Adobe Dynamic Media Classicで、WebVTT、DFXP または SMPTE XML キャプションファイルをアップロードします。

   参照： [ファイルをアップロード](uploading-files.md#uploading_files).

1. 左側のアセットライブラリパネルで、アップロードしたキャプションファイルに関連付けるビデオファイルを含むアセットフォルダーに移動します。
1. アセット参照パネルで、1 つのビデオアセットを選択し、アセットのサムネール画像の下でを選択します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
1. ビューアリストテーブルで、という名前のHTML 5 ビューアを探します。 **Univeral_HTML5_ビデオ**, **HTML Universal_Media5_MixedMedia_dark**、または **HTML Universal_Media5_MixedMedia_light**&#x200B;次のいずれかの操作を行います。

   * ポップアップビデオビューアエクスペリエンスの場合は、次を選択します。 **[!UICONTROL URL をコピー]** 名前の右端。

     ビデオのコピー済み URL を次の構文で追加すると、キャプションファイルのコピー済み URL に関連付けることができます。

     `&caption=<full Copy URL path to the caption file .vtt>,1`

     「」に注目してください `,1` キャプション URL パスの末尾に追加されます。 パスの VTT ファイル名拡張子の直後で、ビデオプレーヤーバーのクローズドキャプションボタンの有効/無効を任意に切り替えることができます。それには、を設定します。 `1` または `0`、それぞれ。

   * 埋め込みビデオビューアエクスペリエンスの場合は、を選択します。 **[!UICONTROL 埋め込みコード]** 名前の右端。

     埋め込みコード ダイアログボックスで、を選択します。 **[!UICONTROL クリップボードにコピー]**.

     HTMLの場合 5 `Universal_HTML5_Video`, `Universal_HTML5_MixedMedia_dark`、または `Universal_HTML5_MixedMedia_light` ビューアの場合、コピーした埋め込みコードに以下を追加します。

     `videoViewer.setParam("caption","<full Copy URL path to the caption file .vtt>,1"`

     「」に注目してください `,1` URL パスの末尾に配置されます。 URL パスの VTT ファイル名拡張子の直後で、ビデオプレーヤーバーのキャプションボタンの有効/無効を任意に切り替えることができます。それには、を設定します。 `1` または `0`、それぞれ。
