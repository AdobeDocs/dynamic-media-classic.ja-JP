---
title: 「クイック開始:Adobe TargetStandard/Premiumの連携»
description: Adobe Target標準/プレミアムの統合テクニックをすばやく習得できるように、Adobe Target標準/プレミアムの概要とクイック開始を紹介します。
uuid: d8f79fbf-8be1-44fa-8058-3508060fcd70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: f8c25768-cf59-45ec-8193-522404191d57
feature: Dynamic Mediaクラシック
role: Data Engineer,Administrator,Business Practitioner
exl-id: 4745ace5-7825-468e-8a82-bfbbcf1b0440
translation-type: tm+mt
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 12%

---

# クイック開始:Adobe Target標準/プレミアム統合{#quick-start-target-integration}

Adobe Target標準/Premiumは、複数のA/Bおよび多変量分析テストを迅速かつ継続的に実行し、効果を測定し、セグメント化、ターゲティング、自動パーソナライゼーションを通じてオンラインコンテンツの関連性を高めるため、マーケターに直接管理を提供します。

Dynamic Mediaクラシックでは、Adobe Target標準/プレミアムキャンペーン用のオファーとオファーセットを作成できます。 例えば、同じリッチメディアアセットの3つのバリエーションを含むオファーセットを作成できます。 次に、どのアセットがコンバージョン率の向上に役立つかをAdobe Target標準/プレミアムに判断させます。 基本テンプレートまたは個々の画像からオファーやオファーセットを作成できます。オファーセットがMboxおよびエクスペリエンスに関連付けられているAdobe Target標準/プレミアムにプッシュまたは保存されると、Adobe Target標準/プレミアムでキャンペーンを実行できます。 これらのキャンペーンは、クリックスルー数とコンバージョンに対してパフォーマンスが最も高いWebサイトのバリエーションを判断します。

動的なDynamic Mediaクラシックコンテンツをさらにカスタマイズするには、Adobe Target標準/プレミアムHTMLオファーを使用します。 詳しくは、[Adobe Target標準/プレミアム製品ドキュメント](https://experienceleague.adobe.com/docs/target.html)を参照してください。

>[!NOTE]
>
>Dynamic MediaクラシックでAdobe Target標準/プレミアムを使用するには、有効なAdobe Target標準/プレミアムアカウントが必要です。

このクイック開始では、Adobe Target標準/プレミアムHTMLオファーセットをすばやく習得できます。 手順 1 ～ 3 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

## 1.アプリの全般設定ページで、Adobe Target標準/プレミアムURLを入力します。

Dynamic Mediaクラシックは、Adobe Target標準/プレミアムと統合するために、Adobe Target標準/プレミアムURLが必要です。 Adobe Target標準/プレミアムURLの先頭から`.com`までをコピーし、を含む部分をDynamic Mediaクラシック&#x200B;**[!UICONTROL アプリケーションの全般設定]**&#x200B;ページの&#x200B;**[!UICONTROL サーバー]**&#x200B;グループ&#x200B;**[!UICONTROL Test&amp;ターゲットサーバー名]**&#x200B;テキストフィールドに入力します。 「[Dynamic MediaクラシックとAdobe Target標準/プレミアムとの統合](integrating-dmc-with-target.md#integrating-dmc-with-target)」を参照してください。

## 2. オファーセットの作成

オファーセットを作成するには、パラメータ化テンプレートまたは画像を使用します。HTMLオファーセットは、テストターゲットオファーセットページで作成します。 このページを開くには、テンプレートまたは画像を選択し、グローバルナビゲーションバーで&#x200B;**[!UICONTROL ビルド]**/**[!UICONTROL ターゲットオファーセット]**&#x200B;をクリックします。

テンプレートを使用してオファーを作成するには、**[!UICONTROL 追加 &amp;プレビュー]**&#x200B;をクリックします。 &amp;プレビュー追加ページで、パラメータ値を変更します。

画像を使用してオファーを作成するには、画像をテスト&amp;ターゲットオファーセットページにドラッグします。 「**[!UICONTROL プレビュー]**」をクリックし、オファーセット内の画像またはすべての画像の画像プリセットを選択します。

作成したら、オファーセットを保存します。

詳しくは、[オファーセットの作成](creating-offer-set.md#creating_an_offer_set)を参照してください。

## 3.オファーセットをAdobe Target標準/プレミアムにプッシュ

テストターゲットオファーセットページで、「**[!UICONTROL オファーをプッシュ]**」をクリックし、Test&amp;ターゲットのログインダイアログボックスにログイン資格情報を入力します。 「[オファーセットをAdobe Target標準/プレミアムにプッシュする](pushing-offer-sets-target.md#pushing_offer_sets_to_target)」を参照してください。
