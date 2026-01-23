---
title: Web ページへの画像セットのリンク
description: Adobe Dynamic Media Classicで画像セットを Web ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 16%

---

# Web ページへの画像セットのリンク{#linking-an-image-set-to-a-web-page}

画像セットを公開した後、関連する URL または埋め込みコードをコピーして、web サイトやアプリケーションで使用できます。 その後、必要に応じて URL をデプロイするか、埋め込みコードを貼り付けて、ユーザーが web サイトまたはアプリケーションで画像セットを表示できるようにします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## 画像セット URL をコピー {#copying-an-image-set-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL 画像セット]**」を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ画像セットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッド表示]** を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の **[!UICONTROL URL と埋め込みコード]** パネルで、必要なビューアの右側にある **[!UICONTROL URL をコピー]** を選択します。
   * **[!UICONTROL グリッド表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL リスト表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL グリッド表示]**、**[!UICONTROL リスト表示]** または **[!UICONTROL 詳細表示]** を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

## Web ページへの画像セット URL の追加 {#adding-image-set-urls-to-your-web-page}

画像セットをデプロイする最も一般的な方法は、Web ページに（ナビゲーションアイコンを介して）リンクを配置することです。 選択すると、リンクによって動的ページ（JSP）が起動され、ポップアップズームウィンドウに画像セットが表示されます。 ズームリンクをクリックすると、実際のズーム機能を含むポップアップウィンドウが開きます。

詳細とコードサンプルについては、『Adobe ビューアリファレンスガイド』の [ 埋め込みHTML5 ズームビューア ](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2) を参照してください。

## 画像セットビューアの埋め込みコードのコピー {#copying-the-embed-code-of-an-image-set-viewer}

埋め込みコード機能を使用すると、選択した画像セットのビューアコードを確認できます。 コードをクリップボードにコピーして、Web ページに貼り付け、ビューアをデプロイすることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**画像セットビューアの埋め込みコードをコピーするには：**

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL 画像セット]**」を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ画像セットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッド表示]** を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL パネルで、「**[!UICONTROL 埋め込みコード]**」を選択します。
   * **[!UICONTROL グリッド表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL リスト表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL グリッド表示]**、**リスト表示** または **詳細表示** を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

1. **[!UICONTROL 埋め込みコード]** ダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

   **[!UICONTROL 埋め込みコード]** ダイアログボックスでは、コードの編集は許可されていません。

1. **[!UICONTROL 閉じる]** を選択します。

>[!MORELIKETHIS]
>
>* [ 公開 ](publishing-files.md#publishing_files)
