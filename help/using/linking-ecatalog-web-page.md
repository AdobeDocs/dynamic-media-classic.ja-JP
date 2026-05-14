---
title: eCatalogをWeb ページにリンクする
description: Adobe Dynamic Media ClassicでeCatalogをWeb ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:52:09.030Z'
TQID: 'https://experienceleague.adobe.com/cAIaFvlJ3jYoqu1LeLRILuuYsfvuYH6f-N8PqqkHkrk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 698
ht-degree: 20%

---

# eCatalogをWeb ページにリンクする{#linking-an-ecatalog-to-a-web-page}

Web サイトとアプリケーションは、URL文字列または埋め込みコードを使用して、e カタログを含むDynamic Media Image Server コンテンツにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。 Web ページやアプリケーションにeCatalogのURL文字列または埋め込みコードを配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## eCatalog URLのコピー {#copying-an-ecatalog-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL カタログ]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーするeCatalogを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側の「URLと埋め込みコード」パネルで、必要なビューアの右側にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**URLをコピー**」を選択します。

## Web ページへのeCatalog URLの追加 {#adding-ecatalog-urls-to-your-web-page}

eCatalogをデプロイする最も一般的な方法は、Web ページにeCatalog サムネールカバーページの形式でリンクを配置することです。 中央にきちんと表示されるポップアップウィンドウで eCatalog が起動するように、IT 部門の担当者と相談してください。 また、ブラウザ画面にツールバーやアドレスバーなどを表示しないように依頼してください。

詳細およびコードサンプルについては、「Adobe ビューアリファレンス」の「[Embedded HTML5 eCatalog Viewer](https://experienceleague.adobe.com/ja/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)」を参照してください。

## eCatalog ビューアの埋め込みコードのコピー {#copying-the-embed-code-of-an-ecatalog-viewer}

埋め込みコード機能を使用すると、選択したeCatalogのビューアコードを確認できます。 コードをクリップボードにコピーして、ビューアのデプロイメント用にWeb ページに貼り付けることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**eCatalog ビューアの埋め込みコードをコピーするには：**

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL カタログ]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーするeCatalogを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側のURL パネルで、**[!UICONTROL 埋め込みコード]**&#x200B;を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

1. 埋め込みコードダイアログボックスで、**[!UICONTROL クリップボードにコピー]**&#x200B;を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. **[!UICONTROL 閉じる]**&#x200B;を選択します。
