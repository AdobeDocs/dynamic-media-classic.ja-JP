---
title: Web ページへの eCatalog のリンク
description: Adobe Dynamic Media Classicで eCatalog を web ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 23%

---

# Web ページへの eCatalog のリンク{#linking-an-ecatalog-to-a-web-page}

Web サイトおよびアプリケーションは、URL 文字列または埋め込みコードを介して、eCatalog を含むDynamic Media Image Server コンテンツにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。Web ページやアプリケーションに eCatalog の URL 文字列または埋め込みコードを配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## eCatalog URL をコピー {#copying-an-ecatalog-url}

1. アセットの参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL カタログ]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーする eCatalog を含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッド表示]** を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、必要なビューアの右側にある **[!UICONTROL URL をコピー]** を選択します。
   * **[!UICONTROL グリッド表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL リスト表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL グリッド表示]**、**[!UICONTROL リスト表示]** または **[!UICONTROL 詳細表示]** を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**URL をコピー**」を選択します。

## Web ページへの eCatalog URL の追加 {#adding-ecatalog-urls-to-your-web-page}

eCatalog をデプロイする最も一般的な方法は、web ページに eCatalog のサムネールのカバーページの形式でリンクを配置することです。 中央にきちんと表示されるポップアップウィンドウで eCatalog が起動するように、IT 部門の担当者と相談してください。また、ブラウザ画面にツールバーやアドレスバーなどを表示しないように依頼してください。

詳細とコードサンプルについては、[AdobeビューアリファレンスガイドのHTML5 eCatalog ビューアの埋め込み ](https://experienceleague.adobe.com/ja/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) を参照してください。

## eCatalog ビューアの埋め込みコードのコピー {#copying-the-embed-code-of-an-ecatalog-viewer}

埋め込みコード機能を使用すると、選択した eCatalog のビューアコードをレビューすることができます。コードをクリップボードにコピーして、Web ページに貼り付け、ビューアをデプロイすることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**eCatalog ビューアの埋め込みコードをコピーするには：**

1. アセットの参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL カタログ]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーする eCatalog を含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッド表示]** を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL パネルで、「**[!UICONTROL 埋め込みコード]**」を選択します。
   * **[!UICONTROL グリッド表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL リスト表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL グリッド表示]**、**[!UICONTROL リスト表示]** または **[!UICONTROL 詳細表示]** を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

1. 埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. **[!UICONTROL 閉じる]** を選択します。
