---
title: オファーセットをAdobe Target標準/プレミアムにプッシュする
seo-title: オファーセットをAdobe Target標準/プレミアムにプッシュする
description: 'null'
seo-description: オファーセットをAdobe Target標準/プレミアムにプッシュする方法について説明します。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 5%

---


# オファーセットをAdobe Target標準/プレミアムにプッシュする {#pushing-offer-sets-to-target}

オファーセットを作成または編集した後、次の手順に従ってTarget Standard/プレミアムにプッシュします。

1. In the Test&amp;Target Offer Set screen, click **[!UICONTROL Push Offers]**.
1. クライアントコードとログイン資格情報を入力します。
1. 「**[!UICONTROL ログイン]**」をクリックします。

Target Standard/プレミアムへの転送中に、オファー名の開始にプリフィックスS7_が自動的に付加される。 このプレフィックスは、Test&amp;ClassicオファーリストでDynamic MediaClassicオファーを簡単に見つけられるように追加されています。 例えば、オファーは、「S7_&lt;オファーセット名>_&lt;オファー名>」のように表示されます。

Dynamic Mediaクラシックは、Target Standard/プレミアムウィジェットオファーにプッシュされます。 Widgetオファーを使用して、Target Standard/Premiumの外部で独自のオファーコンテンツをホストできます。 Widgetのオファーは、Target Standard/プレミウムの外部でホストされる標準のオファーに似ています。 Target Standard/Premiumでは、サーバーに保存されたオファーコンテンツをデプロイできるので、より高度で動的な使用方法が可能です。 ウィジェットオファーはURLからコンテンツを取得し、約2時間そのコンテンツをキャッシュして提供します。 ウィジェットオファーは、Target Standard/Premium以外の他のオファーが実行できない、動的コンテンツ生成機能を提供します。 If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. これらのパラメーターは、WidgetオファーURLで利用できるサービスによって、mboxからの商品や注文情報を使用するTarget Standard/Premiumの外部のコンテンツを返すために使用できます。 また、WidgetオファーにAPI経由でアクセスし、Target Standard/Premiumの外部でオファーをプログラム的に作成することもできます。
