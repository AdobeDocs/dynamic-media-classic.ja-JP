---
title: Web ページへのテンプレートのリンク
description: テンプレートをWebページにリンクする方法を説明します。
uuid: f111ef06-4afc-454c-86ce-5d640236d40b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 989dba07-448a-45b1-b157-af50abb5359a
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 50%

---

# Web ページへのテンプレートのリンク{#linking-a-template-to-a-web-page}

Webサイトやアプリケーションは、URL文字列を使用してDynamic Media Image Serverコンテンツにアクセスします。 テンプレートを公開すると、Dynamic Media Classicは、Dynamic Media Image Server上のテンプレートを参照するURL文字列をアクティブ化します。 この URL を Web ブラウザにペーストしてテストすることができます。

WebページやアプリケーションにURL文字列を配置するには、Dynamic Media Classicからコピーします。 画像プリセットとともに生成されたテンプレート URL 文字列を取得するには、プレビュー画面または参照パネル（詳細ビュー）に進みます。そして、画像プリセットを選択して、「URL をコピー」ボタンを選択します。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## テンプレート URL の取得 {#obtaining-a-template-url}

画像プリセットとともに生成されたテンプレート URL 文字列は、テンプレートのプレビュー画面から取得できます。URL をコピーすると、URL はクリップボードに格納され、必要に応じてペーストできるようになります。画像プリセットで生成されたテンプレートURL文字列をテンプレートプレビューページから取得するには、次の手順を実行します。

1. テンプレートのロールオーバーの「**[!UICONTROL プレビュー]**」ボタンをクリックするか、**[!UICONTROL ファイル]**/**[!UICONTROL プレビュー]**&#x200B;を選択します。
1. プリセットのメニューを使用して、テンプレート画像を配信する画像プリセットを選択します。プレビューページには、テンプレートをサーバーから配信したときにどのように表示されるかが示されます。
1. 「**[!UICONTROL URLをコピー]**」をクリックして、URLをクリップボードにコピーします。

## Web ページへのテンプレート URL の追加 {#adding-template-urls-to-your-web-page}

Webページにテンプレートを追加するには、Webページ開発チームに問い合わせて、HTML Webページコードの`<IMG>`タグを変更してください。 Dynamic Media Classic URL文字列を使用して、Dynamic Media Image Serverにリクエストを送信します。 コマースエンジンまたは動的 Web ページコードは、テンプレート用に選択した画像プリセットによって定義されているサイズおよび形式仕様でテンプレート画像を挿入します。

>[!MORELIKETHIS]
>
>* [Web ページへの動的画像の追加](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)

