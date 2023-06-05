---
title: オファーセットをAdobe Target Standard/Premium にプッシュ
description: Adobe Dynamic Media ClassicからAdobe Target Standard/Premium にオファーセットをプッシュする方法について説明します。
uuid: 8c895a7c-21b4-4d85-8b0b-a3d2a420bf2e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 39a05654-4f66-4f1e-aec5-ebe6d174353f
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# オファーセットをAdobe Target Standard/Premium にプッシュ {#pushing-offer-sets-to-target}

オファーセットを作成または編集した後、次の手順に従って、Adobe Target Standard/Premium にプッシュします。

1. Test&amp;Target オファーセット画面で、「 **[!UICONTROL オファーをプッシュ]**.
1. クライアントコードとログイン資格情報を入力します。
1. 選択 **[!UICONTROL ログイン]**.

Adobe Target Standard/Premium への転送時に、 `S7_` は、オファー名の先頭に自動的に添付されます。 Test&amp;Target のオファーリストでAdobe Dynamic Media Classicオファーを簡単に見つけられるように、このプレフィックスが付加されています。 例えば、オファーは `S7_<name of offer set>_<offer name>`.

Adobe Dynamic Media ClassicはAdobe Target Standard/Premium ウィジェットオファーをプッシュします。 ウィジェットオファーを使用すると、Adobe Target Standard/Premium の外部で独自のオファーコンテンツをホストできます。 ウィジェットオファーは、Adobe Target Standard/Premium の外部でホストされる標準オファーに似ています。 Adobe Target Standard/Premium では、サーバーに保存されたオファーコンテンツをデプロイして、より高度で動的な使用を実現します。 ウィジェットオファーでは、URL からコンテンツを取得し、そのコンテンツをキャッシュして約 2 時間提供できます。 ウィジェットオファーは、Adobe Target Standard/Premium 以外のオファーでは実現できない、動的コンテンツ生成機能を提供します。 オファーを提供する mbox に、次のような mbox パラメーターが含まれている場合。 `mboxProductID` および `mbox.offerId`、 `productId=[PRODUCT_ID]`および `offerID=[OFFERID]` URL パラメーターがリクエストされた URL に追加されます。 これらのパラメーターは、Widget のオファー URL で利用できるサービスによって使用され、mbox からの製品情報や注文情報を使用するAdobe Target Standard/Premium 外のコンテンツを返すことができます。 また、ウィジェットオファーには、API を通じてアクセスし、Adobe Target Standard/Premium 以外でオファーをプログラムによって作成することもできます。
