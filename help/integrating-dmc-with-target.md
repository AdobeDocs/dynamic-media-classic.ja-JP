---
title: AdobeDynamic MediaクラシックとAdobe Target標準/プレミアムの統合
description: AdobeDynamic MediaクラシックをAdobe Target標準/プレミアムと統合する方法を説明します。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Mediaクラシック
role: Data Engineer,Administrator,Business Practitioner
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 1%

---

# AdobeDynamic MediaクラシックとAdobe Target標準/プレミアムとの統合{#integrating-dmc-with-target}

[!DNL Dynamic Media Classic]と[!DNL Target Standard/Premium]を統合する前に、[!DNL Dynamic Media Classic]アプリケーションの全般設定画面でターゲットURLを入力する必要があります。 ターゲットURLを取得して、アプリケーションの全般設定ページに入力するには、次の手順を実行します。

1. [!DNL Adobe Experience Cloud]で、[!DNL Target Standard/Premium]アカウントにサインインします。
1. ログインした後、ブラウザーのアドレスバーに表示されているURLの先頭から`.com`までをコピーします。

   例えば、アドレスバーに表示される&#x200B;*架空の* URL（URLのパスには、この例のようにバックスラッシュではなく、常にスラッシュが含まれる）が`https:\\www.myfictionalsite.com/categories/admin/home.do`の場合、*架空の* URLの次の部分のみをコピーします。`https:\\www.myfictionalsite.com`。

1. [!DNL Dynamic Media Classic]で、**[!UICONTROL セットアップ]**/**[!UICONTROL アプリケーションセットアップ]**&#x200B;をクリックします。
1. アプリケーションの全般設定ページの「**[!UICONTROL Test&amp;ターゲットサーバー名]**」フィールドに、手順2でコピーしたURLを貼り付けます。
1. 「**[!UICONTROL 閉じる]**」をクリックします。
