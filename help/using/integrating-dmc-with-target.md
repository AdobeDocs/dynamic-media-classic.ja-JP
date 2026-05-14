---
title: Adobe Dynamic Media ClassicとAdobe Target Standard/Premiumの統合
description: Adobe Dynamic Media ClassicとAdobe Target Standard/Premiumの統合方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:50.750Z'
TQID: 'https://experienceleague.adobe.com/csg3qawhCOMv6niWQHp9vyGgpJBcVuOOhExioDeURuA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 150
ht-degree: 0%

---

# Adobe Dynamic Media ClassicとAdobe Target Standard/Premiumの統合 {#integrating-dmc-with-target}

[!DNL Adobe Dynamic Media Classic]を[!DNL Target Standard/Premium]と統合する前に、[!DNL Adobe Dynamic Media Classic] アプリケーションの一般設定画面でターゲット URLを入力する必要があります。 Target URLを取得し、アプリケーションの一般設定ページに入力するには、次の操作を行います。

1. [!DNL Adobe Experience Cloud]で、[!DNL Target Standard/Premium] アカウントにログインします。
1. ログイン後、ブラウザーのアドレスバーに、`.com`までのURLをコピーします。

   例えば、アドレスバーの&#x200B;*架空の* URL （URLのパスに常にスラッシュが含まれ、この例のようにスラッシュが戻っていない）が`https:\\www.myfictionalsite.com/categories/admin/home.do`の場合、*架空の* URLのこの部分のみをコピーします：`https:\\www.myfictionalsite.com`。

1. [!DNL Adobe Dynamic Media Classic]で、**[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]**&#x200B;に移動します。
1. アプリケーションの一般設定ページの「**[!UICONTROL Test&amp;Target Server Name]**」フィールドに、手順2でコピーしたURLを貼り付けます。
1. **[!UICONTROL 閉じる]**&#x200B;を選択します。
