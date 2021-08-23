---
title: ビデオへのチャプターマーカーの追加
description: Dynamic Media Classicでビデオにチャプターマーカーを追加する方法を説明します。
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
feature: Dynamic Media Classic，ビューア，ビデオ
role: User
exl-id: a9250841-2dba-4fdc-8a6e-91b2fecef72f
source-git-commit: 1d30c98b76ebe78ff60bae87bd112de7a577182d
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 42%

---

# ビデオへのチャプターマーカーの追加 {#adding-chapter-markers-to-video}

チャプターマーカーを単一のビデオまたはアダプティブビデオセットに追加することにより、再生時間の長いビデオの閲覧やナビゲートがしやすくなります。ユーザーがビデオを再生する際に、ビデオタイムライン上のチャプターマーカー（ビデオスクラバーとも呼ばれます）を選択できます。 これにより、ユーザーは目標地点に簡単に移動したり、新しいコンテンツ、デモ、チュートリアルなどにすぐに移動したりできます。

>[!NOTE]
>
>使用されるビデオプレーヤーがチャプターマーカーの使用に対応している必要があります。

`Universal_HTML5_Video`ビューア(HTML5)用にチャプターナビゲーションキューポイントとチャプタータイトルポップアップテキストを設定する場合は、[ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)を参照してください。

[ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets)も参照してください。

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

この例では、`Chapter 1` はキュー識別子（オプション）です。`00:00:000 --> 01:04:364`のキュー時間は、チャプターの開始時間と終了時間を00:00:000形式で指定します。 末尾の 3 桁はミリ秒であり、必要に応じて 000 のままにすることができます。チャプタータイトル`The bicycle store behind it all`は、チャプターの内容を示す実際の説明です。 ビデオのタイムライン内のビジュアルキューポイントにポインターを置くと、キュー識別子、開始キュー時間およびチャプタータイトルが、ビデオプレーヤー内にポップアップ表示されます。

HTML5 ビデオビューアを使用しているので、作成するチャプターファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。チャプターファイル名の拡張子は.VTTです。 WebVTT のキャプション規格について、さらに詳しく調べることができます。

[WebVTTを参照してください。Webビデオテキストトラックの形式](https://w3c.github.io/webvtt/)。

**ビデオにチャプターマーカーを追加するには:**

1. Dynamic Media Classicの外部で単純なテキストエディターを使用して、ビデオチャプターファイルを作成します。

   >[!NOTE]
   >
   >英語以外の言語でビデオチャプターをグローバルにサポートする場合、WebVTT標準では、サポートする言語ごとに個別の.vttファイルを作成し呼び出す必要があります。

1. VTTファイルをUTF8エンコーディングで保存して、チャプタータイトルテキストの文字レンディションに関する問題を回避できます。

   通常、チャプター VTT ファイルにはビデオファイルと同じ名前を指定し、`chapters` を付加します。これにより、既存の Web コンテンツ管理システムを使用して、ビデオ URL の生成を自動化できます。

1. Dynamic Media Classicで、WebVTTチャプターファイルをアップロードします。

   [ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたチャプターファイルに関連付けるビデオファイルを含んでいるアセットフォルダーに移動します。
1. アセットの参照パネルで1つのビデオアセットを選択し、アセットのサムネール画像の下で&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;を選択します。
1. ビューアリストの表で、**Univeral_HTML5_Video** という名前の HTML5 ビューアを探し、次のいずれかの操作を行います。

   * ポップアップビデオビューアエクスペリエンスの場合、名前の右端にある「URL ]**をコピー」を選択します。**[!UICONTROL 

      コピーしたビデオのURLを次の構文で追加し、コピーしたURLにキャプションファイルを関連付けることができます。

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 埋め込みビデオビューアエクスペリエンスの場合、名前の右端にある「**[!UICONTROL 埋め込みコード]**」を選択します。

      埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

      HTML5 `Universal_HTML5_Video`ビューアの場合、コピーした埋め込みコードを次のように追加します。

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`
