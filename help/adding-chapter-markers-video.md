---
title: ビデオへのチャプターマーカーの追加
seo-title: ビデオへのチャプターマーカーの追加
description: 'null'
seo-description: ビデオにチャプターマーカーを追加する方法を説明します。
uuid: 4e1e6daf-afc6-49d9-ac90-183fe2a903b2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 8bc5e552-2abb-41f0-89d2-bdf3ae5d96c2
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 88%

---


# ビデオへのチャプターマーカーの追加{#adding-chapter-markers-to-video}

チャプターマーカーを単一のビデオまたはアダプティブビデオセットに追加することにより、再生時間の長いビデオの閲覧やナビゲートがしやすくなります。ユーザーがビデオを再生するとき、ビデオタイムライン（ビデオスクラバーとも呼ばれる）のチャプターマーカーをクリックすれば、関心のあるポイントに簡単にナビゲートできます。また、新しいコンテンツ、デモ、チュートリアルなどにすぐにアクセスできます。

>[!NOTE]
>
>使用されるビデオプレーヤーがチャプターマーカーの使用に対応している必要があります。

[ ビューア（HTML5）でのチャプターナビゲーションキューポイントやチャプタータイトルポップアップテキストの設定方法については、](previewing-videos-video-viewer.md#adding_or_editing_a_video_viewer_preset)ビデオビューアプリセットの追加または編集`Universal_HTML5_Video`を参照してください。

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

この例では、`Chapter 1` はキュー識別子（オプション）です。`00:00:000 --> 01:04:364` というキュー時間では、そのチャプターの開始時間と終了時間を「00:00:000」という形式で指定しています。末尾の 3 桁はミリ秒であり、必要に応じて 000 のままにすることができます。The chapter title of `The bicycle store behind it all` is the actual description of the chapter’s contents. キュー識別子、開始キュー時間およびチャプタータイトルはすべて、ビデオプレーヤーでユーザーがビデオのタイムライン内の視覚的なキューポイントにマウスポインターを置いたときにポップアップ表示されます。

HTML5 ビデオビューアを使用しているので、作成するチャプターファイルが WebVTT（Web Video Text Tracks）規格に従っていることを確認してください。チャプターのファイル名拡張子は .vtt です。WebVTT のキャプション規格について、さらに詳しく調べることができます。

See [WebVTT: The Web Video Text Tracks format](https://dev.w3.org/html5/webvtt/).

**ビデオにチャプターマーカーを追加するには**

1. Dynamic Media Classicの外部でシンプルなテキストエディターを使用して、ビデオチャプターファイルを作成します。

   >[!NOTE]
   >
   >英語以外の言語のビデオチャプターをグローバルサポートする場合、WebVTT 規格では、サポートする言語ごとに個別の .vtt ファイルを作成して呼び出す必要があることに注意してください。

1. チャプタータイトルテキストの文字レンダリングの問題を回避するために、.vtt ファイルを UTF8 エンコーディングで保存します。

   通常、チャプター VTT ファイルにはビデオファイルと同じ名前を指定し、`chapters` を付加します。これにより、既存の Web コンテンツ管理システムを使用して、ビデオ URL の生成を自動化できます。

1. Dynamic Media Classicで、WebVTTチャプターファイルをアップロードします。

   詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

1. 左側のアセットライブラリパネルで、アップロードしたチャプターファイルに関連付けるビデオファイルを含んでいるアセットフォルダーに移動します。
1. アセットの参照パネルで 1 つのビデオアセットを選択して、アセットのサムネール画像の下にある&#x200B;**[!UICONTROL プレビュー]**／**[!UICONTROL ビューアリスト]**&#x200B;をクリックします。
1. ビューアリストの表で、**Univeral_HTML5_Video** という名前の HTML5 ビューアを探し、次のいずれかの操作を行います。

   * ポップアップビデオビューアの操作については、名前の最も右側にある&#x200B;**[!UICONTROL 「URL をコピー」]**&#x200B;をクリックします。

      コピーしたビデオの URL を次の構文と共に追加し、この URL とコピーしたキャプションファイルの URL を関連付けます。

      `&navigation=*<full Copy URL path to the chapter navigation file .vtt>*`

   * 埋め込まれたビデオビューアの操作については、名前の最も右側にある&#x200B;**[!UICONTROL 「埋め込みコード」]**&#x200B;をクリックします。

      埋め込みコードダイアログボックスで、**[!UICONTROL 「クリップボードにコピー」]**&#x200B;をクリックします。

      For the HTML5 `Universal_HTML5_Video` viewer, append the copied embed code with the following:

      `videoViewer.setParam("navigation","*<full Copy URL path to the chapter navigation file .vtt>*”`

