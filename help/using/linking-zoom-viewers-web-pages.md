---
title: Web ページへのZoom ビューアのリンク
description: Adobe Dynamic Media ClassicでZoom ビューアをWeb ページにリンクする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
autotag-review: '2026-05-13T20:03:57.696Z'
TQID: 'https://experienceleague.adobe.com/Urf0qGJqj7tCCGDfNwprZnxf6YfDgavWb44pThwds0I'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a39ab917e54f3c998f3542e0ff6628de720ca017
workflow-type: tm+mt
source-wordcount: 696
ht-degree: 19%

---

# Web ページへのZoom ビューアの接続{#linking-zoom-viewers-to-your-web-pages}

web サイトやアプリケーションは、URL文字列や埋め込みコードを使用して、Dynamic Media Image Serverのコンテンツにアクセスできます。 このアクセスには、プライマリ画像と関連するズームターゲットが含まれます。 また、Zoom Viewer プリセットも含まれています。 この URL 文字列は、公開処理中にアクティブになります。 これらのURL文字列または埋め込みコードをWeb ページやアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## Zoom ビューア URLのコピー {#copying-a-zoom-viewer-url}

1. 左側のアセットライブラリパネルで、コピーする URL を持つズームビューアを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;または&#x200B;**[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側の「URLと埋め込みコード」パネルで、必要なビューアの右側にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

## Web ページへのZoom ビューア URLの追加 {#adding-zoom-viewer-urls-to-your-web-page}

通常、訪問者は、最初にズームアイコンを選択することで、web ページで画像をズームします（多くの場合、アイコンには虫眼鏡の画像が表示されます）。 このアイコンを選択すると、画像をポップアップウィンドウに表示する動的なWeb ページ（ASPまたはJSP）が起動します。 ポップアップウィンドウでは、訪問者が画像をズームします。

詳細およびコードサンプルについては、『HTML ビューアリファレンスガイド』の「[Embedded Adobe5 Basic Zoom Viewer](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)」を参照してください。

## Zoom ビューアの埋め込みコピーをコピーする {#copying-the-embed-copy-of-a-zoom-viewer}

埋め込みコード機能を使用すると、選択したZoom ビューアのビューアコードを確認できます。 コードをクリップボードにコピーして、ビューアのデプロイメント用にWeb ページに貼り付けることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**Zoom ビューアの埋め込みコードをコピーするには：**

1. 左側のアセットライブラリパネルで、埋め込みコードをコピーするZoom ビューアを含むアセットフォルダーに移動します。
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
