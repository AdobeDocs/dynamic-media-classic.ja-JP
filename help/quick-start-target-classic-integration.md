---
title: 「クイックスタート:Target Classicの統合」
seo-title: 「クイックスタート:Target Classicの統合」
description: 'null'
seo-description: Target Classicの統合テクニックをすばやく習得できるように、はじめにおよびクイックスタートについて説明します。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/target_ classic_ integration
discoiquuid: f8c25768- cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# クイックスタート:Target Classicの統合{#quick-start-target-classic-integration}

Adobe Target Classicは、複数のA/Bテストおよび多変量テストを迅速かつ継続的に実行し、有効性を測定し、セグメント化、ターゲティング、自動パーソナライゼーションを通じてオンラインコンテンツの関連性を向上させるためのコントロールをマーケティング担当者に提供します。

Scene7Publishing Systemを使用すると、Target Classicキャンペーン用のオファーおよびオファーセットを作成できます。例えば、同じリッチメディアアセットの3つのバリエーションを含むオファーセットを作成できます。次に、Target Classicにより、どのアセットがコンバージョンの上昇率を高めるかを判断できます。基本テンプレートまたは個々の画像からオファーやオファーセットを作成できます。オファーセットをAdobe Target Classicにプッシュまたは保存して、オファーがmboxおよびエクスペリエンスに関連付けられると、Target Classicはキャンペーンを実行して、クリックスルーおよびコンバージョンに最適なWebサイトのバリエーションを判断できます。

ダイナミックダイナミックMedia Classicコンテンツをよりカスタマイズするには、Target Classic HTMLオファーを使用します。詳しくは、Target Classic製品ドキュメントを参照してください。

>[!NOTE]
>
>Target ClassicをScene7Publishing Systemと共に使用するには、有効なAdobe Target Classicアカウントが必要です。

**クイックスタート**

ここでは、Target Classic HTMLオファーセットの操作方法をすばやく習得できるように、手順について簡潔に説明します。手順 1 ～ 3 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

**1. Enter your Target Classic URL in the Application General Settings screen.**

Dynamic Media ClassicではTarget Classic URLをTarget Classicと統合する必要があります。Copy the portion of your Target Classic URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. Dynamic Media Classic [とTarget Classic](integrating-scene7-target-classic.md#integrating_scene7_with_target_classic)の統合を参照してください。

**2．オファーセットの作成**

オファーセットを作成するには、パラメータ化テンプレートまたは画像を使用します。HTMLオファーセットは、Target Classicオファーセット画面で作成します。To open this screen, select your template or images, and click **Build** &gt; **Target Classic Offer Set**.

テンプレートを使用してオファーを作成するには、 **「追加とプレビュー**」をクリックします。追加とプレビュー画面で、パラメータの値を変更します。

画像を使用してオファーを作成するには、画像をTarget Classicオファーセット画面にドラッグします。**「プレビュー」** をクリックして、オファーセット内の画像またはすべての画像の画像プリセットを選択します。

作成したら、オファーセットを保存します。

詳しくは、[オファーセットの作成](creating-offer-set.md#creating_an_offer_set)を参照してください。

**3. Push the offer set to Target Classic**

In the Target Classic Offer Set screen, click **Push Offers**, and enter your login credentials in the Target Classic Login dialog box. See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).
