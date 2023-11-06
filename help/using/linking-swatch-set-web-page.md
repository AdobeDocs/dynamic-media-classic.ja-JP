---
title: Web ページへのスウォッチセットのリンク
description: Adobe Dynamic Media Classicでスウォッチセットを Web ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 8bb1c744-270a-4752-b163-443708fca6c2
topic: Content Management
level: Intermediate
source-git-commit: 597b7d6bd98c59a644984baeecb888f86a8975c9
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 33%

---

# Web ページへのスウォッチセットのリンク{#linking-a-swatch-set-to-a-web-page}

スウォッチセットを公開した後は、関連する URL を使用したり、Web サイトやアプリケーションで埋め込みコードを使用したりできます。 次に、必要に応じてこの URL または埋め込みコードを配信すると、ユーザは Web サイトやアプリケーション上でスウォッチセットを表示できます。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## スウォッチセットの URL のコピー {#copying-a-swatch-set-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL スウォッチセット]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つスウォッチセットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコードパネルで、 **[!UICONTROL URL をコピー]** を選択します。
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下で、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

## Web ページへのスウォッチセット URL の追加 {#adding-swatch-set-urls-to-your-web-page}

スウォッチセットをデプロイする最も一般的な方法は、Web ページに（ナビゲーションアイコンを使用して）リンクを配置することです。 選択すると、リンクは、スウォッチセットをポップアップズームウィンドウで表示する動的ページ（ASP または JSP）を起動します。 ズームリンクによって実際のズーム機能を備えたポップアップウィンドウが開きます。

詳細およびコードサンプルについては、 [『HTMLビューアリファレンスガイド』のAdobe5 ズームビューアの埋め込み](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## スウォッチセットビューアの埋め込みコードをコピーする {#copying-the-embed-code-of-a-swatch-set-viewer}

埋め込みコード機能を使用すると、選択したスウォッチセットのビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。埋め込みコードダイアログボックスでは、コードを編集することはできません。

**スウォッチセットビューアの埋め込みコードをコピーするには:**

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL スウォッチセット]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つスウォッチセットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコードパネルで、 **[!UICONTROL 埋め込みコード]** を選択します。
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下で、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

1. 埋め込みコードダイアログボックスで、「 **[!UICONTROL クリップボードにコピー]**.

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. 選択 **[!UICONTROL 閉じる]**.

>[!MORELIKETHIS]
>
>* [公開](publishing-files.md#publishing_files)
