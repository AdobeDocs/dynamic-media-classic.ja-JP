---
title: 「クイックスタート：Adobe Target Standard と Premium の統合」
description: Adobe Dynamic Media ClassicでAdobe Target Standard と Premium を統合する手法をすぐに使い始めるのに役立つ、Adobe Target Standard と Premium の概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# クイックスタート：Adobe Target Standard と Premium の統合{#quick-start-target-integration}

Adobe Target Standard/Premium は、マーケターの管理下に置かれます。 これにより、複数の A/B テストや多変量分析テストを迅速かつ継続的に実行し、有効性を測定できます。 また、セグメント化、ターゲット設定、Automated Personalizationを通じて、オンラインコンテンツの関連性を高めることができます。

Adobe Dynamic Media Classicでは、Adobe Target Standard/Premium キャンペーン用のオファーおよびオファーセットを作成できます。 例えば、同じリッチメディアアセットの 3 つのバリエーションでオファーセットを作成できます。 次に、Adobe Target Standard または Premium で、どのアセットのコンバージョン上昇率が高いかを判断できます。 オファーとオファーセットは、基本テンプレートまたは個々の画像から作成できます。 オファーセットがAdobe Target Standard/Premium にプッシュまたは保存された後（オファーが mbox とエクスペリエンスに関連付けられている場合）、Adobe Target Standard/Premium はキャンペーンを実行できます。 これらのキャンペーンは、クリックスルーとコンバージョンに最も効果が高い web サイトのバリエーションを決定します。

動的なAdobe Dynamic Media Classic コンテンツをカスタマイズする場合は、Adobe Target Standard/Premium のHTMLオファーを利用してください。 を参照してください。 [Adobe Target Standard/Premium 製品ドキュメント](https://experienceleague.adobe.com/en/docs/target) を参照してください。

>[!NOTE]
>
>Adobe Dynamic Media ClassicでAdobe Target Standard/Premium を使用するには、有効なAdobe Target Standard/Premium アカウントが必要です。

このクイックスタートは、Adobe Target Standard/PremiumHTMLオファーセットをすぐに使い始められるように設計されています。 手順 1 ～ 3 に従ってください。各手順に続いて、詳細な情報を見つけることができるトピックの見出しへの相互参照があります。

## 1. アプリケーションの一般設定ページにAdobe Target Standard/Premium の URL を入力します

Adobe Dynamic Media ClassicをAdobe Target Standard/Premium と統合するには、Adobe Target Standard/Premium の URL が必要です。 Adobe Target Standard/Premium URL の一部を次の値までコピーします。 `.com`を選択し、Adobe Dynamic Media Classicに入力します **[!UICONTROL アプリケーションの一般設定]** ページ （内） **[!UICONTROL サーバー]** グループ、 **[!UICONTROL Test&amp;Target サーバー名]** テキストフィールド。 参照： [Adobe Dynamic Media ClassicとAdobe Target Standard/Premium の統合](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. オファーセットの作成

パラメーター化されたテンプレートまたは画像を使用してオファーセットを作成します。 HTMLオファーセットは、Test&amp;Target オファーセット ページで作成できます。 このページを開くには、テンプレートまたは画像を選択し、グローバルナビゲーションバーで以下に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL Test&amp;Target オファーセット]**.

テンプレートを使用してオファーを作成するには、次を選択します。 **[!UICONTROL 追加とプレビュー]**. 「追加とプレビュー」ページで、パラメーター値を変更します。

画像を使用してオファーを作成するには、画像を Test&amp;Target オファーセット ページにドラッグします。 を選択 **[!UICONTROL プレビュー]** 特定の画像またはオファーセット内のすべての画像の画像プリセットを選択します。

オファーセットの作成後に保存します。

参照： [オファーセットの作成](creating-offer-set.md#creating_an_offer_set).

## 3. オファーセットをAdobe Target Standard/Premium にプッシュする

Test&amp;Target オファーセットページで、 **[!UICONTROL プッシュオファー]**&#x200B;をクリックし、Test&amp;Target ログイン ダイアログボックスにログイン資格情報を入力します。 参照： [オファーセットをAdobe Target Standard/Premium にプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
