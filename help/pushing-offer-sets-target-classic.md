---
title: オファーセットのAdobeターゲットクラシックへのプッシュ
seo-title: オファーセットのAdobeターゲットクラシックへのプッシュ
description: 'null'
seo-description: オファーセットをAdobe Professional Classicにプッシュする方法を説明します。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# オファーセットのAdobeターゲットクラシックへのプッシュ{#pushing-offer-sets-to-adobe-target-classic}

オファーセットを作成または編集した後、次の手順に従ってターゲットクラシックにプッシュします。

1. ターゲットクラシックオファーセット画面で、「プッシュオファー」ボタンをクリックします。
1. ログイン情報を入力します。
1. 「ログイン」ボタンをクリックします。

S7_は、ターゲットクラシックへの転送中に、プレフィックスS7_が自動的にオファー名の開始に付加される。 このプレフィックスは、Dynamic Media Classicオファーをターゲットクラシックオファーリストで簡単に見つけられるように追加されています。 例えば、オファーは、「S7_&lt;オファーセット名>_&lt;オファー名>」のように表示されます。

SPSは、ターゲットクラシックWidgetオファーにプッシュ ウィジェットオファーを使用して、Widget Classicの外部で独自のオファーコンテンツをターゲットできます。 ウィジェットオファーは、Widget Classicの外部でホストされる標準オファーに似ています。 これにより、ターゲットClassicでオファーに保存されたサーバーコンテンツをデプロイし、より高度で動的な使用を実現できます。 ウィジェットオファーは、URLからコンテンツを取得し、約2時間そのコンテンツをキャッシュして提供します。 ウィジェットオファーは、Widget Classic以外の他のオファーが使用できない、動的コンテンツ生成機能をターゲットに提供します。 If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. これらのパラメーターは、ウィジェットオファーURLで利用できるサービスによって使用され、mboxの製品情報や注文情報を使用するWidget Classicの外部のターゲットを返すために使用できます。 また、ウィジェットオファーはAPIを通じてアクセスし、Widget Classicの外部でオファーをプログラム的に作成することもできます。
