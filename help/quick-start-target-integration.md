---
title: 「クイック開始:Target Standard/Premiumの統合」
description: Target Standard/Premiumの統合テクニックをすばやく習得できるように、Adobe Target Standard/Premiumの概要とクイック開始を紹介します。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Mediaクラシック
role: データエンジニア、管理者、実業家
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 19%

---


# クイック開始:Adobe Target標準/プレミアム統合{#quick-start-target-integration}

Adobe Target標準/Premiumは、複数のA/Bおよび多変量分析テストを迅速かつ継続的に実行し、効果を測定し、セグメント化、ターゲティング、自動パーソナライゼーションを通じてオンラインコンテンツの関連性を高めるため、マーケターに直接管理を提供します。

Dynamic Mediaクラシックを使用すると、Target Standard/Premiumキャンペーン用のオファーとオファーセットを作成できます。 例えば、同じリッチメディアアセットの3つのバリエーションを含むオファーセットを作成できます。 次に、Target Standard/Premiumで、どのアセットがコンバージョン率が高いかを判断できます。 基本テンプレートまたは個々の画像からオファーやオファーセットを作成できます。オファーセットをMboxやエクスペリエンスに関連付けられたAdobe TargetStandard/Premiumにプッシュまたは保存した後、Target Standard/Premiumでキャンペーンを実行して、クリックスルーとコンバージョンに最も適したWebサイトのバリエーションを特定できます。

動的なDynamic Mediaクラシックコンテンツをさらにカスタマイズするには、Target Standard/PremiumのHTMLオファーを使用します。 詳しくは、Target Standard/Premium製品ドキュメントを参照してください。

>[!NOTE]
>
>Target Standard/PremiumをDynamic Mediaクラシックと共に使用するには、有効なAdobe Target標準/プレミアムアカウントが必要です。

**クイック開始**

このクイック開始では、Target Standard/PremiumのHTMLオファーセットをすばやく習得できるように設計されています。 手順 1 ～ 3 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

**1.アプリの全般設定画面で、Adobe Target標準/プレミアムURLを入力します。**

Dynamic MediaクラシックをTarget Standard/Premiumと統合するには、Target Standard/PremiumのURLが必要です。 Target Standard/Premium URLの先頭から&#x200B;*.com*&#x200B;までをコピーし、Dynamic Mediaクラシックアプリケーションの全般設定画面に入力します。 「[Target Standard/PremiumとのDynamic Mediaクラシックの統合](integrating-dmc-with-target.md#integrating-dmc-with-target)」を参照してください。

**2．オファーセットの作成**

オファーセットを作成するには、パラメータ化テンプレートまたは画像を使用します。HTML オファーセットは、Test&amp;Target オファーセット画面で作成します。この画面を開くには、テンプレートまたは画像を選択し、**ビルド**/**ターゲットオファーセット**&#x200B;をクリックします。

テンプレートを使用してオファーを作成するには、**追加 &amp;プレビュー**&#x200B;をクリックします。 &amp;プレビュー追加画面で、パラメータ値を変更します。

画像を使用してオファーを作成するには、画像を Test&amp;Target オファーセット画面内にドラッグします。「**プレビュー**」をクリックして、オファーセット内の画像またはすべての画像の画像プリセットを選択します。

作成したら、オファーセットを保存します。

詳しくは、[オファーセットの作成](creating-offer-set.md#creating_an_offer_set)を参照してください。

**3.オファーセットをAdobe Target標準/プレミアムにプッシュ**

テストターゲットオファーセット画面で、「**オファーをプッシュ**」をクリックし、Test&amp;ターゲットのログインダイアログボックスにログイン情報を入力します。 [Target Standard/Premiumへのオファーセットのプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target)を参照してください。
