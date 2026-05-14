---
title: Adobe Target Standard/Premiumへのオファーセットのプッシュ
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
source-wordcount: 289
ht-degree: 0%

---

# Adobe Target Standard/Premiumへのオファーセットのプッシュ {#pushing-offer-sets-to-target}

オファーセットを作成または編集したら、次の手順に従ってAdobe Target Standard/Premiumにプッシュします。

1. Test&amp;Target オファーセット画面で、**[!UICONTROL プッシュオファー]**&#x200B;を選択します。
1. クライアントコードとログイン資格情報を入力します。
1. 「**[!UICONTROL ログイン]**」を選択します。

Adobe Target Standard/Premiumへの転送時に、オファー名の先頭に接頭辞`S7_`が自動的に付加されます。 この接頭辞は、Test&amp;Target オファーリストでAdobe Dynamic Media Classic オファーを簡単に見つけられるように添付されています。 例えば、オファーは`S7_<name of offer set>_<offer name>`と表示されます。

Adobe Dynamic Media Classicは、Adobe Target Standard/Premium ウィジェットのオファーにプッシュします。 Widget オファーを使用して、Adobe Target Standard/Premiumで独自の提供コンテンツをホストできます。 ウィジェットのオファーは、Adobe Target Standard/Prermiumがホストする標準オファーと似ています。 Adobe Target Standard/Premiumでは、サーバーに保存されたオファーコンテンツをデプロイできるため、より洗練された動的な使用が可能になります。 ウィジェットのオファーは、URLからコンテンツを取得し、そのコンテンツを約2時間キャッシュして配信できます。 Widgetのオファーは、Adobe Target Standard/Preimium以外のオファーでは提供されない、一部の動的コンテンツ生成機能を提供します。 オファーを配信するmboxに`mboxProductID`や`mbox.offerId`などのmbox パラメーターが含まれている場合、`productId=[PRODUCT_ID]`および`offerID=[OFFERID]`のURL パラメーターがリクエストされたURLに追加されます。 これらのパラメーターは、ウィジェットのオファーURLで利用できるサービスで使用され、mboxから商品または注文情報を使用するAdobe Target Standard/Premium以外のコンテンツを返します。 Widget オファーはAPIからもアクセスできるため、Adobe Target Standard/Premium以外でもプログラムでオファーを作成できます。
