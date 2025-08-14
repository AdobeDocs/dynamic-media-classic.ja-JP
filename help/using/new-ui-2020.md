---
title: Adobe Dynamic Media Classic デスクトップアプリ
description: Adobe Dynamic Media Classic ユーザーは、ユーザーインターフェイスを完全に更新できます。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: d61ea80a-a98e-43e6-9e2e-4389962134f1
topic: Administration
level: Intermediate
source-git-commit: 550d44027a314dd473a428048f4274bc16b033cd
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 0%

---

# Adobe Dynamic Media Classic デスクトップアプリ：提供開始 {#new-ui-2020}

システム要件を確認するには、[Adobe Dynamic Media Classic デスクトップアプリ ](/help/using/dynamic-media-classic-desktop-app.md) を参照し、新しいアプリをダウンロードしてインストールしてから、サインインします。

## _最終更新日：2020 年 6 月 30 日_

Adobe Dynamic Media Classic ユーザーは、ブラウザーのAdobe Flash テクノロジーに依存しなくなった新しいログインにアクセスできるようになりました。

## よくある質問 (FAQ)

+++**_2020 年 12 月 31 日（PT）にブラウザーがAdobe Flash のサポートを停止すると、Adobe Dynamic Media Classic（旧称 Scene7）に影響はありますか？_**
Adobe Flash Player は、Adobe Flash Platform で開発されたコンテンツを web ブラウザーが使用できるようにする web ブラウザープラグインでした。 Adobe Dynamic Media Classicの Web ユーザーインターフェイス（現在のラベルは [!DNL Scene7 Publishing System] または [!DNL SPS]）には、Adobe Flash Player が必要です。 2020 年 12 月 31 日（PT）にAdobe フラッシュが非推奨（廃止予定）になると、Adobe Dynamic Media Classicのお客様は web ユーザーインターフェイスにログインできなくなります。 この変更により、Adobeでは、ブラウザーエクスペリエンスに代わるデスクトップアプリをお客様に提供します。
+++

+++**_新しいデスクトップアプリケーションにアクセスするにはどうすればよいですか？_**
新しいデスクトップアプリケーションは、macOSの `.dmg` インストーラーとして、または Windows® の `.exe` インストーラーとして使用できます。

[Adobe Dynamic Media Classic デスクトップアプリ ](/help/using/dynamic-media-classic-desktop-app.md) を参照して、必要なシステム構成を確認し、新しいアプリをダウンロードしてインストールしてから、そのアプリにサインインします。
+++

