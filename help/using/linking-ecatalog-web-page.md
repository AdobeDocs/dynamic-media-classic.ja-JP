---
title: eCatalog を Web ページにリンクする
description: eCatalog をAdobe Dynamic Media Classicの Web ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
topic: Integrations, Development
level: Experienced
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '672'
ht-degree: 38%

---

# eCatalog を Web ページにリンクする{#linking-an-ecatalog-to-a-web-page}

Web サイトやアプリケーションは、URL 文字列または埋め込みコードを使用して、eCatalog を含むDynamic Media Image Server コンテンツにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。eCatalog の URL 文字列または埋め込みコードを Web ページやアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## eCatalog の URL をコピーする {#copying-an-ecatalog-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL カタログ]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ eCatalog を含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコードパネルで、 **[!UICONTROL URL をコピー]** を選択します。
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下で、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **URL をコピー**.

## Web ページへの eCatalog URL の追加 {#adding-ecatalog-urls-to-your-web-page}

eCatalog にアクセスする方法としてよく使われるのは、eCatalog の表紙のサムネールを Web ページにリンクとして貼り付ける方法です。中央にきちんと表示されるポップアップウィンドウで eCatalog が起動するように、IT 部門の担当者と相談してください。また、ブラウザ画面にツールバーやアドレスバーなどを表示しないように依頼してください。

詳細およびコードサンプルについては、 [HTMLビューアリファレンスガイドのAdobe5 eCatalog ビューアを埋め込む](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2).

## eCatalog ビューアの埋め込みコードをコピーする {#copying-the-embed-code-of-an-ecatalog-viewer}

埋め込みコード機能を使用すると、選択した eCatalog のビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。埋め込みコードダイアログボックスでは、コードを編集することはできません。

**eCatalog ビューアの埋め込みコードをコピーするには：**

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL カタログ]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ eCatalog を含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL パネルで、「 」を選択します。 **[!UICONTROL 埋め込みコード]**.
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下で、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

1. 埋め込みコードダイアログボックスで、「 **[!UICONTROL クリップボードにコピー]**.

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. 選択 **[!UICONTROL 閉じる]**.
