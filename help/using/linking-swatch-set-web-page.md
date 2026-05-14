---
title: スウォッチセットをWeb ページにリンクする
description: Adobe Dynamic Media ClassicでスウォッチセットをWeb ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 8bb1c744-270a-4752-b163-443708fca6c2
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:03:11.713Z'
TQID: 'https://experienceleague.adobe.com/OhGE3-jniPFknPmpVykZWWSKo2jwdef2sA3Yqo5WpWw'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 710
ht-degree: 16%

---

# スウォッチセットをWeb ページにリンクする{#linking-a-swatch-set-to-a-web-page}

スウォッチセットを公開した後、関連するURLまたは埋め込みコードをWeb サイトまたはアプリケーションで使用できます。 次に、必要に応じてURLまたは埋め込みコードをデプロイして、ユーザーがWeb サイトまたはアプリケーションでスウォッチセットを表示できるようにします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## スウォッチセット URLのコピー {#copying-a-swatch-set-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL スウォッチセット]**」を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードのスウォッチセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側の「URLと埋め込みコード」パネルで、必要なビューアの右側にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

## Web ページへのスウォッチセット URLの追加 {#adding-swatch-set-urls-to-your-web-page}

スウォッチセットをデプロイする最も一般的な方法は、（ナビゲーションアイコンを使用して） Web ページにリンクを配置することです。 選択すると、リンクは動的ページ（ASPまたはJSP）を起動し、ポップアップズームウィンドウにスウォッチセットが表示されます。 ズームリンクによって実際のズーム機能を備えたポップアップウィンドウが開きます。

詳細およびコードサンプルについては、Adobe ビューアリファレンスガイド ](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)の「[HTML5 Zoom Viewerの埋め込み」を参照してください。

## スウォッチセットビューアの埋め込みコードのコピー {#copying-the-embed-code-of-a-swatch-set-viewer}

埋め込みコード機能を使用すると、選択したスウォッチセットのビューアコードを確認できます。 コードをクリップボードにコピーして、ビューアのデプロイメント用にWeb ページに貼り付けることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**スウォッチセットビューアの埋め込みコードをコピーするには：**

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL スウォッチセット]**」を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードのスウォッチセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側の「URLと埋め込みコード」パネルで、必要なビューアの右側にある「**[!UICONTROL 埋め込みコード]**」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

1. 埋め込みコードダイアログボックスで、**[!UICONTROL クリップボードにコピー]**&#x200B;を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. **[!UICONTROL 閉じる]**&#x200B;を選択します。

>[!MORELIKETHIS]
>
>* [公開](publishing-files.md#publishing_files)
