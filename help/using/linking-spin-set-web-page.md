---
title: Web ページへのスピンセットのリンク
description: Adobe Dynamic Media Classicでスピンセットを Web ページにリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
topic: Content Management
level: Intermediate
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 33%

---

# Web ページへのスピンセットのリンク{#linking-a-spin-set-to-a-web-page}

Web サイトおよびアプリケーションは、URL 文字列または埋め込みコードを介して、スピンセットを含むDynamic Media Image Server コンテンツにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。スピンセットの URL 文字列または埋め込みコードを web ページやアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## スピンセット URL のコピー {#copying-a-spin-set-url}

1. アセットの参照パネルの「表示」ドロップダウンリストで、を選択します **[!UICONTROL スピンセット]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つスピンセットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * を選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、を選択します。 **[!UICONTROL URL をコピー]** をビューアの右側にクリックします。
   * を選択 **[!UICONTROL グリッド表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の下のに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**.

   * を選択 **[!UICONTROL リスト表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の右側で、 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**.

   * を選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**、または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL URL をコピー]**.

## Web ページへのスピンセット URL の追加 {#adding-spin-set-urls-to-your-web-page}

スピンセットは、すべてのズームビューアと同様、スピンセットをズームウィンドウ内に表示するダイナミックページ（ASP や JSP）経由で配信されます。Adobe Dynamic Media Classic プラットフォームへの URL 呼び出しは、ズームビューアでも同じプロトコルに従います。 ただし、ビューアプリセット名は、管理者が初期設定のスピンセットビューアプリセットとして定義したプリセットによって決まります。例えば、次の非ライブ URL 構文の例にはというプリセット名が含まれています `viewer.jsp` SKU パラメーターがスピンセット名になります。

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

この URL 構文の例（リンクが有効ではない）では、SKU 番号（ `sku=backpack_spin`）に設定します。 後の文字列 `sku=` はスピンセット名（ `backpack spin`）に設定します。

## スピンセットビューアの埋め込みコードのコピー {#copying-the-embed-code-of-a-spin-set-viewer}

埋め込みコード機能を使用すると、選択したスピンセットのビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。埋め込みコードダイアログボックスでは、コードを編集することはできません。

**スピンセットビューアの埋め込みコードをコピーするには：**

1. アセットの参照パネルの「表示」ドロップダウンリストで、を選択します **[!UICONTROL スピンセット]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つスピンセットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * を選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、を選択します。 **[!UICONTROL 埋め込みコード]** をビューアの右側にクリックします。
   * を選択 **[!UICONTROL グリッド表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の下のに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**.

   * を選択 **[!UICONTROL リスト表示]**. アセット参照パネルで、1 つのアセットを選択し、サムネール画像の右側で、 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**.

   * を選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**、または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

     ビューアリストページの表の「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]**.

1. 埋め込みコード ダイアログボックスで、を選択します。 **[!UICONTROL クリップボードにコピー]**.

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. を選択 **[!UICONTROL 閉じる]**.
