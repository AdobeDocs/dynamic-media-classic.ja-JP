---
title: AdobeDynamic Media ClassicとAdobe Target Standard/Premiumの統合
description: Dynamic Media ClassicとAdobe Target Standard/PremiumのAdobeを統合する方法について説明します。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# AdobeDynamic Media ClassicとAdobe Target Standard/Premiumの統合 {#integrating-dmc-with-target}

[!DNL Adobe Dynamic Media Classic]と[!DNL Target Standard/Premium]を統合する前に、[!DNL Adobe Dynamic Media Classic]アプリケーションの一般設定画面にTarget URLを入力する必要があります。 Target URLを取得して、アプリケーションの一般設定ページに入力するには、次の手順を実行します。

1. [!DNL Adobe Experience Cloud]で、[!DNL Target Standard/Premium]アカウントにサインインします。
1. ログイン後、ブラウザーのアドレスバーで、URLを`.com`までコピーします。

   例えば、アドレスバーの&#x200B;*fiction* URL（URLパスには常にスラッシュが含まれ、この例のようにバックスラッシュは含まれません）が`https:\\www.myfictionalsite.com/categories/admin/home.do`の場合、*fictional* URLのこの部分のみをコピーします。`https:\\www.myfictionalsite.com`.

1. [!DNL Adobe Dynamic Media Classic]で、**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]**&#x200B;に移動します。
1. アプリケーションの一般設定ページの「**[!UICONTROL Test&amp;Target Server Name]**」フィールドに、手順2でコピーしたURLを貼り付けます。
1. **[!UICONTROL 閉じる]**&#x200B;を選択します。
