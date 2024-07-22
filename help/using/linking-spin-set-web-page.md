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
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 23%

---

# Web ページへのスピンセットのリンク{#linking-a-spin-set-to-a-web-page}

Web サイトおよびアプリケーションは、URL 文字列または埋め込みコードを介して、スピンセットを含むDynamic Media Image Server コンテンツにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。スピンセットの URL 文字列または埋め込みコードを web ページやアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## スピンセット URL のコピー {#copying-a-spin-set-url}

1. アセットの参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL スピンセット]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーするスピンセットを含むアセットフォルダーに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッド表示]** を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコード パネルで、必要なビューアの右側にある **[!UICONTROL URL をコピー]** を選択します。
   * **[!UICONTROL グリッド表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL リスト表示]** を選択します。 アセット参照パネルで、アセットを 1 つ選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

   * **[!UICONTROL グリッド表示]**、**[!UICONTROL リスト表示]** または **[!UICONTROL 詳細表示]** を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]** に移動します。

     ビューアリストページの表の「アクション」列で、「**[!UICONTROL URL をコピー]**」を選択します。

## Web ページへのスピンセット URL の追加 {#adding-spin-set-urls-to-your-web-page}

スピンセットは、すべてのズームビューアと同様、スピンセットをズームウィンドウ内に表示するダイナミックページ（ASP や JSP）経由で配信されます。Adobe Dynamic Media Classic プラットフォームへの URL 呼び出しは、ズームビューアでも同じプロトコルに従います。 ただし、ビューアプリセット名は、管理者が初期設定のスピンセットビューアプリセットとして定義したプリセットによって決まります。例えば、次のライブ以外の URL 構文の例には `viewer.jsp` というプリセット名が含まれており、SKU パラメーターはスピンセット名になっています。

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

この URL 構文の例（リンクが実稼動中ではない）では、SKU 番号（`sku=backpack_spin`）が表示されています。 `sku=` の後の文字列はスピンセット名（`backpack spin`）です。

## スピンセットビューアの埋め込みコードのコピー {#copying-the-embed-code-of-a-spin-set-viewer}

埋め込みコード機能を使用すると、選択したスピンセットのビューアコードをレビューすることができます。コードをクリップボードにコピーして、Web ページに貼り付け、ビューアをデプロイすることもできます。 埋め込みコードダイアログボックスでは、コードを編集することはできません。

**スピンセットビューアの埋め込みコードをコピーするには：**

1. アセットの参照パネルの「表示」ドロップダウンリストで、「**[!UICONTROL スピンセット]**」を選択します。
1. 左側のアセットライブラリパネルで、埋め込みコードをコピーするスピンセットを含むアセットフォルダーに移動します。
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
