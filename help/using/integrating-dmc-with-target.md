---
title: Adobe Dynamic Media ClassicとAdobe Target Standard/Premium の統合
description: Adobe Dynamic Media ClassicとAdobe Target Standard/Premium を統合する方法について説明します。
uuid: d1c07a52-b058-4ae3-a31d-44c43dc27f65
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 3b4add18-4191-475e-a3a3-0184367a25fc
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Adobe Dynamic Media ClassicとAdobe Target Standard/Premium の統合 {#integrating-dmc-with-target}

統合する前に [!DNL Adobe Dynamic Media Classic] と [!DNL Target Standard/Premium]を使用する場合は、 [!DNL Adobe Dynamic Media Classic] アプリケーションの一般設定画面。 Target URL を取得し、アプリケーションの一般設定ページに入力するには、次の手順を実行します。

1. In [!DNL Adobe Experience Cloud]、 [!DNL Target Standard/Premium] アカウント
1. ログイン後、ブラウザーのアドレスバーに URL をコピーし、次の URL を含めます。 `.com`.

   例えば、 *架空の* アドレスバーの URL（URL のパスには常にスラッシュが含まれ、この例のようにバックスラッシュは含まれません）: `https:\\www.myfictionalsite.com/categories/admin/home.do`、 *架空の* URL: `https:\\www.myfictionalsite.com`.

1. In [!DNL Adobe Dynamic Media Classic]に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]**.
1. アプリケーションの一般設定ページの **[!UICONTROL Test&amp;Target サーバ名]** 「 」フィールドに、手順 2 でコピーした URL を貼り付けます。
1. 選択 **[!UICONTROL 閉じる]**.
