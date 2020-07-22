---
title: Adobe ClassicとAdobe TargetClassicの統合
seo-title: Adobe ClassicとAdobe TargetClassicの統合
description: 'null'
seo-description: Adobe ClassicとAdobe Classicの統合Dynamic Mediaを説明します。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
translation-type: tm+mt
source-git-commit: 044c4fd8dc06369b7ac6b5eb65014835d2b84fee
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 9%

---


# Adobe ClassicとAdobe TargetClassicの統合{#integrating-adobe-scene-with-adobe-target-classic}

Dynamic MediaClassicをTargetClassicと統合する前に、Dynamic Mediaクラシックアプリケーションの全般設定画面でTargetクラシックURLを入力する必要があります。 TargetのクラシックURLを取得して、アプリケーションの全般設定画面に入力するには、次の手順に従います。

1. 次のアドレスの「Targetクラシックログイン」ページに移動します。 https://admin.testandtarget.omniture.com
1. 資格情報を入力し、「 **ログイン**」をクリックします。
1. ログインした後に、ブラウザのアドレスバーに表示されている URL の先頭から *.com* までをコピーします。

   For example, if the *fictional* URL (URLs paths always contain forward slashes, not back slashes as in this example) in the address bar is `https:\\www.mysite.com/categories/admin/home.do`, copy only this portion of the *fictional* URL: `https:\\www.mysite.com`.

   手順5で、コピーしたURLの一部をDynamic Mediaクラシックアプリケーションの全般設定画面に貼り付けます。

1. Dynamic Mediaクラシックで、 **設定** / **アプリケーション設定をクリックします**。
1. アプリケーションの全般設定ページの「 **[!UICONTROL Test&amp;Application Server Name]** 」フィールドに、手順3でコピーしたURLを貼り付けます。
1. 「**閉じる**」をクリックします。

