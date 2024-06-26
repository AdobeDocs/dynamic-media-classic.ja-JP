---
title: アセットのプレビュー
description: Adobe Dynamic Media Classicでアセットをプレビューする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Viewers
role: User
exl-id: 7e6f652c-b197-4171-b11b-f532795f7cf2
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 12%

---

# アセットのプレビュー{#previewing-an-asset}

プレビューを使用して、デジタルアセットがユーザーに表示されたときにどのように表示されるかを確認できます。 プレビューでは、アセットに割り当てられている初期設定ビューアが使用されます。初期設定ビューアは、アプリケーション設定で設定します。

参照： [デフォルトビューアを設定](application-setup.md#configuring_default_viewers).

パラメーターレイヤーを含むテンプレートアセットをプレビューしている場合は、パラメーターを変更したり、画像プリセットを変更したりできます。 変更はインラインで行われるため、同じプレビューウィンドウに直ちに結果が表示されます。

関連トピック [Adobeビューアリファレンスライブラリの例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

**アセットをプレビューするには：**

1. 左側のアセットライブラリパネルで、プレビューするアセットを含むアセットフォルダーに移動します。
1. 次のいずれかの操作を行います。

   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL グリッド表示]**.
   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL リスト表示]**.
   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL 詳細ビュー]**.

1. 使用しているビューに応じて、次のいずれかの操作を行います。

   * グリッド表示またはリスト表示のアセットウィンドウで、1 つのアセットを選択してから、を選択します **[!UICONTROL プレビュー]** サムネール画像の近く。
   * グリッド表示、リスト表示または詳細表示の Assets ウィンドウの上にあるツールバーで、を選択します。 **[!UICONTROL プレビュー]**.

## ビューアプラットフォームタイプに基づいたアセットのプレビュー {#previewing-an-asset-based-on-viewer-platform-type}

ビューアリストを使用して、HTML 5 などの特定のビューアプラットフォームタイプでのアセットの表示方法をプレビューできます。 アセットタイプとプレビューのために選択した関連ビューアによっては、ビューアリストで使用できないプラットフォームがあります。

また、ビューアリストを使用して、ビューアの URL をコピーしたり、Web ページに埋め込むビューアコードを表示してコピーしたりすることもできます。

特定のビューアプラットフォームの場合、ビューアリストウィンドウを使用すると、ビューアで使用可能なデバイス（タブレットやスマートフォンなど）を視覚的に確認できます。

**ビューアプラットフォームタイプに基づいてアセットをプレビューするには：**

1. 左側のアセットライブラリパネルで、プレビューするアセットを含むアセットフォルダーに移動します。
1. 次のいずれかの操作を行います。

   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL グリッド表示]**. アセットウィンドウで 1 つのアセットを選択し、サムネール画像の下の「」に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL リスト表示]**. アセットウィンドウで 1 つのアセットを選択し、サムネール画像の右側で、 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

1. （オプション）ビューアリストウィンドウで、列見出しを選択します **[!UICONTROL 名前]** または **[!UICONTROL プラットフォームタイプ]** をクリックして、列を昇順または降順で並べ替えます。
1. ビューアリストウィンドウの表の「アクション」列で、次の項目を選択します **[!UICONTROL プレビュー]** 選択したビューアおよび platform タイプでのアセットの表示方法を確認するには、

   表示されたプレビューを閉じます。

1. （オプション）ビューアリストウィンドウの下部にある「URL 生成をコピーするための URL エンコーディング」ドロップダウンリストで、「URL エンコーディング」を選択します。 このエンコーディングは、アセットの URL をコピーするときに適用されます。
1. 必要に応じて次の操作を行います。

   * ビューアリストウィンドウの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]** 選択したビューアおよびプラットフォームのタイプ用。

     選択した場合 **[!UICONTROL URL をコピー]**&#x200B;に関連付けられた URL がクリップボードに自動的にコピーされます。

   * ビューアリストウィンドウの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**.

     選択した場合 **[!UICONTROL 埋め込みコード]**&#x200B;を選択すると、埋め込みコード ウィンドウが開き、ビューアコードを確認できます。 このウィンドウではコードの編集はできません。コードをクリップボードにコピーして、Web ページに貼り付けることもできます。

     表示されたプレビューを閉じます。

1. Viewer List ウィンドウの右下隅にある以下の項目を選択します。 **[!UICONTROL 閉じる]** をクリックして、アセット画面に戻ります。

## 画像プリセットに基づいた画像アセットのプレビュー {#previewing-an-image-asset-based-on-its-image-preset}

画像アセットを画像プリセットに基づいてプレビューすると、様々なサイズで web サイトやアプリケーションに動的に配信された画像がどのように表示されるかを確認できます。

画像プリセットは、事前定義済みの設定のコレクションです。 これらの設定により、画像のサイズ、画質、形式、解像度、書き出し時の画像の外観のその他の側面が変更されます。

参照： [画像プリセットの設定](setting-image-presets.md#setting_up_image_presets).

参照： [画像プリセットを作成して有効にする](creating-enabling-image-presets.md#creating_and_enabling_image_presets).

**画像プリセットに基づいて画像アセットをプレビューするには：**

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダーに移動します。
1. 次のいずれかの操作を行います。

   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL グリッド表示]**. アセットウィンドウで、1 つの画像アセットを選択し、サムネール画像の下の「」に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL 画像プリセットリスト]**.
   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL リスト表示]**. アセットウィンドウで、1 つの画像アセットを選択し、サムネール画像の右側で、 **[!UICONTROL プレビュー]** > **[!UICONTROL 画像プリセットリスト]**.
   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します **[!UICONTROL プレビュー]** > **[!UICONTROL 画像プリセットリスト]**.

1. 画像プリセットリストウィンドウの表で、右パネルでインラインでプレビューする画像アセットのプリセットタイプ名を選択します。
1. （オプション）画像プリセットリストウィンドウの **[!UICONTROL コピー URL 生成用の URL エンコーディング]** 下部のドロップダウンリスト。
1. 画像アセットの URL をコピーするときに適用する URL エンコーディングを選択します。
1. （オプション）画像プリセットリストウィンドウのプレビューペインの右上にある領域で、 **[!UICONTROL URL をコピー]** （選択したプリセットタイプ用）

   選択した場合 **[!UICONTROL URL をコピー]**&#x200B;に関連付けられた URL がクリップボードに自動的にコピーされます。

1. 画像プリセットリスト ウィンドウの右下隅にある「」を選択します。 **[!UICONTROL 閉じる]** をクリックして、アセット画面に戻ります。
