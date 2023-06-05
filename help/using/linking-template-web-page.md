---
title: Web ページへのテンプレートのリンク
description: Adobe Dynamic Media Classicでテンプレートを Web ページにリンクする方法を説明します。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 37%

---

# Web ページへのテンプレートのリンク{#linking-a-template-to-a-web-page}

Web サイトやアプリケーションは、URL 文字列を使用してDynamic Media Image Server コンテンツにアクセスします。 テンプレートを公開すると、Adobe Dynamic Media Classicは、Dynamic Media Image Server 上のテンプレートを参照する URL 文字列をアクティベートします。 この URL を Web ブラウザにペーストしてテストすることができます。

Web ページやアプリケーションに URL 文字列を配置するには、Adobe Dynamic Media Classicからコピーします。 画像プリセットで生成されたテンプレート URL 文字列を取得するには、プレビュー画面または参照パネル（詳細ビュー）に移動します。 そして、画像プリセットを選択して、「URL をコピー」ボタンを選択します。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## テンプレート URL の取得 {#obtaining-a-template-url}

画像プリセットとともに生成されたテンプレート URL 文字列は、テンプレートのプレビュー画面から取得できます。URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。画像プリセットで生成されたテンプレート URL 文字列をテンプレートプレビューページから取得するには、次の手順を実行します。

1. テンプレートのロールオーバーを選択 **[!UICONTROL プレビュー]** ボタンまたは移動 **[!UICONTROL ファイル]** > **[!UICONTROL プレビュー]**.
1. プリセットのメニューを使用して、テンプレート画像を配信する画像プリセットを選択します。プレビューページには、サーバーから配信されたときのテンプレートの外観が表示されます。
1. 選択 **[!UICONTROL URL をコピー]** URL をクリップボードにコピーできます。

## Web ページへのテンプレート URL の追加 {#adding-template-urls-to-your-web-page}

Web ページにテンプレートを追加するには、Web ページ開発チームに問い合わせて、 `<IMG>` タグをHTMLの Web ページコードに追加します。 Adobe Dynamic Media Classic Image Server にリクエストを送信するには、 Dynamic Media URL 文字列を使用します。 コマースエンジンまたは動的 Web ページコードは、テンプレート用に選択した画像プリセットによって定義されているサイズおよび形式仕様でテンプレート画像を挿入します。

>[!MORELIKETHIS]
>
>* [Web ページへの動的画像の追加](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

