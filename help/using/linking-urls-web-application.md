---
title: Web アプリケーションへのURLのリンク
description: Adobe Dynamic Media ClassicからWeb アプリケーションにURLをリンクする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic
role: User
exl-id: ca629427-da33-4bab-9d08-6d9368042f7e
topic: Administration, Content Management, Development
level: Intermediate
autotag-review: '2026-05-13T20:03:48.579Z'
TQID: 'https://experienceleague.adobe.com/c8e722KVmasJVtoVl8k7-5vGjvs4Lm-GZavm-TF9fk0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 844
ht-degree: 24%

---

# Web アプリケーションへのURLのリンク{#linking-urls-to-your-web-application}

Web サイトとアプリケーションは、URL文字列を介してDynamic Media Image Server コンテンツにアクセスします。 画像を公開すると、Adobe Dynamic Media Classicは、Dynamic Media Image Serverの画像プリセットを参照するURL文字列をアクティブにします。 これらのURLをWeb ブラウザーに貼り付けてテストできます。

これらのURL文字列をWeb ページおよびアプリケーションに配置するには、Adobe Dynamic Media Classicからコピーします。 画像プリセットで生成されたURL文字列を取得するには、プレビュー画面または参照パネル（詳細表示）に移動します。

## 画像プリセット URLの取得 {#obtaining-an-image-preset-url}

画像プリセットとともに生成された URL 文字列は、プレビューまたは詳細ビューから取得できます。 URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

### プレビューから画像プリセット URLを取得 {#obtaining-an-image-preset-url-from-preview}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダーに移動します。
1. 次のいずれかの操作を行います。

   * Assets ウィンドウの上、ツールバーの右側にある&#x200B;**[!UICONTROL グリッド表示]**&#x200B;を選択します。 アセットウィンドウで、単一の画像アセットを選択し、サムネイル画像の下の「**[!UICONTROL プレビュー]**」 > 「**[!UICONTROL 画像プリセットリスト]**」に移動します。
   * Assets ウィンドウの上、ツールバーの右側にある「**[!UICONTROL リスト表示]**」を選択します。 アセットウィンドウで、単一の画像アセットを選択し、サムネイル画像の右側にある&#x200B;**[!UICONTROL プレビュー]**/**[!UICONTROL 画像プリセットリスト]**&#x200B;に移動します。
   * Assets ウィンドウの上、ツールバーの右側にある&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** > **[!UICONTROL 画像プリセットリスト]**&#x200B;に移動します。

1. （オプション）画像プリセットリストの「URL エンコーディング URL生成のコピー」ドロップダウンリストで、画像アセットのコピー時にURLに適用するURL エンコーディングを選択します。
1. 画像プリセットリストウィンドウのプレビューペインの右上領域で、選択したプリセットタイプの&#x200B;**[!UICONTROL URLをコピー]**&#x200B;を選択します。
1. 画像プリセットリストウィンドウの右下隅にある「**[!UICONTROL 閉じる]**」を選択して、Assets画面に戻ります。

### 参照パネルから画像プリセット URLを取得する {#obtaining-an-image-preset-url-from-the-browse-panel}

1. 左側のアセットライブラリパネルで、プレビューする画像アセットを含むアセットフォルダーに移動します。
1. Assets ウィンドウの上、ツールバーの右側にある&#x200B;**[!UICONTROL グリッド表示]**&#x200B;を選択します。 アセットウィンドウで、1 つの画像アセットを選択します。
1. Assets ウィンドウの上、ツールバーの右側にある&#x200B;**[!UICONTROL 詳細表示]**&#x200B;を選択します。
1. 画面の右側にあるパネルで「**[!UICONTROL URL]**」を選択して、画像プリセットのリストを展開します。
1. クリップボードにコピーするURLを含む画像プリセットの名前の横にある「**[!UICONTROL URLをコピー]**」リンクを選択します。

## 画像プリセットの URL 文字列について {#about-image-preset-url-strings}

Dynamic Media Image Serverへの画像サイズ変更のURL呼び出しには、次の基本的な構文があります。

*パス*/*画像サーバーの名前*/*アカウント名*/*画像名*?*modifier1*&amp;*modifier2*&amp;...

Dynamic Media Image ServerのURLでは、画像を表示するためのサーバーへの指示が、疑問符（?）の後に表示されます。 例えば、このURL呼び出しは、幅250 ピクセルの「バックパック」という名前の画像を配信します。

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250
```

画像プリセット URL には、画像を適切なサイズおよび形式仕様で表示するためのすべての命令修飾子が含まれています。 画像プリセットを使用しない場合は、次の URL 文字列のように、疑問符（?）の後ろにすべての命令修飾子が 表示されます。

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?wid=250&fmt=jpeg&qlt=80,0&resMode=sharp&op_usm=1.1,0.5,1,0
```

画像プリセットとともに生成された URL 文字列では、画像プリセットによって定義されている命令の代わりに画像プリセット名が表示されます。 例えば、上記の長い URL を表す URL 文字列は、次のようになります。

```as3
https://s7d1.scene7.com/is/image/S7learn/backpack?$Large$
```

URL 内で、画像プリセット名はドル記号（$）で囲まれています。 Dynamic Media Image ServerでURLの画像プリセット部分（この場合は`Large`）が検出された場合、「大」画像プリセットで定義されたサイズと形式の指示を使用します。

## Web ページへの動的画像の追加 {#adding-dynamic-images-to-your-web-page}

Web ページに動的画像を追加する場合、通常、HTML ページコードの`<IMG>` タグは、Adobe Dynamic Media Classic URL文字列を使用してDynamic Media Image Serversにリクエストを行うために変更されます。 この文字列は、画像プリセットによって定義されているサイズおよび形式仕様で画像を生成します。

例えば、静的な画像を開くための次のような一般的な呼び出しの代わりに、

```as3
img src="/company_images/products/backpack_thumbnail.jpg"
```

これで、`<IMG>` タグを使用して、静止画像への参照を、Adobe Dynamic Media Classic プラットフォームへの画像プリセット呼び出しに置き換えることができました。 呼び出しの例を次に示します。

```as3
img src="https://s7d2.scene7.com/is/image/S7learn/backpack_trns?$thumbnail$"
```

この例では、Dynamic Media Image Serverが`$thumbnail$`の定義を「検索」し、`thumbnail`画像プリセットで定義されたサイズと形式の仕様を使用して、適切な画像を動的に生成します。 URL文字列では、製品画像のファイル名（この場合は`backpack_trns`）を除くすべての項目は、通常、ページテンプレートに対してハード接続されます。 コマースサーバからページテンプレートに自動的に挿入される唯一の項目は、IPS ID または画像の名前です。
