---
title: オファーセットをAdobe Target標準/プレミアムにプッシュする
description: オファーセットをAdobe Target標準/プレミアムにプッシュする方法について説明します。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Mediaクラシック
role: Data Engineer,Administrator,Business Practitioner
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# オファーセットをAdobe Target標準/プレミアムにプッシュ{#pushing-offer-sets-to-target}

オファーセットを作成または編集した後、次の手順に従って、Adobe Target標準/プレミアムにプッシュします。

1. テストターゲットオファーセット画面で、「**[!UICONTROL オファーをプッシュ]**」をクリックします。
1. クライアントコードとログイン資格情報を入力します。
1. 「**[!UICONTROL ログイン]**」をクリックします。

Adobe Target標準/プレミアムへの転送中に、プレフィックス`S7_`がオファー名の開始に自動的に付加されます。 このプレフィックスは、Test&amp;ClassicオファーをTest&amp;ターゲットオファーリストで簡単に見つけられるように追加されています。 例えば、オファーは`S7_<name of offer set>_<offer name>`のように表示されます。

Dynamic Mediaクラシックは、Adobe Target標準/プレミアムウィジェットオファーにプッシュされます。 ウィジェットオファーを使用して、Adobe Target標準/プレミアムの外部で独自のオファーコンテンツをホストできます。 ウィジェットのオファーは、Adobe Target標準/プレミウムの外部でホストされる標準オファーに似ています。 Standard/Premiumでは、サーバーに保存されたオファーコンテンツをAdobe TargetStandard/Premiumでデプロイできるので、より高度で動的な使用が可能です。 ウィジェットオファーはURLからコンテンツを取得し、約2時間そのコンテンツをキャッシュして提供します。 ウィジェットオファーは、Adobe Target標準/プレミアム以外の他のオファーが実行できない、動的コンテンツ生成機能を提供します。 オファーを提供するmboxに、`mboxProductID`や`mbox.offerId`などのmboxパラメーターが含まれる場合、リクエストされたURLに`productId=[PRODUCT_ID]`や`offerID=[OFFERID]`のURLパラメーターが追加されます。 これらのパラメーターは、ウィジェットオファーのURLで利用できるサービスによって、mboxからの製品情報や注文情報を使用する、Adobe Target標準/プレミアム外のコンテンツを返すために使用できます。 また、WidgetオファーはAPIを介してアクセスし、Adobe Target標準/Premium以外でオファーをプログラム的に作成することもできます。
