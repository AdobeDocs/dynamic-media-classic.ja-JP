---
title: テンプレートをWeb ページにリンクする
description: Adobe Dynamic Media ClassicでテンプレートをWeb ページにリンクする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 6305c287-360f-48c2-b456-58be0791c7af
topic: Administration, Content Management, Development
level: Experienced
autotag-review: '2026-05-13T19:52:27.080Z'
TQID: 'https://experienceleague.adobe.com/c1Un6UFrYZh-tqwPp98shMiTUEEMhkEn1vmxEl2rVq0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: f55e82148ae9d11c54dda28351743b02c1fb58a4
workflow-type: tm+mt
source-wordcount: 330
ht-degree: 11%

---

# テンプレートをWeb ページにリンクする{#linking-a-template-to-a-web-page}

web サイトやアプリケーションは、URL文字列を使用してDynamic Media Image Serverのコンテンツにアクセスできます。 テンプレートを公開すると、Adobe Dynamic Media Classicは、Dynamic Media Image Server上のテンプレートを参照するURL文字列をアクティブにします。 このURLをWeb ブラウザーに貼り付けてテストできます。

Web ページやアプリケーションにURL文字列を配置するには、Adobe Dynamic Media ClassicからURL文字列をコピーします。 画像プリセットで生成されたテンプレート URL文字列を取得するには、プレビュー画面または参照パネル（詳細表示）に移動します。 そして、画像プリセットを選択して、「URL をコピー」ボタンを選択します。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## テンプレート URLの取得 {#obtaining-a-template-url}

画像プリセットとともに生成されたテンプレート URL 文字列は、テンプレートのプレビュー画面から取得できます。 URLをコピーした後、クリップボードに保存され、必要に応じて貼り付けることができます。 画像プリセットで生成されたテンプレート URL文字列をテンプレートプレビューページから取得するには、次の操作を行います。

1. テンプレートの&#x200B;**[!UICONTROL プレビュー]** ボタンを選択するか、**[!UICONTROL ファイル]** > **[!UICONTROL プレビュー]**&#x200B;に移動します。
1. プリセットのメニューを使用して、テンプレートを配信する画像プリセットを選択します。 プレビューページには、サーバーから配信されるテンプレートが表示されます。
1. 「**[!UICONTROL URLをコピー]**」を選択すると、URLをクリップボードにコピーできます。

## Web ページへのテンプレート URLの追加 {#adding-template-urls-to-your-web-page}

Web ページにテンプレートを追加するには、Web ページ開発チームに問い合わせて、HTML Web ページコードの`<IMG>` タグを変更します。 Adobe Dynamic Media Classic URL文字列を使用して、Dynamic Media Image Serverにリクエストを送信します。 コマースエンジンまたはダイナミックウェブページコードは、テンプレート画像を、サイズと、テンプレートに選択した画像プリセットで定義された書式仕様で挿入します。

>[!MORELIKETHIS]
>
>* [Web ページに動的画像を追加](linking-urls-web-application.md#adding_dynamic_images_to_your_web_page)
