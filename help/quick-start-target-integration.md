---
title: '「クイック開始: Target Standard/Premiumとの統合」'
seo-title: '「クイック開始: Target Standard/Premiumとの統合」'
description: 'null'
seo-description: Standard/PremiumのAdobe Targetテクニックをすばやく習得できるように、Target Standard標準/Premiumの概要と開始を簡単に説明します。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
translation-type: tm+mt
source-git-commit: 38f5cf5264f9775a225d354ed9dc2f6caee236f2
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 19%

---


# クイック開始: Target Standard/Premiumの統合{#quick-start-target-integration}

Adobe Target標準/プレミアムは、複数のA/Bおよび多変量分析テストを迅速かつ継続的に実行し、効果を測定し、セグメント化、ターゲティング、自動パーソナライゼーションを通じてオンラインコンテンツの関連性を高めるため、マーケターに直接管理を提供します。

Dynamic Mediaクラシックでは、Target Standard/プレミアムキャンペーン用のオファーとオファーセットを作成できます。 例えば、同じリッチメディアアセットの3つのバリエーションを含むオファーセットを作成できます。 次に、どのアセットがコンバージョン率を高めるかをTarget Standard/プレミアムで判断できます。 基本テンプレートまたは個々の画像からオファーやオファーセットを作成できます。オファーセットをMboxやエクスペリエンスに関連付けるWebサイトStandard/Premiumにプッシュまたは保存した後、Target Standard/Premiumはキャンペーンを実行して、クリックスルーとコンバージョンに最も適したWebサイトのバリエーションを特定できます。

動的なDynamic MediaのClassicコンテンツをさらにカスタマイズするには、Target Standard/プレミアムHTMLオファーを使用します。 詳しくは、Target Standard/プレミアムの製品ドキュメントを参照してください。

>[!NOTE]
>
>Dynamic MediaClassicでTarget Standard/プレミアムを使用するには、有効なAdobe Target標準/プレミアムアカウントが必要です。

**クイック開始**

このクイック開始では、Target Standard/プレミアムのHTMLオファーセットをすばやく習得できます。 手順 1 ～ 3 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

**1.Enter your Target Standard/Premium URL in the Application General Settings screen.**

Dynamic MediaクラシックをTarget Standard/プレミアムと統合するには、Target Standard/プレミアムURLが必要です。 Copy the portion of your Target Standard/Premium URL up to and including *.com*, and enter it in the Dynamic Media Classic Application General Settings screen. 詳しくは、Dynamic MediaClassicとTarget Standard/プレミアムの [統合を参照してください](integrating-dmc-with-target.md#integrating-dmc-with-target)。

**2．オファーセットの作成**

オファーセットを作成するには、パラメータ化テンプレートまたは画像を使用します。HTML オファーセットは、Test&amp;Target オファーセット画面で作成します。To open this screen, select your template or images, and click **Build** > **Test&amp;Target Offer Set**.

テンプレートを使用してオファーを作成するには、「 **&amp;追加プレビュー**」をクリックします。 &amp;プレビュー追加画面で、パラメータ値を変更します。

画像を使用してオファーを作成するには、画像を Test&amp;Target オファーセット画面内にドラッグします。Click **Preview** to choose an Image Preset for an image or all the images in the offer set.

作成したら、オファーセットを保存します。

詳しくは、[オファーセットの作成](creating-offer-set.md#creating_an_offer_set)を参照してください。

**3. オファーセットをTarget Standard/プレミアムにプッシュ**

In the Test&amp;Target Offer Set screen, click **Push Offers**, and enter your login credentials in the Test&amp;Target Login dialog box. 詳しくは、 [オファーセットのTarget Standard/プレミアムへのプッシュを参照してください](pushing-offer-sets-target.md#pushing_offer_sets_to_target)。
