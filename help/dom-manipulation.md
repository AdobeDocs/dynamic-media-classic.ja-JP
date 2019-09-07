---
title: DOM 操作
seo-title: DOM 操作
description: 'null'
seo-description: DOM操作について説明します。
uuid: 275cd49d-2a55-41f9-80b0- e147d0cd2907
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/template- publishing
discoiquuid: 890ca93e-3146-4347-864b- bd5e94037038
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# DOM 操作{#dom-manipulation}

DOM（ドキュメントオブジェクトモデル）操作は、XML コードを直接操作してデザインファイルを編集する方法です。DOM 操作では、コンテンツや外観の変更など、可変デザイン要素を詳細に制御することができます。また、必要に応じて新しい要素を作成することもできます。

Dynamic Media Classicでは、テンプレートの公開後にURLコマンドを使用して、Dynamic Media Classic FXGテンプレートのDOMを操作できます。FXG テンプレートのデザイン要素は、URL を通じてコマンドを渡すことで操作します。この方法により、グラフィックの属性を動的に操作および追加することができます。

DOM操作を使用するには、s7を作成します。elementIDを使用します。

>[!NOTE]
>
>DOM 操作コマンドを使用する場合は、渡す値がすべて URL でエンコードされている必要があります。

>[!NOTE]
>
>Illustrator Plug-in for Web-to-Print (for converting Illustrator files) converts to FXG 2.0. For information about this specification, see [www.adobe.com/go/learn_s7_fxg2_en](https://www.adobe.com/go/learn_s7_fxg2_en).

## Illustrator ファイル内への s7:elementID の作成 {#creating-s-elementids-in-illustrator-files}

Illustrator で作成したデザインで DOM 操作を使用するには、Illustrator のデザイン内に s7:elementID を作成します。s7:elementID を作成することで、テンプレートの公開後に URL コマンドを使用してデザイン要素を変更できるようになります。

### テキストの DOM 操作用の s7:elementID の作成 {#creating-s-elementids-for-dom-manipulation-of-text}

テキストオブジェクトの DOM 操作用の s7:elementID を作成するには、Illustrator でレイヤーパネルを開きます。次に、可変テキストが含まれているテキストレイヤーで、s7:elementID を使用してレイヤーに名前を付けます。To do so, enter the letters `id` (for identification), a colon ( `:`), and a name. s7:elementID テキストレイヤー名の例を次に示します。

`id:BirthdayBoyName`

`id:DateofBirth`

`id:EnterFirstNameHer`

### オブジェクトの DOM 操作用の s7:elementID の作成 {#creating-s-elementids-for-dom-manipulation-of-objects}

オブジェクトの s7:elementID は、エンドユーザがオブジェクトの属性を変更できるようにする場合に作成します。オブジェクトは、テキストフレーム、グラフィックおよび画像全体を構成することができます。色付きの背景は、オブジェクト要素 ID の一つの例です。エンドユーザは、季節の移り変わりに伴って、ポスターの背景色を季節に適した色に入れ替えることができます。

Illustrator でオブジェクトの s7:elementID を作成する前に、オブジェクト用の個別のレイヤーを作成します。

Illustrator でオブジェクトの s7:elementID を作成するには、次の手順に従います。

1. オブジェクトを選択します。
1. **ウィンドウ** / **レイヤー**&#x200B;をクリックします。
1. レイヤーパネルで、オブジェクトレイヤーにs7という名前を付けます。elementID.To do so, enter the letters `id` (for identification), a colon ( `:`), and description to identify the element. s7:elementID オブジェクトレイヤー名の例を次に示します。

   `id:BackgroundColor`

   `id:RotationPercentage`

   `id:JacketJPG`

## FXG テンプレートの公開 {#publish-fxg-templates}

FXGテンプレートを公開すると、それがDynamic Media Classicサーバーに配置され、Webサイトやアプリケーションで使用できるようになります。公開処理中に、Scene7 Publishing System は Web サイトやアプリケーションに必要な URL 文字列もアクティブにします。

>[!NOTE]
>
>FXG テンプレートを使用するには、フォントや画像など、テンプレートを作成するのに使用したすべてのコンテンツを公開します。必要なすべてのファイルを含めないと、公開時にエラーメッセージが表示されます。

### FXG テンプレートを公開用にマーク {#mark-fxg-templates-for-publish}

テンプレートとそのすべてのサポートファイルは、ダイナミックメディア画像サーバに配置するために公開用にマークする必要があります。

1. 参照パネルで、使用されているグラフィック、画像、およびフォントとともに、FXG テンプレートを選択します。
1. 「公開用 **にマーク」をクリック**&#x200B;します。

### FXG テンプレートの公開 {#publish-your-fxg-template}

1. グローバルナビゲーションバーで「**公開**」をクリックします。
1. 「日時」オプションを選択し、必要に応じて、公開ジョブの名前を入力します。
1. Click **Start Publish**.

### テキストオーバーフローインジケータ表示 {#text-overflow-indicator-display}

*テキストオーバーフローインジケータ*&#x200B;は、テキストフレーム（スレッドテキストの場合は最後のテキストフレーム）で割り当てられているスペースをテキストが超過した場合に表示されます。インジケータはプラス記号が入った赤いボックスとして表示されます。SPS のテキストオーバーフローインジケータは常に有効です。

テキストオーバーフローインジケータは `markOverflowingTextFrame` 修飾子で制御します。修飾子は次のように使用します。

| 修飾子／値 | 説明 |
|--- |--- |
| markOverflowingTextFrame=0,1 | 値が 1 の場合は、テキストフローインジケータが表示されます。初期設定は 0 です（初期設定は 0 ですが、SPS のテキストオーバーフローインジケータは常に有効な状態です）。markOverflowingTextFrame 修飾子では大文字と小文字が区別されます。 |

>[!MORELIKETHIS]
>
>* [可変性の定義：パラメータ化と DOM 操作について](defining-variability-parameterization-versus-dom.md#defining_variability_parameterization_versus_dom_manipulation)
>* [公開](publishing-files.md#publishing_files)

