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
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 38%

---

# ビデオへのチャプターマーカーの追加 {#adding-chapter-markers-to-video}

1 つのビデオまたはアダプティブビデオセットにチャプターマーカーを追加することで、長形式のビデオを見やすくし、移動しやすくすることができます。 ユーザーがビデオを再生する際に、ビデオタイムライン上のチャプターマーカー（ビデオスクラバーとも呼ばれます）を選択できます。 これにより、ユーザーは目標地点に簡単に移動したり、新しいコンテンツ、デモ、チュートリアルなどにすぐに移動したりできます。

>[!NOTE]
>
>使用されるビデオプレーヤーがチャプターマーカーの使用に対応している必要があります。

詳しくは、 [ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset) チャプターナビゲーションキューポイントとチャプタータイトルポップアップテキストを `Universal_HTML5_Video` viewer(HTML5)

関連トピック [ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets).

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

この例では、`Chapter 1` はキュー識別子（オプション）です。のキュー時間 `00:00:000 --> 01:04:364` チャプターの開始時間と終了時間を 00 で指定します。:00:000 形式。 末尾の 3 桁はミリ秒であり、必要に応じて 000 のままにすることができます。チャプタータイトル： `The bicycle store behind it all` は、チャプターの内容を示す実際の説明です。 ビデオのタイムライン内のビジュアルキューポイントにポインターを置くと、キュー識別子、開始キュー時間およびチャプタータイトルが、ビデオプレーヤー内にポップアップ表示されます。

HTML5 ビデオビューアを使用しているので、作成するチャプターファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。チャプターファイル名の拡張子は.VTT です。 WebVTT のキャプション規格について、さらに詳しく調べることができます。

詳しくは、 [WebVTT:Web Video Text Tracks Format](https://w3c.github.io/webvtt/).

**ビデオにチャプターマーカーを追加するには:**

1. Adobe Dynamic Media Classicの外部で単純なテキストエディターを使用して、ビデオチャプターファイルを作成します。

   >[!NOTE]
   >
   >英語以外の言語でビデオチャプターをグローバルにサポートする場合、WebVTT 標準では、サポートする言語ごとに個別の.vtt ファイルを作成して呼び出す必要があります。

1. VTT ファイルを UTF8 エンコーディングで保存して、チャプタータイトルテキストの文字レンディションに関する問題を回避できます。

   通常、チャプター VTT ファイルにはビデオファイルと同じ名前を指定し、`chapters` を付加します。これにより、既存の Web コンテンツ管理システムを使用して、ビデオ URL の生成を自動化できます。

1. Adobe Dynamic Media Classicで、WebVTT チャプターファイルをアップロードします。

   詳しくは、 [ファイルをアップロード](uploading-files.md#uploading_files).

1. 左側のアセットライブラリパネルで、アップロードしたチャプターファイルに関連付けるビデオファイルを含んでいるアセットフォルダーに移動します。
1. アセットの参照パネルで 1 つのビデオアセットを選択し、アセットのサムネール画像の下でを選択します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
1. ビューアリストの表で、**Univeral_HTML5_Video** という名前の HTML5 ビューアを探し、次のいずれかの操作を行います。

   * ポップアップビデオビューアエクスペリエンスの場合は、 **[!UICONTROL URL をコピー]** を名前の右端にドラッグします。

     コピーしたビデオの URL を次の構文で追加して、コピーした URL とキャプションファイルを関連付けることができます。

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 埋め込みビデオビューアエクスペリエンスの場合、 **[!UICONTROL 埋め込みコード]** を名前の右端にドラッグします。

     埋め込みコードダイアログボックスで、「 **[!UICONTROL クリップボードにコピー]**.

     HTML5 `Universal_HTML5_Video` ビューアで、コピーした埋め込みコードを次のように追加します。

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
