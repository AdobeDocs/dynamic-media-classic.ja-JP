---
title: Web ページへのズームビューアのリンク
description: Adobe Dynamic Media Classicでズームビューアを web ページにリンクする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 21%

---

# Web ページへのズームビューアのリンク{#linking-zoom-viewers-to-your-web-pages}

Web サイトおよびアプリケーションは、URL 文字列または埋め込みコードを介して Dynamic Media Image Server コンテンツにアクセスします。 このアクセスには、プライマリ画像と関連するズームターゲットが含まれます。 また、ズームビューアプリセットも含まれています。 この URL 文字列は、公開処理中にアクティブになります。これらの URL 文字列または埋め込みコードを web ページおよびアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## ズームビューア URL のコピー {#copying-a-zoom-viewer-url}

1. 左側のアセットライブラリパネルで、コピーする URL を持つズームビューアを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッド表示]** または **[!UICONTROL リスト表示]** を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、必要なビューアの右側にある **[!UICONTROL URL をコピー]** を選択します。
   * **[!UICONTROL グリッド表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL リスト表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL グリッド表示]**、**[!UICONTROL リスト表示]** または **[!UICONTROL 詳細表示]** を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

## Web ページへのズームビューア URL の追加 {#adding-zoom-viewer-urls-to-your-web-page}

通常、訪問者は、最初にズームアイコン（多くの場合、アイコンは虫眼鏡の画像を表示）を選択して、web サイト上で画像をズームします。 このアイコンを選択すると、動的な web ページ（ASP または JSP）が起動し、ポップアップウィンドウに画像が表示されます。 このポップアップウィンドウが、閲覧者が実際に画像をズームする場所となります。

詳細とコードサンプルについては、『Adobe ビューアリファレンスガイド』の [&#x200B; 埋め込みHTML5 基本ズームビューア &#x200B;](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) を参照してください。

## ズームビューアの埋め込みコピーのコピー {#copying-the-embed-copy-of-a-zoom-viewer}

埋め込みコード機能を使用すると、選択したズームビューアのビューアコードを確認できます。 コードをクリップボードにコピーして、Web ページに貼り付け、ビューアをデプロイすることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**ズームビューアの埋め込みコードをコピーするには：**

1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つズームビューアを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッド表示]** を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、目的とするビューアの右側にある **[!UICONTROL 埋め込みコード]** を選択します。
   * **[!UICONTROL グリッド表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL リスト表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL グリッド表示]**、**[!UICONTROL リスト表示]** または **[!UICONTROL 詳細表示]** を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

1. 埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. **[!UICONTROL 閉じる]** を選択します。
