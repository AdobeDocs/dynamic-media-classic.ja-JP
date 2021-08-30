---
title: 「クイックスタート：Adobe Target Standard/Premiumとの統合»
description: AdobeDynamic Media ClassicのAdobe Target Standard/Premium統合テクニックをすばやく習得できる、Adobe Target Standard/Premiumの概要とクイックスタート。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 11%

---

# クイックスタート：Adobe Target Standard/Premiumの統合{#quick-start-target-integration}

Adobe Target Standard/Premiumでは、複数のA/Bテストと多変量分析テストを迅速かつ継続的に実行し、効果を測定し、セグメント化、ターゲティング、Automated Personalizationを通じてオンラインコンテンツの関連性を高めるために、マーケティング担当者が直接制御をおこないます。

AdobeDynamic Media Classicを使用すると、Adobe Target Standard/Premiumキャンペーン用のオファーおよびオファーセットを作成できます。 例えば、同じリッチメディアアセットの3つのバリエーションを含むオファーセットを作成できます。 次に、Adobe Target Standard/Premiumでコンバージョンの上昇率を高めるアセットを決定できます。 基本テンプレートまたは個々の画像からオファーやオファーセットを作成できます。オファーセットがAdobe Target Standard/Premiumにプッシュまたは保存され（オファーがmboxおよびエクスペリエンスに関連付けられる）、Adobe Target Standard/Premiumでキャンペーンを実行できます。 これらのキャンペーンは、クリックスルーとコンバージョンに対して最も効果が高いWebサイトのバリエーションを特定します。

動的なAdobeDynamic Media Classicコンテンツをより詳細にカスタマイズするには、 Adobe Target Standard/PremiumのHTMLオファーを使用します。 詳しくは、[Adobe Target Standard/Premiumの製品ドキュメント](https://experienceleague.adobe.com/docs/target.html)を参照してください。

>[!NOTE]
>
>Adobe Target Standard/PremiumをAdobeDynamic Media Classicで使用するには、有効なAdobe Target Standard/Premiumアカウントが必要です。

このクイックスタートは、Adobe Target Standard/PremiumのHTMLオファーセットをすぐに使い始められるように設計されています。 手順 1 ～ 3 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

## 1.アプリケーションの一般設定ページで、Adobe Target Standard/PremiumのURLを入力します。

AdobeDynamic Media ClassicをAdobe Target Standard/Premiumと統合するには、Adobe Target Standard/PremiumのURLが必要です。 Adobe Target Standard/Premium URLの先頭から`.com`までをコピーし、Dynamic Media Classicの&#x200B;**[!UICONTROL Adobeの一般設定]**&#x200B;ページの&#x200B;**[!UICONTROL サーバー]**&#x200B;グループの&#x200B;**[!UICONTROL Test&amp;Targetサーバー名]**&#x200B;テキストフィールドに入力します。 [AdobeDynamic Media ClassicとAdobe Target Standard/Premiumの統合](integrating-dmc-with-target.md#integrating-dmc-with-target)を参照してください。

## 2. オファーセットの作成

オファーセットを作成するには、パラメータ化テンプレートまたは画像を使用します。HTMLオファーセットは、 Test&amp;Targetオファーセットページで作成します。 このページを開くには、テンプレートまたは画像を選択し、グローバルナビゲーションバーで&#x200B;**[!UICONTROL Build]**/**[!UICONTROL Test&amp;Target Offer Set]**&#x200B;に移動します。

テンプレートを使用してオファーを作成するには、「**[!UICONTROL 追加とプレビュー]**」を選択します。 [追加とプレビュー]ページで、パラメータ値を変更します。

画像を使用してオファーを作成するには、画像をTest&amp;Targetオファーセットページにドラッグします。 「**[!UICONTROL プレビュー]**」を選択し、画像の画像プリセットを選択します。または、オファーセット内のすべての画像を選択します。

作成したら、オファーセットを保存します。

[オファーセットの作成](creating-offer-set.md#creating_an_offer_set)を参照してください。

## 3.オファーセットをAdobe Target Standard/Premiumにプッシュします。

Test&amp;Targetオファーセットページで、「**[!UICONTROL Push Offers]**」を選択し、Test&amp;Targetのログインダイアログボックスにログイン資格情報を入力します。 [Adobe Target Standard/Premiumへのオファーセットのプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target)を参照してください。
