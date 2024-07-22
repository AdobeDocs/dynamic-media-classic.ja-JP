---
title: オファーセットをAdobe Target Standard/Premium にプッシュ
description: Adobe Dynamic Media ClassicからAdobe Target Standard/Premium にオファーセットをプッシュする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 778fd54b-a9e5-40c5-aff1-a156a5c15923
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---

# オファーセットをAdobe Target Standard/Premium にプッシュ {#pushing-offer-sets-to-target}

オファーセットを作成または編集した後、次の手順に従ってオファーセットをAdobe Target Standard/Premium にプッシュします。

1. Test&amp;Target オファーセット画面で、「**[!UICONTROL プッシュオファー]**」を選択します。
1. クライアントコードとログイン資格情報を入力します。
1. **[!UICONTROL ログイン]** を選択します。

Adobe Target Standard/Premium への転送中に、オファー名の先頭に `S7_` というプレフィックスが自動的に付加されます。 このプレフィックスは、Test&amp;Target オファーリストでAdobe Dynamic Media Classic オファーを簡単に見つけられるように付加されます。 例えば、オファーは `S7_<name of offer set>_<offer name>` のように表示されます。

Adobe Dynamic Media Classicは、Adobe Target Standard/Premium ウィジェットオファーにプッシュします。 ウィジェットオファーを使用して、独自に提供されたコンテンツをAdobe Target Standard/Premium でホストできます。 ウィジェットオファーは、Adobe Target Standard/Premium がホストする標準オファーに似ています。 Adobe Target Standard/Premium で、サーバーに保存されたオファーコンテンツをデプロイできるので、より高度で動的な使用が可能になります。 ウィジェットオファーでは、URL からコンテンツを取得し、そのコンテンツを約 2 時間キャッシュして提供できます。 Widget オファーは、Adobe Target Standard/Preimium 以外の他のオファーにはない、動的コンテンツ生成機能を提供します。 オファーを提供する mbox に `mboxProductID` や `mbox.offerId` などの mbox パラメーターが含まれている場合、リクエストされた URL に `productId=[PRODUCT_ID]` と `offerID=[OFFERID]` の URL パラメーターが追加されます。 これらのパラメーターは、ウィジェットオファー URL で利用可能なサービスによって、mbox の商品または注文情報を使用するAdobe Target Standard/Premium 外のコンテンツを返すために使用されます。 このウィジェットオファーには API を通じてアクセスすることもできるので、Adobe Target Standard/Premium 以外でプログラムによってオファーを作成できます。
