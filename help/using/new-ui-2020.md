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
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 0%

---

# Adobe Dynamic Media Classic デスクトップアプリ：提供開始 {#new-ui-2020}

を参照してください。 [Adobe Dynamic Media Classic デスクトップアプリ](/help/using/dynamic-media-classic-desktop-app.md) システム要件を確認するには、新しいアプリをダウンロードしてインストールし、そのアプリにサインインします。

## _最終更新日：2020 年 6 月 30 日（PT）_

Adobe Dynamic Media Classic ユーザーは、ブラウザーのAdobeFlashテクノロジーに依存しなくなった新しいログインにアクセスできるようになりました。

## よくある質問 (FAQ)

+++**_2020 年 12 月 31 日（PT）にブラウザーがAdobeFlashのサポートを停止すると、Adobe Dynamic Media Classic（旧称Scene7）に何らかの影響がありますか？_**
AdobeFlash Playerは、web ブラウザーがAdobe Flash Platformで開発されたコンテンツを使用できるようにする web ブラウザープラグインでした。 Adobe Dynamic Media Classicの Web ユーザーインターフェイス（現在のラベルは [!DNL Scene7 Publishing System] または [!DNL SPS] （商品で）はAdobeFlash Playerが必要でした。 2020 年 12 月 31 日（PT）にAdobeFlashが非推奨（廃止予定）になると、Adobe Dynamic Media Classicのお客様は web ユーザーインターフェイスにログインできなくなります。 この変更により、Adobeでは、ブラウザーエクスペリエンスに代わるデスクトップアプリをお客様に提供しています。
+++

+++**_新しいデスクトップアプリケーションにアクセスするにはどうすればよいですか？_**
新しいデスクトップアプリケーションは、 `.dmg` macOSまたは as a のインストーラー `.exe` windows® 用インストーラー。

を参照してください。 [Adobe Dynamic Media Classic デスクトップアプリ](/help/using/dynamic-media-classic-desktop-app.md) システム要件を確認するには、新しいアプリをダウンロードしてインストールし、そのアプリにサインインします。
+++

