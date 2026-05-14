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
autotag-review: '2026-05-13T17:37:15.687Z'
TQID: 'https://experienceleague.adobe.com/7o-hO9obr6JB8sIHWQ3KTC6dRzxIBYqlOJOAbanTig0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 624
ht-degree: 22%

---

# ビデオへのチャプターマーカーの追加 {#adding-chapter-markers-to-video}

チャプターマーカーを単一のビデオまたはアダプティブビデオセットに追加することで、長編ビデオの視聴や操作を簡単にすることができます。 ユーザーがビデオを再生すると、ビデオタイムライン上のチャプターマーカー（ビデオスクラバーとも呼ばれます）を選択できます。 そうすることで、顧客は容易に自身の興味を引いた場所に移動したり、新しいコンテンツやデモ、チュートリアルなどにすぐに移動したりできます。

>[!NOTE]
>
>ビデオプレーヤーは、チャプターマーカーの使用をサポートしている必要があります。

`Universal_HTML5_Video` ビューア （HTML5）のチャプターナビゲーションキューポイントとチャプタータイトルポップアップテキストを設定する場合は、[ ビデオビューアプリセットの追加または編集](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)を参照してください。

[ ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets)も参照してください。

ビデオのチャプターリストの作成方法は、キャプションの作成方法とよく似ていて、 WebVTT ファイルを作成します。 ただし、このファイルは、使用している他の WebVTT キャプションファイルと分ける必要があります。キャプションとチャプターを 1 つの WebVTT ファイルにまとめることはできません。

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

上記の例では、`Chapter 1`はキュー識別子であり、オプションです。 `00:00:000 --> 01:04:364`のキュー時間は、00:00:000形式で、章の開始時間と終了時間を指定します。 末尾の 3 桁はミリ秒であり、必要に応じて 000 のままにすることができます。 `The bicycle store behind it all`の章タイトルは、章の内容の実際の説明です。 ビデオのタイムラインの視覚的なキューポイントにポインターを置くと、キュー識別子、開始キュー時間、章タイトルがすべてビデオプレーヤーのポップアップに表示されます。

HTML5 ビデオビューアを使用しているので、作成するチャプターファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。 章ファイル名の拡張子は`.VTT`です。 WebVTT のキャプション規格について、さらに詳しく調べることができます。

[WebVTT: Web ビデオ テキストのトラック形式](https://w3c.github.io/webvtt/)を参照してください。

**ビデオにチャプターマーカーを追加するには：**

1. Adobe Dynamic Media Classic以外のシンプルなテキストエディターを使用して、ビデオチャプターファイルを作成します。

   >[!NOTE]
   >
   >英語以外の言語でビデオチャプターをグローバルにサポートする場合、WebVTT標準では、サポートする言語ごとに`.VTT`個のファイルと呼び出しを個別に作成する必要があります。

1. VTT ファイルをUTF8 エンコーディングで保存すると、章タイトルテキストの文字レンディションに関する問題を回避できます。

   通常、チャプターVTT ファイルにビデオファイルと同じ名前を付け、`chapters`を付けて追加します。 これにより、既存のWeb コンテンツ管理システムを使用してビデオ URLの生成を自動化できます。

1. Adobe Dynamic Media Classicで、WebVTT チャプターファイルをアップロードします。

   [ ファイルのアップロード ](uploading-files.md#uploading_files)を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたチャプターファイルに関連付けるビデオファイルを含むアセットフォルダーに移動します。
1. アセット参照パネルで、1つのビデオアセットを選択し、アセットのサムネール画像の下にある「**[!UICONTROL プレビュー]**」 > 「**[!UICONTROL ビューアーリスト]**」を選択します。
1. ビューアリストの表で、**Univeral_HTML5_Video** という名前の HTML5 ビューアを探し、次のいずれかの操作を行います。

   * ポップアップビデオのビューアエクスペリエンスの場合は、名前の右端にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。

     次の構文を使用してビデオのコピーURLを追加し、コピーしたURLとキャプションファイルに関連付けることができます。

     `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 埋め込みビデオビューアエクスペリエンスの場合は、名前の右端にある「**[!UICONTROL 埋め込みコード]**」を選択します。

     埋め込みコードダイアログボックスで、**[!UICONTROL クリップボードにコピー]**&#x200B;を選択します。

     HTML5 `Universal_HTML5_Video` ビューアの場合は、コピーした埋め込みコードを次のように追加します。

     `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*"`
