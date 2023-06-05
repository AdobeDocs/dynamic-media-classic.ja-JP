---
title: Web ページへのズームビューアのリンク
description: ズームビューアをAdobe Dynamic Media Classicの Web ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 34%

---

# Web ページへのズームビューアのリンク{#linking-zoom-viewers-to-your-web-pages}

Web サイトやアプリケーションは、URL 文字列または埋め込みコードを使用して、プライマリ画像や関連するズームターゲットなどのDynamic Media Image Server コンテンツやズームビューアプリセットにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。これらの URL 文字列または埋め込みコードを Web ページやアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## ズームビューアの URL のコピー {#copying-a-zoom-viewer-url}

1. 左側のアセットライブラリパネルで、コピーする URL を持つズームビューアを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]** または **[!UICONTROL リスト表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコードパネルで、 **[!UICONTROL URL をコピー]** を選択します。
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

## Web ページへのズームビューアの URL の追加 {#adding-zoom-viewer-urls-to-your-web-page}

通常、訪問者は Web サイト上の画像をズームする際に、最初にズームアイコン（多くの場合、アイコンには虫眼鏡の画像が表示されます）を選択します。 このアイコンを選択すると、ポップアップウィンドウで画像を表示する動的 Web ページ（ASP または JSP）が起動します。このポップアップウィンドウが、閲覧者が実際に画像をズームする場所となります。

詳細およびコードサンプルについては、 [HTMLビューアリファレンスガイドのAdobe5 基本ズームビューアを埋め込む](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## ズームビューアの埋め込みコピーをコピーする {#copying-the-embed-copy-of-a-zoom-viewer}

埋め込みコード機能を使用すると、選択したズームビューアのビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。埋め込みコードダイアログボックスでは、コードを編集することはできません。

**ズームビューアの埋め込みコードをコピーするには:**

1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つズームビューアを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコードパネルで、 **[!UICONTROL 埋め込みコード]** を選択します。
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

1. 埋め込みコードダイアログボックスで、「 **[!UICONTROL クリップボードにコピー]**.

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. 選択 **[!UICONTROL 閉じる]**.
