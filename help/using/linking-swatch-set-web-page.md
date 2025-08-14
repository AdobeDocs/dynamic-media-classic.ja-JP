---
title: スウォッチセットの Web ページへのリンク
description: Adobe Dynamic Media Classicでスウォッチセットを Web ページにリンクする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 8bb1c744-270a-4752-b163-443708fca6c2
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 16%

---

# スウォッチセットの Web ページへのリンク{#linking-a-swatch-set-to-a-web-page}

スウォッチセットを公開した後、関連する URL または埋め込みコードを web サイトまたはアプリケーションで使用できます。 その後、必要に応じて URL または埋め込みコードをデプロイし、ユーザーが web サイトまたはアプリケーションでスウォッチセットを表示できるようにします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## スウォッチセット URL のコピー {#copying-a-swatch-set-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL スウォッチセット]**」を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードのスウォッチセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッド表示]** を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、必要なビューアの右側にある **[!UICONTROL URL をコピー]** を選択します。
   * **[!UICONTROL グリッド表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL リスト表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL グリッド表示]**、**[!UICONTROL リスト表示]** または **[!UICONTROL 詳細表示]** を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

## Web ページへのスウォッチセット URL の追加 {#adding-swatch-set-urls-to-your-web-page}

スウォッチセットをデプロイする最も一般的な方法は、Web ページに（ナビゲーションアイコンを介して）リンクを配置することです。 選択すると、リンクによって動的ページ（ASP または JSP）が起動され、ポップアップズームウィンドウにスウォッチセットが表示されます。 ズームリンクをクリックすると、実際のズーム機能を含むポップアップウィンドウが開きます。

詳細とコードサンプルについて詳しくは、[Adobe ビューアリファレンスガイドのHTML5 ズームビューアの埋め込み ](https://experienceleague.adobe.com/ja/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) を参照してください。

## スウォッチセットビューアの埋め込みコードのコピー {#copying-the-embed-code-of-a-swatch-set-viewer}

埋め込みコード機能を使用すると、選択したスウォッチセットのビューアコードをレビューすることができます。コードをクリップボードにコピーして、Web ページに貼り付け、ビューアをデプロイすることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**スウォッチセットビューアの埋め込みコードをコピーするには：**

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL スウォッチセット]**」を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードのスウォッチセットを含むアセットフォルダーに移動します。
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

>[!MORELIKETHIS]
>
>* [ 公開 ](publishing-files.md#publishing_files)
