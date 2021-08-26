---
title: WebページへのeCatalogのリンク
description: Dynamic Media ClassicでeCatalogをWebページにリンクする方法について説明します。Adobe
uuid: 90098a90-180b-477a-8533-24a52a93200b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 140640f2-3ca4-4b6c-a240-5f01be87fa9c
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: aee72576-1e3e-401c-953d-cc2be27f7dfd
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 38%

---

# WebページへのeCatalogのリンク{#linking-an-ecatalog-to-a-web-page}

Webサイトやアプリケーションは、URL文字列や埋め込みコードを使用して、eCatalogを含むDynamic Media Image Serverコンテンツにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。eCatalogのURL文字列または埋め込みコードをWebページやアプリケーションに配置するには、AdobeDynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## eCatalogのURLのコピー {#copying-an-ecatalog-url}

1. アセットの参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL カタログ]**」を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ eCatalog を含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側のURLと埋め込みコードパネルで、目的のビューアの右側にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の下にある「**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]**」に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL 

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の右側にある&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL 

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細ビュー]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** /**[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;**」を選択します。**

## WebページへのeCatalog URLの追加 {#adding-ecatalog-urls-to-your-web-page}

eCatalog にアクセスする方法としてよく使われるのは、eCatalog の表紙のサムネールを Web ページにリンクとして貼り付ける方法です。中央にきちんと表示されるポップアップウィンドウで eCatalog が起動するように、IT 部門の担当者と相談してください。また、ブラウザ画面にツールバーやアドレスバーなどを表示しないように依頼してください。

詳細とコードサンプルについては、『Adobeビューアリファレンスガイド』の[HTML5 eCatalogビューアの埋め込み](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/ecatalog/c-html5-20-ecatalog-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2)を参照してください。

## eCatalogビューアの埋め込みコードをコピーする {#copying-the-embed-code-of-an-ecatalog-viewer}

埋め込みコード機能を使用すると、選択した eCatalog のビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。埋め込みコードダイアログボックスでは、コードの編集はできません。

**eCatalog ビューアの埋め込みコードをコピーするには:**

1. アセットの参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL カタログ]**」を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ eCatalog を含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側のURLパネルで、「**[!UICONTROL 埋め込みコード]**」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の下にある「**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]**」に移動します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の右側にある&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細ビュー]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** /**[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

1. 埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. **[!UICONTROL 閉じる]**&#x200B;を選択します。
