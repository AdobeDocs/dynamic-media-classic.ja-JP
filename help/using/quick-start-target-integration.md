---
title: 「クイックスタート：Adobe Target Standard/Premium の統合»
description: Adobe Dynamic Media ClassicのAdobe Target Standard/Premium 統合テクニックをすばやく習得できるようにする、Adobe Target Standard/Premium の概要とクイックスタートです。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 7%

---

# クイックスタート：Adobe Target Standard/Premium の統合{#quick-start-target-integration}

Adobe Target Standard/Premium では、複数の A/B テストと多変量分析テストを迅速かつ継続的に実行し、効果を測定し、セグメント化、ターゲティング、Automated Personalizationを通じてオンラインコンテンツの関連性を高めるために、マーケターが直接制御をおこないます。

Adobe Dynamic Media Classicでは、Adobe Target Standard/Premium キャンペーン用のオファーおよびオファーセットを作成できます。 例えば、同じリッチメディアアセットの 3 つのバリエーションを含むオファーセットを作成できます。 その後、Adobe Target Standard/Premium で、コンバージョン上昇率の高いアセットを特定できます。 基本テンプレートまたは個々の画像からオファーやオファーセットを作成できます。オファーセットがAdobe Target Standard/Premium にプッシュまたは保存され、そのオファーが mbox およびエクスペリエンスに関連付けられると、Adobe Target Standard/Premium はキャンペーンを実行できます。 これらのキャンペーンは、クリックスルーとコンバージョンに対して最も効果が高い Web サイトのバリエーションを特定します。

動的なAdobe Dynamic Media Classicコンテンツをさらにカスタマイズするには、Adobe Target Standard/PremiumHTMLオファーを使用します。 詳しくは、 [Adobe Target Standard/Premium 製品ドキュメント](https://experienceleague.adobe.com/docs/target.html) を参照してください。

>[!NOTE]
>
>Adobe Dynamic Media ClassicでAdobe Target Standard/Premium を使用するには、有効なAdobe Target Standard/Premium アカウントが必要です。

このクイックスタートは、Adobe Target Standard/Premium のHTMLオファーセットをすぐに使い始めるためのものです。 手順 1 ～ 3 に従ってください。各手順の後に、トピックの見出しへの相互参照があり、詳細を確認できます。

## 1.アプリケーションの一般設定ページで、Adobe Target Standard/Premium の URL を入力します。

Adobe Dynamic Media ClassicをAdobe Target Standard/Premium と統合するには、Adobe Target Standard/Premium の URL が必要です。 Adobe Target Standard/Premium URL の部分を、を含むまでコピーします。 `.com`をクリックし、Adobe Dynamic Media Classicに入力します。 **[!UICONTROL アプリケーションの一般設定]** ページの **[!UICONTROL サーバー]** グループ **[!UICONTROL Test&amp;Target サーバ名]** テキストフィールド。 詳しくは、 [Adobe Dynamic Media ClassicとAdobe Target Standard/Premium の統合](integrating-dmc-with-target.md#integrating-dmc-with-target).

## 2. オファーセットの作成

オファーセットを作成するには、パラメータ化テンプレートまたは画像を使用します。HTMLオファーセットは、 Test&amp;Target オファーセットページで作成します。 このページを開くには、テンプレートまたは画像を選択し、グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL Test&amp;Target オファーセット]**.

テンプレートを使用してオファーを作成するには、「 **[!UICONTROL 追加とプレビュー]**. [ 追加とプレビュー ] ページで、パラメータ値を変更します。

画像を含むオファーを作成するには、画像を Test&amp;Target オファーセットページにドラッグします。 選択 **[!UICONTROL プレビュー]** をクリックして、画像またはオファーセット内のすべての画像の画像プリセットを選択します。

作成したら、オファーセットを保存します。

詳しくは、 [オファーセットの作成](creating-offer-set.md#creating_an_offer_set).

## 3.オファーセットをAdobe Target Standard/Premium にプッシュします

Test&amp;Target オファーセットページで、「 」を選択します。 **[!UICONTROL オファーをプッシュ]**&#x200B;をクリックし、Test&amp;Target のログインダイアログボックスにログイン資格情報を入力します。 詳しくは、 [オファーセットをAdobe Target Standard/Premium にプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target).
