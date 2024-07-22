---
title: Web アプリケーションへの URL のリンク
description: Adobe Dynamic Media Classicから web アプリケーションに URL をリンクする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 26%

---

# Web アプリケーションへの URL のリンク{#linking-urls-to-your-web-application}

Web サイトおよびアプリケーションは、URL 文字列を介してDynamic Media Image Server コンテンツにアクセスします。 画像を公開すると、Adobe Dynamic Media ClassicはDynamic Media Image Server 上の画像プリセットを参照する URL 文字列をアクティベートします。 これらの URL を Web ブラウザーに貼り付けてテストできます。

これらの URL 文字列を web ページやアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。 画像プリセットで生成された URL 文字列を取得するには、プレビュー画面または参照パネル（詳細表示）に移動します。

## 画像プリセット URL の取得 {#obtaining-an-image-preset-url}

画像プリセットとともに生成された URL 文字列は、プレビューまたは詳細ビューから取得できます。URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

### プレビューからの画像プリセット URL の取得 {#obtaining-an-image-preset-url-from-preview}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダーに移動します。
1. 次のいずれかの操作を行います。

   * Assetsウィンドウの上のツールバーの右側にある「**[!UICONTROL グリッド表示]**」を選択します。 アセットウィンドウで、1 つの画像アセットを選択し、サムネール画像の下で **[!UICONTROL プレビュー]**/**[!UICONTROL 画像プリセットリスト]** に移動します。
   * Assetsウィンドウの上のツールバーの右側にある「**[!UICONTROL リスト表示]**」を選択します。 アセットウィンドウで、1 つの画像アセットを選択し、サムネール画像の右側で **[!UICONTROL プレビュー]**/**[!UICONTROL 画像プリセットリスト]** に移動します。
   * Assetsウィンドウの上のツールバーの右側にある「**[!UICONTROL 詳細ビュー]**」を選択します。 同じツールバーで、**[!UICONTROL プレビュー]**/**[!UICONTROL 画像プリセットリスト]** に移動します。

1. （オプション）画像プリセットリストの「URL 生成をコピーするための URL エンコーディング」ドロップダウンリストで、画像アセットの URL をコピーするときに適用する URL エンコーディングを選択します。
1. 画像プリセットリスト ウィンドウのプレビューペインの右上領域で、選択したプリセットタイプに対して「**[!UICONTROL URL をコピー]**」を選択します。
1. 画像プリセットリストウィンドウの右下隅にある「**[!UICONTROL 閉じる]** を選択して、Assets画面に戻ります。

### 参照パネルからの画像プリセット URL の取得 {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダーに移動します。
1. Assetsウィンドウの上のツールバーの右側にある「**[!UICONTROL グリッド表示]**」を選択します。 アセットウィンドウで、1 つの画像アセットを選択します。
1. Assetsウィンドウの上のツールバーの右側にある「**[!UICONTROL 詳細ビュー]**」を選択します。
1. 画面の右側のパネルで **[!UICONTROL URL]** を選択して、画像プリセットのリストを展開します。
1. クリップボードにコピーする URL を含む画像プリセット名の横にある **[!UICONTROL URL をコピー]** リンクを選択します。

## 画像プリセットの URL 文字列について {#about-image-preset-url-strings}

Dynamic Media Image Server に対する画像サイズ設定の URL 呼び出しは、次の基本的な構文を持ちます。

*パス*/*Image Server 名*/*アカウント名*/*image画像名*?*モディファイア 1*&amp;*モディファイア 2*&amp;...

Dynamic Media Image Server の URL では、疑問符（?）の後に画像を表示するためのサーバーへの指示が表示されます。 例えば、次の URL 呼び出しは、「backpack」という名前の画像を 250 ピクセルの幅で配信します。

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

URL 内で、画像プリセット名はドル記号（$）で囲まれています。「Large」画像プリセットで定義されるサイズおよびフォーマット手順を使用して、Dynamic Media Image Server が URL （この場合は `Large`）の画像プリセット部分に到達したとき。

## Web ページへの動的画像の追加 {#adding-dynamic-images-to-your-web-page}

Web ページに動的画像を追加する場合、HTMLページコードの `<IMG>` タグは通常、Adobe Dynamic Media Classic URL 文字列を使用して変更され、Dynamic Media Image Server にリクエストを送信します。 この文字列は、画像プリセットによって定義されているサイズおよび形式仕様で画像を生成します。

例えば、静的な画像を開くための次のような一般的な呼び出しの代わりに、

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

`<IMG>` タグを使用して、静的画像への参照を、Adobe Dynamic Media Classic プラットフォームへの画像プリセット呼び出しに置き換えるようになりました。 呼び出しの例を次に示します。

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

この例では、Dynamic Media Image Server が `$thumbnail$` の定義を「検索」し、`thumbnail` 画像プリセットで定義されたサイズとフォーマットの仕様を使用して、適切な画像を動的に生成します。 URL 文字列では、製品画像のファイル名（この場合は `backpack_trns`）を除くすべての項目が、通常、ページテンプレートにハードワイヤリングされます。 コマースサーバからページテンプレートに自動的に挿入される唯一の項目は、IPS ID または画像の名前です。
