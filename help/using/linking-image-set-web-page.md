---
title: Web ページへの画像セットのリンク
description: Adobe Dynamic Media Classicで画像セットをWeb ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: df4e5218-2a66-413c-b247-b2a16d884041
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:02:41.296Z'
TQID: 'https://experienceleague.adobe.com/d1hGtQAgf1wwjIAbeRJ-kQW4kfglXNu5VSIGxRTgxnc'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 703
ht-degree: 18%

---

# Web ページへの画像セットのリンク{#linking-an-image-set-to-a-web-page}

画像セットを公開したら、関連するURLまたはその埋め込みコードをコピーして、Web サイトまたはアプリケーションで使用できます。 次に、必要に応じてURLをデプロイするか、埋め込まれたコードを貼り付けて、ユーザーがWeb サイトまたはアプリケーションで画像セットを表示できるようにします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## 画像セット URLをコピー {#copying-an-image-set-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、**[!UICONTROL 画像セット]**&#x200B;を選択します。
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つ画像セットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側の&#x200B;**[!UICONTROL URLと埋め込みコード]** パネルで、必要なビューアの右側にある&#x200B;**[!UICONTROL URL]**&#x200B;をコピーを選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

## Web ページへの画像セット URLの追加 {#adding-image-set-urls-to-your-web-page}

画像セットをデプロイする最も一般的な方法は、（ナビゲーションアイコンを使用して） Web ページにリンクを配置することです。 選択すると、リンクは動的ページ（JSP）を起動し、画像セットをポップアップズームウィンドウに表示します。 ズームリンクによって実際のズーム機能を備えたポップアップウィンドウが開きます。

詳細およびコードサンプルについては、『HTML ビューアリファレンスガイド』の「[埋め込みAdobe5 Zoom Viewer](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/zoom/c-html5-20-zoom-viewer-about#section-e1c3106f5b3e445d9b95be337c2f94e2)」を参照してください。

## 画像セットビューアの埋め込みコードのコピー {#copying-the-embed-code-of-an-image-set-viewer}

埋め込みコード機能を使用すると、選択した画像セットのビューアコードを確認できます。 コードをクリップボードにコピーして、ビューアのデプロイメント用にWeb ページに貼り付けることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**画像セットビューアの埋め込みコードをコピーするには：**

1. アセット参照パネルの「表示」ドロップダウンリストで、**[!UICONTROL 画像セット]**&#x200B;を選択します。
1. 左側のアセットライブラリパネルで、埋め込まれたコードをコピーする画像セットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側のURL パネルで、**[!UICONTROL 埋め込みコード]**&#x200B;を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**リストビュー**、または&#x200B;**詳細表示**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

1. **[!UICONTROL 埋め込みコード]** ダイアログボックスで、**[!UICONTROL クリップボードにコピー]**&#x200B;を選択します。

   コードの編集は、**[!UICONTROL 埋め込みコード]** ダイアログボックスでは許可されていません。

1. **[!UICONTROL 閉じる]**&#x200B;を選択します。

>[!MORELIKETHIS]
>
>* [公開](publishing-files.md#publishing_files)
