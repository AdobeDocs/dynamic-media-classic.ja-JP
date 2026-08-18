---
title: クイックスタート：Adobe Target Standard/Premium統合
description: Adobe Dynamic Media ClassicのAdobe Target Standard/Premium統合手法を迅速に使い始めるための概要とAdobe Target Standard/Premiumのクイックスタート。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
topic: Integrations
level: Experienced
autotag-review: '2026-05-13T19:56:29.690Z'
TQID: 'https://experienceleague.adobe.com/urNoJw6SrzPpsfpoTtudKndZfJOmWsZKtBZ3Za4aE0I'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: 0f0abef2ec6e1d0743eca66e59673547f70ad7b0
workflow-type: tm+mt
source-wordcount: 529
ht-degree: 1%

---

# クイックスタート：Adobe Target Standard/Premium統合{#quick-start-target-integration}

Adobe Target Standard/Premiumは、マーケティング部門が管理的に管理できるようにします。 この機能により、複数のA/B テストと多変量テストを迅速かつ継続的に実行し、その効果を測定できます。 また、セグメンテーション、ターゲティング、Automated Personalizationを通じて、オンラインコンテンツの関連性を高めることができます。

Adobe Dynamic Media Classicでは、Adobe Target Standard/Premium キャンペーンのオファーとオファーセットを作成できます。 例えば、同じリッチメディアアセットの3つのバリエーションを含むオファーセットを作成できます。 そして、Adobe Target StandardまたはPremiumによって、どのアセットがより優れたコンバージョンパフォーマンスを提供するかを判断できます。 基本テンプレートまたは個々の画像から、オファーとオファーセットを作成できます。 オファーセットがAdobe Target Standard/Premiumにプッシュまたは保存され、オファーがmboxとエクスペリエンスに関連付けられると、Adobe Target Standard/Premiumでキャンペーンを実行できます。 こうした施策は、クリックスルーとコンバージョンに対して、web サイトのどのバリエーションが最も優れたパフォーマンスを発揮するかを判断します。

動的なAdobe Dynamic Media Classic コンテンツのカスタマイズを強化するには、Adobe Target Standard/Premium HTML オファーを使用します。 詳しくは、[Adobe Target Standard/Premium製品ドキュメント &#x200B;](https://experienceleague.adobe.com/ja/docs/target)を参照してください。

>[!NOTE]
>
>Adobe Dynamic Media ClassicでAdobe Target Standard/Premiumを使用するには、有効なAdobe Target Standard/Premium アカウントが必要です。

このガイドは、Adobe Target Standard/Premium HTML オファーセットをすばやく使用できるように設計されています。 手順 1 ～ 3 に従ってください。 各ステップの後、トピック見出しへの相互参照があり、詳細を確認できます。

## &#x200B;1. アプリケーションの一般設定ページにAdobe Target Standard/Premium URLを入力します

Adobe Dynamic Media Classicでは、Adobe Target Standard/Premiumと統合するために、Adobe Target Standard/Premium URLが必要です。 Adobe Target Standard/Premium URLの一部を`.com`までコピーし、Adobe Dynamic Media Classic **[!UICONTROL Application General Settings]** ページの&#x200B;**[!UICONTROL Servers]** グループ内の&#x200B;**[!UICONTROL Test&amp;Target Server Name]** テキストフィールドに入力します。 [Adobe Dynamic Media ClassicとAdobe Target Standard/Premiumの統合](integrating-dmc-with-target.md#integrating-dmc-with-target)を参照してください。

## &#x200B;2. オファーセットの作成

パラメータ化されたテンプレートまたは画像を使用して、オファーセットを作成します。 HTML オファーセットは、テストとターゲット オファーセット ページで作成できます。 このページを開くには、テンプレートまたは画像を選択し、グローバルナビゲーションバーで、**[!UICONTROL ビルド]** > **[!UICONTROL テスト&amp;ターゲットオファーセット]**&#x200B;に移動します。

テンプレートを使用してオファーを作成するには、**[!UICONTROL 追加とプレビュー]**&#x200B;を選択します。 「追加とプレビュー」ページで、パラメーター値を変更します。

画像を含むオファーを作成するには、画像をTest&amp;Target オファーセットページにドラッグします。 **[!UICONTROL プレビュー]**&#x200B;を選択し、画像またはオファーセット内のすべての画像の画像プリセットを選択します。

オファーセットを作成した後で、オファーセットを保存します。

[&#x200B; オファーセットの作成](creating-offer-set.md#creating_an_offer_set)を参照してください。

## &#x200B;3. オファーセットをAdobe Target Standard/Premiumにプッシュする

Test&amp;Target オファーセットページで、**[!UICONTROL プッシュオファー]**&#x200B;を選択し、Test&amp;Target ログインダイアログボックスにログイン資格情報を入力します。 Adobe Target Standard/Premium[&#128279;](pushing-offer-sets-target.md#pushing_offer_sets_to_target)へのオファーセットのプッシュを参照してください。
