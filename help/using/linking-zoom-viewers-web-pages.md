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
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 23%

---

# Web ページへのズームビューアのリンク{#linking-zoom-viewers-to-your-web-pages}

Web サイトおよびアプリケーションは、URL 文字列または埋め込みコードを介してDynamic Media Image Server コンテンツにアクセスします。 このアクセスには、プライマリ画像と関連するズームターゲットが含まれます。 また、ズームビューアプリセットも含まれています。 この URL 文字列は、公開処理中にアクティブになります。これらの URL 文字列または埋め込みコードを web ページおよびアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## ズームビューア URL のコピー {#copying-a-zoom-viewer-url}

1. 左側のアセットライブラリパネルで、コピーする URL を持つズームビューアを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * を選択 **[!UICONTROL グリッド表示]** または **[!UICONTROL リスト表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、を選択します。 **[!UICONTROL URL をコピー]** をビューアの右側にクリックします。
   * を選択 **[!UICONTROL グリッド表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の下のに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**.

   * を選択 **[!UICONTROL リスト表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の右側で、 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**.

   * を選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**、または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**.

## Web ページへのズームビューア URL の追加 {#adding-zoom-viewer-urls-to-your-web-page}

通常、訪問者は、最初にズームアイコン（多くの場合、アイコンは虫眼鏡の画像を表示）を選択して、web サイト上で画像をズームします。 このアイコンを選択すると、動的な web ページ（ASP または JSP）が起動し、ポップアップウィンドウに画像が表示されます。 このポップアップウィンドウが、閲覧者が実際に画像をズームする場所となります。

詳細とコードサンプルについては、を参照してください。 [HTMLビューアリファレンスガイドのAdobe5 基本ズームビューアの埋め込み](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## ズームビューアの埋め込みコピーのコピー {#copying-the-embed-copy-of-a-zoom-viewer}

埋め込みコード機能を使用すると、選択したズームビューアのビューアコードをレビューすることができます。コードをクリップボードにコピーして、Web ページに貼り付け、ビューアをデプロイすることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**ズームビューアの埋め込みコードをコピーするには：**

1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つズームビューアを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * を選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、を選択します。 **[!UICONTROL 埋め込みコード]** をビューアの右側にクリックします。
   * を選択 **[!UICONTROL グリッド表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の下のに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**.

   * を選択 **[!UICONTROL リスト表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の右側で、 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**.

   * を選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**、または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**.

1. 埋め込みコード ダイアログボックスで、を選択します。 **[!UICONTROL クリップボードにコピー]**.

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. を選択 **[!UICONTROL 閉じる]**.
