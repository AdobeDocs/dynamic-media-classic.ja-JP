---
title: ビデオへのチャプターマーカーの追加
description: Adobe Dynamic Media Classicでビデオにチャプターマーカーを追加する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 24%

---

# ビデオへのチャプターマーカーの追加 {#adding-chapter-markers-to-video}

1 つのビデオまたはアダプティブビデオセットにチャプターマーカーを追加すると、長編ビデオの視聴と操作が容易になります。 ビデオの再生中に、ビデオタイムライン（ビデオスクラバーとも呼ばれる）のチャプターマーカーを選択することができます。 これにより、ユーザーは、関心のあるポイントや、新しいコンテンツ、デモ、チュートリアルなどにすぐに移動できます。

>[!NOTE]
>
>使用されるビデオプレーヤーがチャプターマーカーの使用に対応している必要があります。

ビデオビューア（HTML5）のチャプターナビゲーションキューポイントおよびチャプタータイトルポップアップテキストを設定する場合は、[`Universal_HTML5_Video` デオビューアプリセットを追加または編集 ](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) を参照してください。

[ ビューアプリセットの追加と編集 ](application-setup.md#adding_and_editing_viewer_presets) も参照してください。

ビデオのチャプターリストの作成方法は、キャプションの作成方法とよく似ていて、WebVTT ファイルを作成します。ただし、このファイルは、使用している他の WebVTT キャプションファイルと分ける必要があります。キャプションとチャプターを 1 つの WebVTT ファイルにまとめることはできません。

チャプターナビゲーションを含む WebVTT ファイルを作成する際には、次のサンプルをフォーマット例として使用できます。

```as3
WEBVTT 
Chapter 1 
00:00.000 --> 01:04.364 
The bicycle store behind it all. 
Chapter 2 
01:04.364 --> 02:00.944 
Creative Cloud. 
Chapter 3 
02:00.944 --> 03:02.937 
Ease of management for a working solution. 
Chapter 4 
03:02.937 --> 03:35.000 
Cost-efficient access to rapidly evolving technology.
```

上記の例では、`Chapter 1` はキュー識別子で、オプションです。 `00:00:000 --> 01:04:364` のキュー時間は、チャプターの開始時間と終了時間を 00:00:000 形式で指定します。 末尾の 3 桁はミリ秒であり、必要に応じて 000 のままにすることができます。`The bicycle store behind it all` のチャプタータイトルは、チャプターの内容を示す実際の説明です。 ビデオのタイムラインのビジュアルキューポイントにポインターを置くと、キュー識別子、開始キュー時間およびチャプタータイトルが、ビデオプレーヤー内にポップアップ表示されます。

HTML5 ビデオビューアを使用しているので、作成するチャプターファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。チャプターファイルの拡張子は `.VTT` です。 WebVTT のキャプション規格について、さらに詳しく調べることができます。

[WebVTT:Web ビデオテキストで形式を追跡 ](https://w3c.github.io/webvtt/) を参照してください。

**ビデオにチャプターマーカーを追加するには：**

1. Adobe Dynamic Media Classicの外部にある単純なテキストエディターを使用して、ビデオチャプターファイルを作成します。

   >[!NOTE]
   >
   >英語以外の言語のビデオチャプターをグローバルサポートする場合、WebVTT 標準では、サポートする言語ごとに個別の `.VTT` ファイルを作成して呼び出す必要があります。

1. この VTT ファイルを UTF8 エンコーディングで保存して、チャプタータイトルテキストの文字レンディションに関する問題を回避します。

   一般に、チャプター VTT ファイルの名前には、ビデオファイルと同じ名前を付けて、名前の末尾に `chapters` を追加します。 そうしておくと、既存の web コンテンツ管理システムを使用してビデオの URL を自動的に生成する際に役立ちます。

1. Adobe Dynamic Media Classicで、WebVTT チャプターファイルをアップロードします。

   [ ファイルのアップロード ](uploading-files.md#uploading_files) を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたチャプターファイルに関連付けるビデオファイルを含むアセットフォルダーに移動します。
1. アセット参照パネルで、1 つのビデオアセットを選択し、アセットのサムネール画像の下で **[!UICONTROL プレビュー]**/ **[!UICONTROL ビューアリスト]** を選択します。
1. ビューアリストの表で、**Univeral_HTML5_Video** という名前の HTML5 ビューアを探し、次のいずれかの操作を行います。

   * ポップアップビデオビューアエクスペリエンスの場合は、名前の右端にある **[!UICONTROL URL をコピー]** を選択します。

     ビデオのコピー済み URL を次の構文で追加すると、キャプションファイルのコピー済み URL に関連付けることができます。

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 埋め込みビデオビューアエクスペリエンスの場合は、名前の右端にある「**[!UICONTROL 埋め込みコード]**」を選択します。

     埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

     HTML 5 `Universal_HTML5_Video` ビューアの場合は、コピーした埋め込みコードに次のコードを追加します。

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