<!-- NEWSLETTER IS DEAD The download links are also available by way of the [Adobe Dynamic Media Classic newsletter subscription page.](https://www.adobe.com/subscription/dynamic-media-newsletter.html) -->

+++**_新しいデスクトップアプリケーションはどのように機能しますか？_**
デスクトップアプリケーションのダウンロード、インストール、起動が完了すると、新しいログイン画面が表示されます。 既存のユーザー名とパスワードを入力し、お住まいの地域に応じて適切なサーバーを選択することで、Adobe Dynamic Media Classicにログインできます。 全体的なエクスペリエンスは、使い慣れた Web ブラウザーのバージョンと同じです。 デスクトップアプリケーションから、Adobe Dynamic Media Classicの実稼動環境とステージング環境にアクセスできます。 また、この機能の資格情報を持っている場合は、Media Portal にアクセスできます。

>[!IMPORTANT]
>
>特定のコンピューターに一度にインストール *および* アクティブ化できるデスクトップアプリケーションのインスタンスは 1 つだけです。 ただし、複数のコンピューターにまたがるインストールの数に制限はありません。

+++

+++**_Adobe Dynamic Media Classic API を使用して製品にアクセスしており、web ユーザーインターフェイスからログインしていない場合はどうなりますか？_**
Adobe Dynamic Media Classicの基になる API に変更はありません。
+++

+++**_この新しいデスクトップアプリケーションのエクスペリエンスでは、サードパーティ統合の移行や変更が必要ですか？_**
いいえ。 Adobe Dynamic Media Classicのお客様は、新しいデスクトップアプリケーションを使用するためにサードパーティの統合機能を移行または変更する必要はありません。
+++

+++**_この変更は自動化スクリプトに影響しますか？_**
いいえ。 自動化スクリプトへの影響はありません。 新しいデスクトップアプリは、既に慣れ親しんでいるブラウザーベースのエクスペリエンスと同様に動作し、動作します。
+++

+++**_新しいAdobe Dynamic Media Classic デスクトップアプリは Mac とパソコンで動作しますか？_**
可。新しいデスクトップアプリは、クロスプラットフォームのソリューションで、Mac と PC で動作します。 Linux® はサポートされて *ません*。
+++

+++**_私の会社には厳しいセキュリティ要件があります。 新しいAdobe Dynamic Media Classic デスクトップアプリケーションは、これらの要件をどのように処理しますか？_**
Adobeは、製品がお客様のセキュリティ要件を満たすよう取り組んでいます。 新しいAdobe Dynamic Media Classic デスクトップアプリは、引き続き、すべてのAdobe セキュリティ標準に準拠した高度に安全なエクスペリエンスをお客様に提供します。
+++

+++**_私の会社では、ソフトウェアやアプリをコンピューターにインストールすることを許可していません。 新しいデスクトップアプリケーションにアクセスするにはどうすればよいですか？_**
一部の企業では、ソフトウェアやアプリを承認なしにシステムにダウンロードしてインストールすることを許可していません。 その場合は、IT チームに早い段階から依頼して、新しいAdobe Dynamic Media Classic デスクトップアプリケーションへのアクセス権を取得します。 2020 年 12 月 31 日（PT）以降、ブラウザーバージョンは非推奨（廃止予定）になります。 新しいデスクトップアプリケーションをダウンロードする直前まで待つのを避けることが重要です。
+++

+++**_新しいデスクトップアプリケーションの複数のインスタンスを同時に開くことはできますか？_**
いいえ。 新しいAdobe Dynamic Media Classic デスクトップアプリケーションが構築されるAIR テクノロジーでは、ユーザーが特定の時間にアプリケーションの複数のインスタンスを開くことはできません。
+++

+++**_ローカルコンピューターからAdobe Dynamic Media Classicにアップロードできるファイルの数に制限はありますか？_**
Windows® で新しいAdobe Dynamic Media Classic デスクトップアプリケーションを使用する場合、**[!UICONTROL アップロード]** ダイアログボックスを使用して、一度に最大 150 個のファイルをアップロードできます。 この制限は、2020 年末までに既に対処されています。 macOS Platform には、アップロードに関する制限はありま *ん*。
+++

+++**_新しいAdobe Dynamic Media Classic デスクトップアプリには新しい SKU が必要ですか？ ライセンス費用はかかりますか？_**
両方の質問に対してはありません。 新しいAdobe Dynamic Media Classic デスクトップアプリを使用する際に、SKU やライセンスを変更する必要はありません。
+++

+++**_Adobe Dynamic Media Classic デスクトップアプリケーションへのアップグレードはどのように有効になりますか？_**
2020 年 6 月 30 日（PT）のAdobe Dynamic Media Classic デスクトップアプリケーションのリリース以降、Adobeで新しいバージョンがリリースされる場合、お客様は新しいバージョンをダウンロードしてインストールする必要があります（**[!UICONTROL Applications]** の既存のアプリを置き換える）。 新しいリリースの通知は、Adobe アカウントチームと、アップグレードをユーザーに通知するアプリ内アップグレード通知メカニズムを通じて受け取ります。
+++

+++**_Adobe Dynamic Media Classic デスクトップアプリの問題に関するヘルプを受けるにはどうすればよいですか？_**
アプリの使用中に問題が発生した場合は、Adobe サポートにお問い合わせください。
+++

+++**_リッチメディア戦略を最適化していることを確認したい。 Adobe Dynamic Media Classicの詳細を確認するにはどうすればよいですか？_** 
Adobe Dynamic Media Classicは、お客様のリッチメディア戦略を強化するために設計された、強力で機能豊富なソリューションです。 すべての機能を確実に活用するには、次のような実用的なリソースを参照してください。

* [Adobe Dynamic Media Classic ベストプラクティスチュートリアル ](https://experienceleague.adobe.com/en/docs/experience-manager-learn/dynamic-media-classic-tutorial/overview)
* [Adobeのブログ投稿 ](https://blog.adobe.com/)<!-- (https://blog.adobe.com/tag/dynamic-media/) -->
* [Adobe Dynamic Media ニュースレターアーカイブ ](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/dynamic-media-newsletter)
+++

<!-- HIDDEN AUGUST 2, 2021 BECAUSE THE NEWSLETTER WAS DISCONTINUED Plus, [subscribe to the Dynamic Media newsletter](https://www.adobe.com/subscription/dynamic-media-newsletter.html) to stay current on the latest news, information, training opportunities, powerful features available to you such as [Smart Imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html), and the complementary audit program. -->

+++**_Adobe Experience Manager Assetsを使用したAdobe Dynamic Media へのアップグレードについて詳しく説明します。 詳細情報はどこで入手できますか？_**
次世代のリッチメディアオーサリング、パブリッシング、および動的配信へのアップグレードの利点について詳しくは、[Adobe アップグレード用 Dynamic Media ポータル ](/help/using/upgrade.md) を参照してください。
+++

>[!MORELIKETHIS]
>
>* [Adobe Dynamic Media Classic デスクトップアプリケーションへのログインとログアウト ](/help/using/signing-out.md)
>* [Adobe Dynamic Media Classic デスクトップアプリケーションをダウンロードしてインストールする ](/help/using/dynamic-media-classic-desktop-app.md)

<!-- SAVE: OLD LINK TO BEST PRACTICES GUIDE IN PDF https://www.adobe.com/content/dam/www/us/en/marketing/experience-manager-assets/dynamic-media/adobe-dynamic-media-classic-best-practices-guide.pdf -->