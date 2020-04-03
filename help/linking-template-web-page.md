---
title: Web ページへのテンプレートのリンク
seo-title: Web ページへのテンプレートのリンク
description: 'null'
seo-description: テンプレートをWebページにリンクする方法を説明します。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Web ページへのテンプレートのリンク{#linking-a-template-to-a-web-page}

Webサイトやアプリケーションは、URL文字列を使用してDynamic Media Image Serverのコンテンツにアクセスします。 テンプレートを公開すると、ダイナミックメディアイメージサーバー上のテンプレートを参照するURL文字列がアクティブになります。 この URL を Web ブラウザにペーストしてテストすることができます。

これらの URL 文字列を Web ページおよびアプリケーションに配置するには、Scene7 Publishing System から URL 文字列をコピーします。画像プリセットとともに生成されたテンプレート URL 文字列を取得するには、プレビュー画面または参照パネル（詳細ビュー）に進みます。そして、画像プリセットを選択して、「URL をコピー」ボタンを選択します。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## テンプレート URL の取得 {#obtaining-a-template-url}

画像プリセットとともに生成されたテンプレート URL 文字列は、テンプレートのプレビュー画面から取得できます。URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。画像プリセットとともに生成されたテンプレート URL 文字列をテンプレートのプレビュー画面から取得するには、次の手順に従います。

1. テンプレートのロールオーバー時に表示される「プレビュー」ボタンをクリックするか、ファイル／プレビューを選択します。プレビュー画面が開きます。
1. プリセットのメニューを使用して、テンプレート画像を配信する画像プリセットを選択します。サーバに配信されたときにテンプレートがどのように表示されるかがプレビュー画面に示されます。
1. 「URL をコピー」ボタンをクリックして、URL をクリップボードにコピーします。

## Web ページへのテンプレート URL の追加 {#adding-template-urls-to-your-web-page}

To add a template to your web page, consult with your web page development team to modify the `<IMG>` tag in your HTML web page code using the Dynamic Media Classic URL string to make a request to Dynamic Media Image Servers. コマースエンジンまたは動的 Web ページコードは、テンプレート用に選択した画像プリセットによって定義されているサイズおよび形式仕様でテンプレート画像を挿入します。

>[!MORELIKETHIS]
>
>* [Web ページへの動的画像の追加](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

