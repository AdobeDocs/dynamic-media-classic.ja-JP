---
title: Web ページへの画像セットのリンク
description: 画像セットをAdobe Dynamic Media Classicの Web ページにリンクする方法を説明します。
uuid: 8153a228-b2ec-4bc2-8996-266113a83df5
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 40f4abab-9059-4d92-a761-f6d573b42e00
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 42%

---

# Web ページへの画像セットのリンク{#linking-an-image-set-to-a-web-page}

画像セットの公開後、その画像セットの URL または埋め込みコードを Web サイトやアプリケーションで使用できるようになります。次に、必要に応じてこの URL を配信するか、埋め込みコードをペーストすると、ユーザは Web サイトやアプリケーション上で画像セットを表示できます。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## 画像セット URL のコピー {#copying-an-image-set-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL 画像セット]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ画像セットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコードパネルで、 **[!UICONTROL URL をコピー]** を選択します。
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

## Web ページへの画像セットの URL の追加 {#adding-image-set-urls-to-your-web-page}

画像セットは、ナビゲーションアイコンにより Web ページにリンク表示するのが、最も一般な使用方法です。リンクをクリックすると、画像セットをポップアップズームウィンドウで表示する動的ページ (JSP) が起動します。 ズームリンクによって実際のズーム機能を備えたポップアップウィンドウが開きます。

詳細およびコードサンプルについては、 [HTMLビューアリファレンスガイドにAdobe5 ズームビューアを埋め込む](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2).

## 画像セットビューアの埋め込みコードをコピーする {#copying-the-embed-code-of-an-image-set-viewer}

埋め込みコード機能を使用すると、選択した画像セットのビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。埋め込みコードダイアログボックスでは、コードを編集することはできません。

**画像セットビューアの埋め込みコードをコピーするには:**

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL 画像セット]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ画像セットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL パネルで、「 」を選択します。 **[!UICONTROL 埋め込みコード]**.
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL グリッド表示]**, **リスト表示**&#x200B;または **詳細ビュー**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

1. 埋め込みコードダイアログボックスで、「 **[!UICONTROL クリップボードにコピー]**.

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. 選択 **[!UICONTROL 閉じる]**.

>[!MORELIKETHIS]
>
>* [公開](publishing-files.md#publishing_files)

