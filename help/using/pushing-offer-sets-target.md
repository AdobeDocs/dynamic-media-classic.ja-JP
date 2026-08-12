---
title: オファーセットをAdobe Target Standard/Premiumにプッシュ
description: Adobe Dynamic Media ClassicからAdobe Target Standard/Premiumにオファーセットをプッシュする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:55:22.850Z'
TQID: 'https://experienceleague.adobe.com/8j9sRn1zhAhgj-wMV6hYix1F9aARZjDUiFZofcVVcBw'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 8a9d304ced3a218ae6393961a278f5ab9581c229
workflow-type: tm+mt
source-wordcount: 283
ht-degree: 0%

---

# Adobe Target Standard/Premiumへのオファーセットのプッシュ {#pushing-offer-sets-to-target}

オファーセットを作成または編集したら、次の手順に従ってAdobe Target Standard/Premiumにプッシュします。

1. テストとターゲットオファーセット画面で、**[!UICONTROL プッシュオファー]**&#x200B;を選択します。
1. クライアントコードとログイン資格情報を入力します。
1. 「**[!UICONTROL ログイン]**」を選択します。

Adobe Target Standard/Premiumへの転送時に、オファー名の先頭にプレフィックス `S7_`が自動的に追加されます。 この接頭辞が追加され、テストとターゲットのオファーリストでAdobe Dynamic Media Classic オファーを簡単に見つけられるようになりました。 例えば、オファーは`S7_<name of offer set>_<offer name>`と表示されます。

Adobe Dynamic Media Classicは、ウィジェットオファーをAdobe Target Standard/Premiumにプッシュします。 Widget オファーを使用して、提供されたコンテンツをAdobe Target Standard/Premiumでホストできます。 ウィジェットオファーは、Adobe Target Standard/Premiumがホストする標準オファーと同等です。 Adobe Target Standard/Premiumでは、サーバーに保存されたオファーコンテンツをデプロイできるため、より高度で動的な使用が可能になります。 Widgetでは、URLからコンテンツを取得し、そのコンテンツを2時間キャッシュして提供します。 Widgetのオファーは、Adobe Target Standard/Premium以外のオファーでは提供されない、一部の動的コンテンツ生成機能を提供します。 オファーを配信するmboxに`mboxProductID`や`mbox.offerId`などのmbox パラメーターが含まれている場合、`productId=[PRODUCT_ID]`と`offerID=[OFFERID]`のURL パラメーターがリクエストされたURLに追加されます。 Widget オファーURLで利用可能なサービスは、これらのパラメーターを使用して、mboxの商品情報または注文情報を使用するAdobe Target Standard/Premium以外のコンテンツを返します。 Widget オファーはAPIからもアクセスできるため、Adobe Target Standard/Premium以外でもプログラムでオファーを作成できます。
