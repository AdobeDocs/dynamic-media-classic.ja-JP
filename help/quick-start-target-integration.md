---
title: 「クイックスタート：Adobe Target Standard/Premiumとの統合»
description: Adobe Target Standard/Premium統合テクニックをすぐに使い始めるのに役立つ、Adobe Target Standard/Premiumの概要とクイックスタートです。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 12%

---

# クイックスタート：Adobe Target Standard/Premiumの統合{#quick-start-target-integration}

Adobe Target Standard/Premiumでは、複数のA/Bテストと多変量分析テストを迅速かつ継続的に実行し、効果を測定し、セグメント化、ターゲティング、自動パーソナライゼーションを通じてオンラインコンテンツの関連性を高めるために、マーケティング担当者が直接制御をおこないます。

Dynamic Media Classicを使用すると、Adobe Target Standard/Premiumキャンペーン用のオファーおよびオファーセットを作成できます。 例えば、同じリッチメディアアセットの3つのバリエーションを含むオファーセットを作成できます。 次に、Adobe Target Standard/Premiumでコンバージョンの上昇率を高めるアセットを決定できます。 基本テンプレートまたは個々の画像からオファーやオファーセットを作成できます。オファーセットがAdobe Target Standard/Premiumにプッシュまたは保存され（オファーがmboxおよびエクスペリエンスに関連付けられる）、Adobe Target Standard/Premiumでキャンペーンを実行できます。 これらのキャンペーンは、クリックスルーとコンバージョンに対して最も効果が高いWebサイトのバリエーションを特定します。

動的なDynamic Media Classicコンテンツをより詳細にカスタマイズするには、Adobe Target Standard/PremiumのHTMLオファーを使用します。 詳しくは、[Adobe Target Standard/Premiumの製品ドキュメント](https://experienceleague.adobe.com/docs/target.html)を参照してください。

>[!NOTE]
>
>Dynamic Media ClassicでAdobe Target Standard/Premiumを使用するには、有効なAdobe Target Standard/Premiumアカウントが必要です。

このクイックスタートは、Adobe Target Standard/PremiumのHTMLオファーセットをすぐに使い始められるように設計されています。 手順 1 ～ 3 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

## 1.アプリケーションの一般設定ページで、Adobe Target Standard/PremiumのURLを入力します。

Dynamic Media ClassicをAdobe Target Standard/Premiumと統合するには、Adobe Target Standard/PremiumのURLが必要です。 Adobe Target Standard/Premium URLの先頭から`.com`までをコピーし、Dynamic Media Classicの&#x200B;**[!UICONTROL アプリケーションの一般設定]**&#x200B;ページの&#x200B;**[!UICONTROL サーバー]**&#x200B;グループの&#x200B;**[!UICONTROL Test&amp;Target Server Name]**&#x200B;テキストフィールドに入力します。 [Dynamic Media ClassicとAdobe Target Standard/Premiumの統合](integrating-dmc-with-target.md#integrating-dmc-with-target)を参照してください。

## 2. オファーセットの作成

オファーセットを作成するには、パラメータ化テンプレートまたは画像を使用します。HTMLオファーセットは、 Test&amp;Targetオファーセットページで作成します。 このページを開くには、テンプレートまたは画像を選択し、グローバルナビゲーションバーで&#x200B;**[!UICONTROL ビルド]** / **[!UICONTROL Test&amp;Targetオファーセット]**&#x200B;をクリックします。

テンプレートを使用してオファーを作成するには、「**[!UICONTROL 追加とプレビュー]**」をクリックします。 [追加とプレビュー]ページで、パラメータ値を変更します。

画像を使用してオファーを作成するには、画像をTest&amp;Targetオファーセットページにドラッグします。 「**[!UICONTROL プレビュー]**」をクリックし、画像の画像プリセットを選択します。または、オファーセット内のすべての画像を選択します。

作成したら、オファーセットを保存します。

詳しくは、[オファーセットの作成](creating-offer-set.md#creating_an_offer_set)を参照してください。

## 3.オファーセットをAdobe Target Standard/Premiumにプッシュします。

Test&amp;Targetオファーセットページで、「**[!UICONTROL オファーをプッシュ]**」をクリックし、Test&amp;Targetのログインダイアログボックスにログイン資格情報を入力します。 [Adobe Target Standard/Premiumへのオファーセットのプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target)を参照してください。
