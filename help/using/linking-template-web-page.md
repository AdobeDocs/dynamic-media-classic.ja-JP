---
title: Web ページへのテンプレートのリンク
description: Adobe Dynamic Media Classicで Web ページにテンプレートをリンクする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 16%

---

# Web ページへのテンプレートのリンク{#linking-a-template-to-a-web-page}

Web サイトおよびアプリケーションは、URL 文字列を介してDynamic Media Image Server コンテンツにアクセスします。 テンプレートを公開すると、Adobe Dynamic Media Classicはそのテンプレートを参照する URL 文字列をDynamic Media Image Server 上でアクティベートします。 この URL を Web ブラウザーに貼り付けてテストできます。

Web ページおよびアプリケーションに URL 文字列を配置するには、Adobe Dynamic Media Classicから URL 文字列をコピーします。 画像プリセットで生成されたテンプレート URL 文字列を取得するには、プレビュー画面または参照パネル（詳細表示）に移動します。 そして、画像プリセットを選択して、「URL をコピー」ボタンを選択します。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## テンプレート URL の取得 {#obtaining-a-template-url}

画像プリセットとともに生成されたテンプレート URL 文字列は、テンプレートのプレビュー画面から取得できます。URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。画像プリセットで生成されたテンプレート URL 文字列をテンプレートのプレビューページから取得するには、次の手順を実行します。

1. テンプレートのロールオーバーの選択 **[!UICONTROL プレビュー]** ボタンまたは移動 **[!UICONTROL ファイル]** > **[!UICONTROL プレビュー]**.
1. プリセットのメニューを使用して、テンプレート画像を配信する画像プリセットを選択します。 プレビューページには、サーバーからテンプレートが配信されたときの外観が表示されます。
1. を選択 **[!UICONTROL URL をコピー]** そのため、URL をクリップボードにコピーできます。

## Web ページへのテンプレート URL の追加 {#adding-template-urls-to-your-web-page}

Web ページにテンプレートを追加するには、Web ページの開発チームに問い合わせて、 `<IMG>` HTMLの web ページコードをタグ付けします。 Adobe Dynamic Media Classic URL 文字列を使用して、Dynamic Media Image Server にリクエストを送信します。 コマースエンジンまたは動的 web ページのコードは、テンプレート画像を、サイズに応じて、およびテンプレート用に選択した画像プリセットで定義されたフォーマット設定で挿入します。

>[!MORELIKETHIS]
>
>* [Web ページへの動的画像の追加](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
