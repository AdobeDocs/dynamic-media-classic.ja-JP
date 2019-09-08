---
title: Adobe Target Classicへのオファーセットのプッシュ
seo-title: Adobe Target Classicへのオファーセットのプッシュ
description: 'null'
seo-description: Adobe Target Classicにオファーセットを表示する方法について説明します。
uuid: 8c895a7c-21b4-4d85-8b0b- a3d2a420bf2e
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/target_ classic_ integration
discoiquuid: 39a05654-4f66-4f1e- bold5- lete6d174353f
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Adobe Target Classicへのオファーセットのプッシュ{#pushing-offer-sets-to-adobe-target-classic}

オファーセットを作成または編集したら、次の手順に従ってTarget Classicにプッシュします。

1. Target Classicオファーセット画面で、「オファーをプッシュ」ボタンをクリックします。
1. ログイン情報を入力します。
1. 「ログイン」ボタンをクリックします。

Target Classicへの転送中に、オファー名の先頭にプレフィックスS7_が自動的に付加されます。このプレフィックスは、Target ClassicオファーリストでDynamic Media Classicオファーを簡単に見つけることができるようにアタッチされます。例えば、オファーは、「S7_&lt;オファーセット名&gt;_&lt;オファー名&gt;」のように表示されます。

SPSはTarget Classicウィジェットオファーにプッシュします。ウィジェットオファーを使用すると、Target Classicの外部で独自のオファーコンテンツをホストできます。ウィジェットオファーは、Target Classicの外部でホストされる標準的なオファーに似ています。Target Classicでは、サーバーに保存されているオファーコンテンツを配信し、より高度で動的な使用を可能にすることができます。ウィジェットオファーはURLからコンテンツを取得し、約2時間そのコンテンツをキャッシュして提供します。ウィジェットオファーは、Target Classicの外部の他のオファーが提供しない動的コンテンツ生成機能を提供します。If the mbox serving the offer contains mbox parameters such as `mboxProductID` and `mbox.offerId`, the `productId=[PRODUCT_ID]`and `offerID=[OFFERID]` URL parameters are appended to the requested URL. これらのパラメーターは、ウィジェットオファーURLにあるサービスで使用して、mboxからの製品情報または注文情報を使用するTarget Classicの外部のコンテンツを返すことができます。また、ウィジェットオファーはAPI経由でアクセスして、Target Classicの外部でオファーをプログラム的に作成することもできます。
