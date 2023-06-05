---
title: Web ページへのスピンセットのリンク
description: スピンセットをAdobe Dynamic Media Classicの Web ページにリンクする方法を説明します。
uuid: d3c5773e-60c4-4e8b-9c48-e1e3eb8028d0
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 651b21ef-e322-4e6d-8e37-45ffd56f7a58
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: af75547e-20e8-44c2-b165-01532d6e21d0
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 40%

---

# Web ページへのスピンセットのリンク{#linking-a-spin-set-to-a-web-page}

Web サイトやアプリケーションは、URL 文字列または埋め込みコードを介して、スピンセットなどのDynamic Media Image Server コンテンツにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。Web ページやアプリケーションにスピンセットの URL 文字列や埋め込みコードを配置するには、Adobe Dynamic Media Classicからコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## スピンセット URL のコピー {#copying-a-spin-set-url}

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL スピンセット]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つスピンセットを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコードパネルで、 **[!UICONTROL URL をコピー]** を選択します。
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

      ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

## スピンセット URL を Web ページに追加する {#adding-spin-set-urls-to-your-web-page}

スピンセットは、すべてのズームビューアと同様、スピンセットをズームウィンドウ内に表示するダイナミックページ（ASP や JSP）経由で配信されます。Adobe Dynamic Media Classicプラットフォームへの URL 呼び出しは、ズームビューアと同じプロトコルに従います。 ただし、ビューアプリセット名は、管理者が初期設定のスピンセットビューアプリセットとして定義したプリセットによって決まります。例えば、次の URL 構文の例（リンクは無効）には、`viewer.jsp` という名前のプリセット名が含まれていて、SKU パラメーターはスピンセット名になっています。

```as3
https://sample.scene7.com/s7ondemand/spin/viewer.jsp?company=S7Web&sku=backpack_spin
```

この URL 構文の例（リンクは無効）には、SKU 番号（`sku=backpack_spin`）が含まれています。の後の文字列 `sku=` はスピンセット名 ( `backpack spin`) をクリックします。

## スピンセットビューアの埋め込みコードをコピーする {#copying-the-embed-code-of-a-spin-set-viewer}

埋め込みコード機能を使用すると、選択したスピンセットのビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。埋め込みコードダイアログボックスでは、コードを編集することはできません。

**スピンセットビューアの埋め込みコードをコピーするには:**

1. アセット参照パネルの「表示」ドロップダウンリストで、 **[!UICONTROL スピンセット]**.
1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つスピンセットを含むアセットフォルダに移動します。
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
