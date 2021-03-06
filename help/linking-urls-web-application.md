---
title: WebアプリケーションへのURLのリンク
description: Dynamic Media ClassicからWebアプリケーションにURLをリンクする方法をAdobeします。
uuid: 1179bdd3-9b39-47f9-945d-1c1ca186bf96
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 71299640-676d-49b7-841d-6118f31044e8
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '843'
ht-degree: 37%

---

# WebアプリケーションへのURLのリンク{#linking-urls-to-your-web-application}

Webサイトやアプリケーションは、URL文字列を介してDynamic Media Image Serverコンテンツにアクセスします。 画像を公開すると、AdobeDynamic Media Classicは、Dynamic Media Image Server上の画像プリセットを参照するURL文字列をアクティブ化します。 これらの URL を Web ブラウザにペーストしてテストすることができます。

これらのURL文字列をWebページやアプリケーションに配置するには、AdobeDynamic Media Classicからコピーします。 画像プリセットで生成されたURL文字列を取得するには、プレビュー画面または参照パネル（詳細ビュー）に移動します。

## 画像プリセットURLの取得 {#obtaining-an-image-preset-url}

画像プリセットとともに生成された URL 文字列は、プレビューまたは詳細ビューから取得できます。URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

### プレビューから画像プリセットURLを取得 {#obtaining-an-image-preset-url-from-preview}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダに移動します。
1. 次のいずれかの操作を行います。

   * アセットウィンドウの上のツールバーの右側で、「**[!UICONTROL グリッドビュー]**」を選択します。 アセットウィンドウで1つの画像アセットを選択し、サムネール画像の下にある「**[!UICONTROL プレビュー]** 」/「**[!UICONTROL 画像プリセットリスト]**」に移動します。
   * アセットウィンドウの上のツールバーの右側で、「**[!UICONTROL リスト表示]**」を選択します。 アセットウィンドウで1つの画像アセットを選択し、サムネール画像の右側にある&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL 画像プリセットリスト]**&#x200B;に移動します。
   * アセットウィンドウの上のツールバーの右側で、**[!UICONTROL 詳細ビュー]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** /**[!UICONTROL 画像プリセットリスト]**&#x200B;に移動します。

1. （オプション）画像プリセットリストの「URLのコピー生成用のURLエンコーディング」ドロップダウンリストで、画像アセットのURLのコピー時に適用するURLエンコーディングを選択します。
1. 画像プリセットリストウィンドウのプレビューパネルの右上領域で、選択したプリセットの種類に対して「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL 
1. 画像プリセットリストウィンドウの右下隅にある「**[!UICONTROL 閉じる]**」を選択して、アセット画面に戻ります。

### 参照パネルから画像プリセットURLを取得する {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダに移動します。
1. アセットウィンドウの上のツールバーの右側で、「**[!UICONTROL グリッドビュー]**」を選択します。 アセットウィンドウで、1 つの画像アセットを選択します。
1. アセットウィンドウの上のツールバーの右側で、**[!UICONTROL 詳細ビュー]**&#x200B;を選択します。
1. 画面の右側のパネルで&#x200B;**[!UICONTROL URL]**&#x200B;を選択して、画像プリセットのリストを展開できます。
1. クリップボードにコピーするURLを持つ画像プリセット名の横にある「**[!UICONTROL URLをコピー]**」リンクを選択します。

## 画像プリセットの URL 文字列について {#about-image-preset-url-strings}

Dynamic Media Image Serverに対する画像サイズ設定のURL呼び出しの基本構文は次のとおりです。

*パス*/*Image Server 名*/*アカウント名*/*image画像名*?*モディファイア 1*&amp;*モディファイア 2*&amp;...

Dynamic Media Image ServerのURLでは、画像を表示するためのサーバーへの指示は、疑問符(?)の後に表示されます。 例えば、次の URL 呼び出しは、「backpack」という名前の画像を幅 250 pixel で配信します。

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

URL 内で、画像プリセット名はドル記号（$）で囲まれています。Dynamic Media Image ServerがURLの画像プリセット部分（この場合は`Large`）にアクセスした場合は、「大」の画像プリセットで定義されているサイズとフォーマットの指示を使用します。

## Webページへの動的画像の追加 {#adding-dynamic-images-to-your-web-page}

動的画像をWebページに追加するには、通常、HTML Webページコードの`<IMG>`タグを、Dynamic Media Image Serverにリクエストを送信するために、AdobeDynamic Media Classic URL文字列を使用して変更します。 この文字列は、画像プリセットによって定義されているサイズおよび形式仕様で画像を生成します。

例えば、静的な画像を開くための次のような一般的な呼び出しの代わりに、

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

次に、`<IMG>`タグを使用して、静的な画像への参照を、AdobeDynamic Media Classicプラットフォームへの画像プリセット呼び出しで置き換えます。 呼び出しの例を次に示します。

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$”
```

この例では、Dynamic Media Image Serverは`$thumbnail$`の定義を「検索」し、`thumbnail`画像プリセットで定義されたサイズとフォーマットの仕様に従って、適切な画像を動的に生成します。 URL 文字列の、製品の画像のファイル名（この例では `backpack_trns`）を除くすべての項目は、通常ページテンプレートに直接記述されています。コマースサーバからページテンプレートに自動的に挿入される唯一の項目は、IPS ID または画像の名前です。
