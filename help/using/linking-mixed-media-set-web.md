---
title: 混在メディアセットをWeb ページにリンクする
description: Adobe Dynamic Media Classicで混在メディアセットをWeb ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 76a7530c-0cc7-4a7f-bc31-2950c4946871
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:02:51.028Z'
TQID: 'https://experienceleague.adobe.com/3AeMn6W1vePdJL1PkXuy-YISRw75QUDfdkUP5V2xhEs'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 657
ht-degree: 20%

---

# 混在メディアセットをWeb ページにリンクする{#linking-a-mixed-media-set-to-a-web-page}

混在メディアセットを公開した後は、Web サイトまたはアプリケーションで使用するための関連URLを取得できます。 次に、必要に応じてURLをデプロイして、ユーザーがWeb サイトまたはアプリケーションで混在メディアセットを表示できるようにします。

## 混在メディアセットの URL の取得 {#obtain-a-mixed-media-set-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL メディアセット]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーするメディアセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL 「グリッドビュー」]**&#x200B;をクリックします。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側の「URLと埋め込みコード」パネルで、必要なビューアの右側にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。
   * **[!UICONTROL 「グリッドビュー」]**&#x200B;をクリックします。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL 「リストビュー」]**&#x200B;をクリックします。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

   * **[!UICONTROL 「グリッドビュー」]**、**[!UICONTROL 「リストビュー」]**、または&#x200B;**[!UICONTROL 「詳細ビュー」]**&#x200B;をクリックします。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL URLをコピー]**」を選択します。

## Web ページへの混在メディアセット URLの追加 {#add-mixed-media-set-urls-to-your-web-page}

混在メディアセットをデプロイする最も一般的な方法は、（ナビゲーションアイコンを介して） Web ページにリンクを配置することです。 選択すると、リンクは動的ページ（ASPまたはJSP）を起動し、Mixed Media Set ViewerにMixed Media Setが表示されます。

## 混在メディアセットビューアの埋め込みコードのコピー {#copying-the-embed-code-of-a-mixed-media-set-viewer}

埋め込みコード機能を使用すると、選択した混在メディアセットのビューアーコードを確認できます。 コードをクリップボードにコピーして、ビューアのデプロイメント用にWeb ページに貼り付けることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**混在メディアセットビューアの埋め込みコードをコピーするには：**

1. アセット参照パネルの「表示」ドロップダウンリストで、**[!UICONTROL 混在メディアセット]**&#x200B;を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーする混在メディアセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL 「グリッドビュー」]**&#x200B;をクリックします。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。 右側の「URLと埋め込みコード」パネルで、必要なビューアの右側にある「**[!UICONTROL 埋め込みコード]**」を選択します。
   * **[!UICONTROL 「グリッドビュー」]**&#x200B;をクリックします。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の下の&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

   * **[!UICONTROL 「リストビュー」]**&#x200B;をクリックします。 アセット参照パネルで、1つのアセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

   * **[!UICONTROL 「グリッドビュー」]**、**[!UICONTROL 「リストビュー」]**、または&#x200B;**[!UICONTROL 「詳細ビュー」]**&#x200B;をクリックします。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。

     ビューアーリストページのテーブルの「アクション」列で、「**[!UICONTROL コードを埋め込む]**」を選択します。

1. 埋め込みコードダイアログボックスで、**[!UICONTROL クリップボードにコピー]**&#x200B;を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. 「**[!UICONTROL 閉じる]**」をクリックします。

>[!MORELIKETHIS]
>
>* [公開](publishing-files.md#publishing_files)
