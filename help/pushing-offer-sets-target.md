---
title: オファーセットをAdobe Target Standard/Premiumにプッシュ
description: AdobeDynamic Media ClassicからAdobe Target Standard/Premiumにオファーセットをプッシュする方法について説明します。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# オファーセットをAdobe Target Standard/Premiumにプッシュ {#pushing-offer-sets-to-target}

オファーセットを作成または編集した後、次の手順に従って、Adobe Target Standard/Premiumにプッシュします。

1. Test&amp;Targetオファーセット画面で、「**[!UICONTROL オファーをプッシュ]**」を選択します。
1. クライアントコードとログイン資格情報を入力します。
1. 「**[!UICONTROL ログイン]**」を選択します。

Adobe Target Standard/Premiumへの転送時に、オファー名の先頭にプレフィックス`S7_`が自動的に付加されます。 Test&amp;TargetのオファーリストでAdobeDynamic Media Classicオファーを簡単に見つけられるように、このプレフィックスが付加されています。 例えば、オファーは`S7_<name of offer set>_<offer name>`と表示されます。

AdobeDynamic Media Classicは、Adobe Target Standard/Premiumウィジェットオファーをプッシュします。 ウィジェットオファーを使用すると、Adobe Target Standard/Premiumの外部で独自のオファーコンテンツをホストできます。 ウィジェットオファーは、Adobe Target Standard/Prermiumの外部でホストされる標準オファーに似ています。 Adobe Target Standard/Premiumでは、サーバーに保存されたオファーコンテンツをデプロイして、より高度で動的な使用を可能にします。 ウィジェットオファーでは、URLからコンテンツを取得し、約2時間そのコンテンツをキャッシュして提供できます。 ウィジェットオファーは、Adobe Target Standard/Premium以外のオファーでは実現できない、動的コンテンツ生成機能を提供します。 オファーを提供するmboxに`mboxProductID`や`mbox.offerId`などのmboxパラメーターが含まれている場合、リクエストされたURLに`productId=[PRODUCT_ID]`および`offerID=[OFFERID]`のURLパラメーターが追加されます。 これらのパラメーターは、WidgetオファーURLで利用できるサービスで使用して、mboxの製品情報や注文情報を使用するAdobe Target Standard/Premium以外のコンテンツを返すことができます。 また、Widgetオファーには、APIを通じてアクセスし、Adobe Target Standard/Premium以外でプログラムによってオファーを作成することもできます。
