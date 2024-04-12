---
title: Adobe Dynamic Media ClassicとAdobe Target Standard/Premium の統合
description: Adobe Dynamic Media ClassicをAdobe Target Standard/Premium と統合する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: c6f217fb-89cb-4c8d-aa7f-309fc42f7d46
topic: Integrations, Development
level: Experienced
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '149'
ht-degree: 0%

---

# Adobe Dynamic Media ClassicとAdobe Target Standard/Premium の統合 {#integrating-dmc-with-target}

統合する前に [!DNL Adobe Dynamic Media Classic] （を使用） [!DNL Target Standard/Premium]にターゲット URL を入力する必要があります [!DNL Adobe Dynamic Media Classic] アプリケーションの一般設定画面 ターゲット URL を取得し、アプリケーションの一般設定ページに入力するには、次の手順を実行します。

1. 対象： [!DNL Adobe Experience Cloud]、にログイン [!DNL Target Standard/Premium] アカウント。
1. ログイン後、ブラウザーのアドレスバーに URL を以下の値までコピーします `.com`.

   例えば、 *架空の* アドレスバーの URL （この例のように、URL パスには常にスラッシュが含まれ、バックスラッシュは含まれません）は、です。 `https:\\www.myfictionalsite.com/categories/admin/home.do`、の該当する部分のみをコピー *架空の* URL: `https:\\www.myfictionalsite.com`.

1. 対象： [!DNL Adobe Dynamic Media Classic]に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]**.
1. アプリケーションの一般設定ページの **[!UICONTROL Test&amp;Target サーバー名]** フィールドに、手順 2 でコピーした URL をペーストします。
1. を選択 **[!UICONTROL 閉じる]**.
