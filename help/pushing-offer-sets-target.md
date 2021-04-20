---
title: オファーセットをAdobe Target標準/プレミアムにプッシュする
description: オファーセットをAdobe Target標準/プレミアムにプッシュする方法について説明します。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 5%

---


# オファーセットをAdobe Target標準/プレミアムにプッシュ{#pushing-offer-sets-to-target}

オファーセットを作成または編集した後、次の手順に従ってTarget Standard/Premiumにプッシュします。

1. テストターゲットオファーセット画面で、「**[!UICONTROL オファーをプッシュ]**」をクリックします。
1. クライアントコードとログイン資格情報を入力します。
1. 「**[!UICONTROL ログイン]**」をクリックします。

Target Standard/Premiumへの転送中に、オファー名の開始にプリフィックスS7_が自動的に付加されます。 このプレフィックスは、Test&amp;ClassicオファーをTest&amp;ターゲットオファーリストで簡単に見つけられるように追加されています。 例えば、オファーは、「S7_&lt;オファーセット名>_&lt;オファー名>」のように表示されます。

Dynamic Mediaクラシックは、Target Standard/Premiumのウィジェットオファーにプッシュします。 Widgetオファーを使用して、Target Standard/Premiumの外部で独自のオファーコンテンツをホストできます。 ウィジェットのオファーは、Target Standard/Premiumの外部でホストされる標準のオファーに似ています。 Target Standard/Premiumでは、サーバーに保存されたオファーコンテンツをデプロイできるので、より高度で動的な使用方法が可能です。 ウィジェットオファーはURLからコンテンツを取得し、約2時間そのコンテンツをキャッシュして提供します。 ウィジェットオファーは、Target Standard/Premium以外の他のオファーが実行できない、動的コンテンツ生成機能を提供します。 オファーを提供するmboxに、`mboxProductID`や`mbox.offerId`などのmboxパラメーターが含まれる場合、リクエストされたURLに`productId=[PRODUCT_ID]`や`offerID=[OFFERID]`のURLパラメーターが追加されます。 これらのパラメーターは、ウィジェットオファーURLで利用できるサービスによって、mboxからの製品情報や注文情報を使用するTarget Standard/Premiumの外部のコンテンツを返すために使用できます。 また、ウィジェットオファーはAPIを介してアクセスし、Target Standard/Premium以外でプログラム的にオファーを作成することもできます。
