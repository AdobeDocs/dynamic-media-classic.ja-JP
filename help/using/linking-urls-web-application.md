---
title: Web アプリケーションへの URL のリンク
description: Adobe Dynamic Media Classicから Web アプリケーションに URL をリンクする方法を説明します。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# Web アプリケーションへの URL のリンク{#linking-urls-to-your-web-application}

Web サイトやアプリケーションは、URL 文字列を介してDynamic Media Image Server コンテンツにアクセスします。 画像を公開すると、Adobe Dynamic Media Classicは、Dynamic Media Image Server 上の画像プリセットを参照する URL 文字列をアクティベートします。 これらの URL を Web ブラウザにペーストしてテストすることができます。

これらの URL 文字列を Web ページやアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。 画像プリセットで生成された URL 文字列を取得するには、プレビュー画面または（詳細ビューの）参照パネルに移動します。

## 画像プリセット URL の取得 {#obtaining-an-image-preset-url}

画像プリセットとともに生成された URL 文字列は、プレビューまたは詳細ビューから取得できます。URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

### プレビューからの画像プリセット URL の取得 {#obtaining-an-image-preset-url-from-preview}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダに移動します。
1. 次のいずれかの操作を行います。

   * アセットウィンドウの上のツールバーの右側で、を選択します。 **[!UICONTROL グリッド表示]**. アセットウィンドウで 1 つの画像アセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL 画像プリセットリスト]**.
   * アセットウィンドウの上のツールバーの右側で、を選択します。 **[!UICONTROL リスト表示]**. アセットウィンドウで 1 つの画像アセットを選択し、サムネール画像の右側にある次の場所に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL 画像プリセットリスト]**.
   * アセットウィンドウの上のツールバーの右側で、を選択します。 **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL 画像プリセットリスト]**.

1. （オプション）画像プリセットリストの「 URL をコピー生成用の URL エンコーディング」ドロップダウンリストで、画像アセットの URL をコピーする際に適用する URL エンコーディングを選択します。
1. 画像プリセットリストウィンドウのプレビューパネルの右上領域で、「 」を選択します。 **[!UICONTROL URL をコピー]** 選択したプリセットタイプ用。
1. 画像プリセットリストウィンドウの右下隅で、「 **[!UICONTROL 閉じる]** をクリックして、アセット画面に戻ります。

### 参照パネルからの画像プリセット URL の取得 {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダに移動します。
1. アセットウィンドウの上のツールバーの右側で、を選択します。 **[!UICONTROL グリッド表示]**. アセットウィンドウで、1 つの画像アセットを選択します。
1. アセットウィンドウの上のツールバーの右側で、を選択します。 **[!UICONTROL 詳細ビュー]**.
1. 選択 **[!UICONTROL URL]** 画面の右側にあるパネルで、画像プリセットのリストを展開できます。
1. 選択 **[!UICONTROL URL をコピー]** クリップボードにコピーする URL を含む画像プリセット名の横にあるリンク。

## 画像プリセットの URL 文字列について {#about-image-preset-url-strings}

Dynamic Media Image Server に対する画像サイズ設定の URL 呼び出しの基本構文は次のとおりです。

*パス*/*Image Server 名*/*アカウント名*/*image画像名*?*モディファイア 1*&amp;*モディファイア 2*&amp;...

Dynamic Media Image Server URL では、画像を表示するためのサーバーへの指示は、疑問符 (?) の後に表示されます。 例えば、次の URL 呼び出しは、「backpack」という名前の画像を幅 250 pixel で配信します。

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

画像プリセット URL には、画像を適切なサイズおよび形式仕様で表示するためのすべての命令修飾子が含まれています。画像プリセットを使用しない場合は、次の URL 文字列のように、疑問符（?）の後ろにすべての命令修飾子が表示されます。

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

画像プリセットとともに生成された URL 文字列では、画像プリセットによって定義されている命令の代わりに画像プリセット名が表示されます。例えば、上記の長い URL を表す URL 文字列は、次のようになります。

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

URL 内で、画像プリセット名はドル記号（$）で囲まれています。Dynamic Media Image Server が URL の画像プリセット部分 ( `Large` この場合は )、「大」の画像プリセットで定義されたサイズとフォーマット手順を使用します。

## Web ページへの動的画像の追加 {#adding-dynamic-images-to-your-web-page}

動的画像を Web ページに追加するには、 `<IMG>` タグの内容は、通常、Dynamic Media Image Servers にリクエストを送信するために、Adobe Dynamic Media Classic URL 文字列を使用して変更されます。 この文字列は、画像プリセットによって定義されているサイズおよび形式仕様で画像を生成します。

例えば、静的な画像を開くための次のような一般的な呼び出しの代わりに、

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

これで、 `<IMG>`タグを使用して、静的な画像への参照をAdobe Dynamic Media Classicプラットフォームへの画像プリセット呼び出しに置き換えます。 呼び出しの例を次に示します。

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

この例では、Dynamic Media Image Server は、 `$thumbnail$` およびは、 `thumbnail`画像プリセット。 URL 文字列の、製品の画像のファイル名（この例では `backpack_trns`）を除くすべての項目は、通常ページテンプレートに直接記述されています。コマースサーバからページテンプレートに自動的に挿入される唯一の項目は、IPS ID または画像の名前です。