<!-- NEWSLETTER IS DEAD The download links are also available by way of the [Adobe Dynamic Media Classic newsletter subscription page.](https://www.adobe.com/subscription/dynamic-media-newsletter.html) -->

+++**_新しいデスクトップアプリケーションの動作_**
デスクトップアプリケーションのダウンロード、インストール、起動が完了すると、新しいログイン画面が表示されます。 既存のユーザー名とパスワードを入力し、お住まいの地域に応じて適切なサーバーを選択することで、Adobe Dynamic Media Classicにログインできます。 全体的なエクスペリエンスは、使い慣れた Web ブラウザーのバージョンと同じです。 デスクトップアプリケーションから、Adobe Dynamic Media Classicの実稼動環境とステージング環境にアクセスできます。 また、この機能の資格情報を持っている場合は、Media Portal にアクセスできます。

>[!IMPORTANT]
>
>インストールできるデスクトップアプリケーションのインスタンスは 1 つだけです *および* 特定のコンピューター上で一度にアクティブです。 ただし、複数のコンピューターにまたがるインストールの数に制限はありません。

+++

+++**_Adobe Dynamic Media Classic API を使用して製品にアクセスしていて、web ユーザーインターフェイスからログインしていない場合は、_**
Adobe Dynamic Media Classicの基になる API に変更はありません。
+++

+++**_この新しいデスクトップアプリケーションのエクスペリエンスでは、サードパーティ統合の移行または変更が必要ですか？_**
いいえ。 Adobe Dynamic Media Classicのお客様は、新しいデスクトップアプリケーションを使用するためにサードパーティの統合機能を移行または変更する必要はありません。
+++

+++**_この変更は自動化スクリプトに影響を与えますか？_**
いいえ。 自動化スクリプトへの影響はありません。 新しいデスクトップアプリは、既に慣れ親しんでいるブラウザーベースのエクスペリエンスと同様に動作し、動作します。
+++

+++**_新しいAdobe Dynamic Media Classic デスクトップアプリケーションは Mac とパソコンで動作しますか？_**
はい。 新しいデスクトップアプリは、クロスプラットフォームのソリューションで、Mac と PC で動作します。 Linux® は *ではない* サポート。
+++

+++**_私の会社には厳しいセキュリティ要件があります。 新しいAdobe Dynamic Media Classic デスクトップアプリケーションは、これらの要件をどのように処理しますか？_**
Adobeは、製品がお客様のセキュリティ要件を満たすよう取り組んでいます。 新しいAdobe Dynamic Media Classic デスクトップアプリは、引き続き、すべてのAdobeセキュリティ標準に準拠した高度に安全なエクスペリエンスをお客様に提供します。
+++

+++**_私の会社は、私が私のコンピュータにソフトウェアとアプリをインストールすることを許可していません。 新しいデスクトップアプリケーションへのアクセス権を取得するにはどうすればよいですか？_**
一部の企業では、ソフトウェアやアプリを承認なしにシステムにダウンロードしてインストールすることを許可していません。 その場合は、IT チームに早い段階から依頼して、新しいAdobe Dynamic Media Classic デスクトップアプリケーションへのアクセス権を取得します。 2020 年 12 月 31 日（PT）以降、ブラウザーバージョンは非推奨（廃止予定）になります。 新しいデスクトップアプリケーションをダウンロードする直前まで待つのを避けることが重要です。
+++

+++**_新しいデスクトップアプリケーションの複数のインスタンスを同時に開くことはできますか？_**
いいえ。 新しいAdobe Dynamic Media Classic デスクトップアプリケーションが構築されるAIR テクノロジーでは、ユーザーが特定の時間にアプリケーションの複数のインスタンスを開くことはできません。
+++

+++**_ローカルコンピューターを介してAdobe Dynamic Media Classicにアップロードできるファイルの数に制限はありますか？_**
Windows® で新しいAdobe Dynamic Media Classic デスクトップアプリケーションを使用する場合、を使用して、一度に最大 150 個のファイルをアップロードできます。 **[!UICONTROL Upload]** ダイアログが表示されます。 この制限は、2020 年末までに既に対処されています。 次のものがあります *なし* macOS Platform への制限のアップロード。
+++

+++**_新しいAdobe Dynamic Media Classic デスクトップアプリには新しい SKU が必要ですか？ ライセンス費用はかかりますか？_**
両方の質問に対してはありません。 新しいAdobe Dynamic Media Classic デスクトップアプリを使用する際に、SKU やライセンスを変更する必要はありません。
+++

+++**_Adobe Dynamic Media Classic デスクトップアプリケーションのアップグレードはどのように有効になりますか？_**
2020 年 6 月 30 日（PT）のAdobe Dynamic Media Classic デスクトップアプリケーションのリリース以降、Adobeが新しいバージョンをリリースする場合、お客様は新しいバージョンをダウンロードしてインストールする必要があります（の既存のアプリを置き換える） **[!UICONTROL アプリケーション]**）に設定します。 新しいリリースの通知は、Adobeアカウントチームと、アップグレードをユーザーに通知するアプリ内アップグレード通知メカニズムを通じて受け取ります。
+++

+++**_Adobe Dynamic Media Classic デスクトップアプリケーションに関する問題が発生した場合、どのようにサポートを受けることができますか？_**
アプリの使用中に問題が発生した場合は、Adobeサポートにお問い合わせください。
+++

+++**_リッチメディア戦略を最適化しているかどうか確認したい。 Adobe Dynamic Media Classicの詳細を確認するにはどうすればよいですか？_**
Adobe Dynamic Media Classicは、お客様のリッチメディア戦略を強化するために設計された、強力で機能豊富なソリューションです。 すべての機能を確実に活用するには、次のような実用的なリソースを参照してください。

* [Adobe Dynamic Media Classic ベストプラクティスチュートリアル](https://experienceleague.adobe.com/en/docs/experience-manager-learn/dynamic-media-classic-tutorial/overview)
* [Adobeのブログ投稿](https://blog.adobe.com/)<!-- (https://blog.adobe.com/tag/dynamic-media/) -->
* [Adobe Dynamic Media ニュースレターアーカイブ](https://experienceleague.adobe.com/en/docs/dynamic-media-classic/using/dynamic-media-newsletter)
+++

<!-- HIDDEN AUGUST 2, 2021 BECAUSE THE NEWSLETTER WAS DISCONTINUED Plus, [subscribe to the Dynamic Media newsletter](https://www.adobe.com/subscription/dynamic-media-newsletter.html) to stay current on the latest news, information, training opportunities, powerful features available to you such as [Smart Imaging](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html), and the complementary audit program. -->

+++**_Adobe Experience Manager Assetsを使用したAdobeDynamic Mediaへのアップグレードに関する詳細を確認します。 詳細情報はどこで入手できますか？_**
次世代のリッチメディアオーサリング、パブリッシング、および動的配信へのアップグレードのメリットについて詳しくは、こちらを参照してください [アップグレード用にDynamic Media ポータルをAdobeする](/help/using/upgrade.md).
+++

>[!MORELIKETHIS]
>
>* [Adobe Dynamic Media Classic デスクトップアプリケーションへのログインとログアウト](/help/using/signing-out.md)
>* [Adobe Dynamic Media Classic デスクトップアプリケーションをダウンロードしてインストールする](/help/using/dynamic-media-classic-desktop-app.md)

<!-- SAVE: OLD LINK TO BEST PRACTICES GUIDE IN PDF https://www.adobe.com/content/dam/www/us/en/marketing/experience-manager-assets/dynamic-media/adobe-dynamic-media-classic-best-practices-guide.pdf -->