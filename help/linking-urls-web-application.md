---
title: Web アプリケーションへの URL のリンク
seo-title: Web アプリケーションへの URL のリンク
description: 'null'
seo-description: URLをWebアプリケーションにリンクする方法について説明します。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/image_ sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Web アプリケーションへの URL のリンク{#linking-urls-to-your-web-application}

Webサイトやアプリケーションは、URL文字列を使用してダイナミックメディアImage Serverのコンテンツにアクセスします。画像を公開すると、ダイナミックメディアImage Server上の画像プリセットを参照するURL文字列がアクティブになります。これらの URL を Web ブラウザにペーストしてテストすることができます。

これらの URL 文字列を Web ページおよびアプリケーションに配置するには、Scene7 Publishing System から URL 文字列をコピーします。画像プリセットとともに生成された URL 文字列を取得するには、プレビュー画面または参照パネル（詳細ビュー）に進みます。

## 画像プリセットの URL の取得 {#obtaining-an-image-preset-url}

画像プリセットとともに生成された URL 文字列は、プレビューまたは詳細ビューから取得できます。URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。

***注意**:URLは、アセットを公開するまでアクティブになりません。*

### プレビューからの画像プリセットの URL の取得 {#obtaining-an-image-preset-url-from-preview}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダに移動します。
1. 次のいずれかの操作を行います。

   * アセットウィンドウの上のツールバー右側にある「グリッドビュー」をクリックします。アセットウィンドウで 1 つの画像アセットを選択し、サムネール画像の下にあるプレビュー／画像プリセットリストをクリックします。
   * アセットウィンドウの上のツールバー右側にある「リストビュー」をクリックします。アセットウィンドウで 1 つの画像アセットを選択し、サムネール画像の右側にあるプレビュー／画像プリセットリストをクリックします。
   * アセットウィンドウの上のツールバー右側にある「詳細ビュー」をクリックします。同じツールバーにあるプレビュー／画像プリセットリストをクリックします。

1. （オプション）画像プリセットリストウィンドウ下部の「URL をコピー生成で使用する URL エンコーディング」ドロップダウンリストで、画像アセットの URL がコピーされるときにアセットの URL に適用する URL エンコーディングを選択します。
1. 画像プリセットリストウィンドウのプレビューパネルの右上の領域で、選択したプリセットの種類の「URL をコピー」をクリックします。
1. 画像プリセットリストウィンドウの右下隅にある「閉じる」をクリックして、アセット画面に戻ります。

### 参照パネルからの画像プリセットの URL の取得 {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダに移動します。
1. アセットウィンドウの上のツールバー右側にある「グリッドビュー」をクリックします。アセットウィンドウで、1 つの画像アセットを選択します。
1. アセットウィンドウの上のツールバー右側にある「詳細ビュー」をクリックします。
1. 画面の右側のパネルで URL をクリックして、画像プリセットのリストを展開します。
1. クリップボードにコピーする URL を表わしている画像プリセット名の横にある「URL をコピー」リンクをクリックします。

## 画像プリセットの URL 文字列について {#about-image-preset-url-strings}

ダイナミックメディア画像サーバへの画像サイズ変更のURL呼び出しには、次の基本構文があります。

*パス*/*Image Server 名*/*アカウント名*/*image画像名*?*モディファイア 1*&amp;*モディファイア 2*&amp;...

ダイナミックメディアImage ServerのURLでは、画像を表示するための指示が、疑問符（?）の後に表示されます。例えば、次の URL 呼び出しは、「backpack」という名前の画像を幅 250 pixel で配信します。

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

URL 内で、画像プリセット名はドル記号（$）で囲まれています。When a Dynamic Media Image Server encounters the Image Preset portion of the URL (the `Large` in this case), using the size and formatting instructions defined by the “Large” Image Preset.

## Web ページへの動的画像の追加 {#adding-dynamic-images-to-your-web-page}

To add dynamic images to your web page, the `<IMG>` tag in your HTML web page code typically is modified using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. この文字列は、画像プリセットによって定義されているサイズおよび形式仕様で画像を生成します。

例えば、静的な画像を開くための次のような一般的な呼び出しの代わりに、

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

you now use the `<IMG>`tag to replace the reference to a static image with an Image Preset call to the Dynamic Media Classic platform. 呼び出しの例を次に示します。

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

In this example, a Dynamic Media Image Server “looks up” the definition of `$thumbnail$` and dynamically generates the appropriate image with the sizing and formatting specifications defined by the `thumbnail`Image Preset. URL 文字列の、製品の画像のファイル名（この例では `backpack_trns`）を除くすべての項目は、通常ページテンプレートに直接記述されています。コマースサーバからページテンプレートに自動的に挿入される唯一の項目は、IPS ID または画像の名前です。
