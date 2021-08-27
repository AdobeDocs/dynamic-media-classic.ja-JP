---
title: 「クイックスタート：AdobeDynamic Media ClassicとAdobe Analyticsの統合»
description: Dynamic Media ClassicとAdobe Analyticsを統合して、すぐに使い始めるのに役立つAdobeの概要とクイックスタートです。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 27%

---

# クイックスタート：AdobeDynamic Media ClassicとAdobe Analyticsの統合 {#quick-start-integrating-dmc-analytics}

Adobe Analytics は、複数のマーケティングチャンネルからのすべてのオンライン業務の統合データを、マーケット担当者が一箇所で測定、分析、最適化できる、業界トップクラスの製品です。

Adobe AnalyticsをAdobeDynamic Media Classicと統合した後、Webサイト上のAdobeDynamic Media Classicビューアを使用して、Webサイト訪問者の行動に関するレポートを取得できます。 例えば、Webサイト訪問者がAdobeDynamic Mediaクラシックズームビューアでズームターゲットをクリックすると、Adobe Analyticsはこのアクションを記録します。 Adobe Analyticsレポートは、AdobeDynamic Media Classicビューアのユーザーアクティビティに関する累積情報を収集できます。

Adobe Analytics レポートを使用して、Web サイト上でのユーザーアクティビティの全体像を明確に把握できます。どの製品プレゼンテーションがコンバージョンにつながり、どの製品プレゼンテーションが顧客の関心を引かないかを判断できます。

[Adobe Analyticsでのビデオの測定](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)も参照してください。

>[!NOTE]
>
>AnalyticsをDynamic Media Classicと統合してAnalyticsレポートを生成するには、有効なAdobe AnalyticsAdobeが必要です。

ここでは、Adobe Analytics 計測キットをすばやく習得できるように、手順について簡潔に説明します。

## 1. Dynamic Media ClassicAdobeを使用してAdobe Analyticsにログインし、Adobe Analyticsレポート変数をダウンロードする

>[!NOTE]
>
>Adobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をAdobeDynamic Media Classicイベントに一致させる前に、Adobe AnalyticsのWebサービスアクセスグループのメンバーとして追加されていることを確認します。 このグループのメンバーは、インターフェイスで設定されている権限に関係なく、Experience CloudのWebサービスAPIを介して、指定したレポートスイートのすべてのレポートにアクセスできます。 グループにメンバーを追加するには、Adobe Analyticsで、**[!UICONTROL 管理ツール]** / **[!UICONTROL ユーザー管理]** / **[!UICONTROL グループの編集]**&#x200B;に移動します。

自分がWebサービスアクセスグループのメンバーであることを確認したら、Dynamic Media ClassicAdobeで、**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL Adobe Analytics]**&#x200B;に移動します。 Adobe Analytics設定ページで、「**[!UICONTROL Adobe Analyticsログイン]**」を選択します。

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

Adobe Analyticsログインダイアログボックスで、Experience Cloud組織ID（オプション）と完全な資格情報を入力し、「**[!UICONTROL ログイン]**」を選択します。 「レポートスイート」ドロップダウンメニューで、使用するレポートスイートの名前を選択します。

## 2. Adobe Analyticsレポート変数をAdobeDynamic Media ClassicビューアイベントとAdobeDynamic Media Classic変数に割り当てる

Adobe Analytics 設定ページで、Adobe Analytics レポートに表示する情報を指定します。情報が必要なAdobeのDynamic Media Classicビューアイベントごとに、Adobe Analytics変数（レポートスイートから）とAdobeのDynamic Media Classic変数を選択します。

* ビューアイベントは、レポートで測定するユーザアクティビティを表します。
* AdobeDynamic Media Classic変数は、レポートに配信するユーザーイベントに関するデータを記述します。

Adobe Analytics 設定には、ビューアイベントのアクティブ化、編集および削除のためのツールもあります。

Adobe Analytics設定ページで「**[!UICONTROL 保存]**」を選択すると、ユーザーアクティビティを測定するためのカスタマイズされたトラッキングコードが、Dynamic Media ClassicAdobeビューアに挿入されます。 この機能により、ユーザーアクティビティを Adobe Analytics レポートで追跡できるようになります。

[Adobe Analyticsレポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)を参照してください。

## 3.AdobeDynamic Media Classicビューアを公開する

AdobeのDynamic Media Classicビューアを公開して、ビューア(Adobe Analyticsレポートのユーザーアクティビティを追跡するコードを含む)をAdobeのDynamic Media Classicサーバーに読み込むようにします。 公開した後、この情報はビューアに取り込まれ、Adobe Analytics 分析に使用できます。

[公開設定情報](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

## 4. WebサイトにAdobeDynamic Media Classicビューアを配置する

Dynamic Media ClassicAdobeとAdobe AnalyticsトラッキングコードをWebサイトに配置する。

## 5. Adobe Analyticsレポートを表示してAdobe Analytics統合をテストする

Adobe Analytics レポートを表示するには、Adobe Analytics Web サイトにアクセスします。「レポート」ページでは、データを表示し、グラフとチャートを生成して様々なビューアでユーザーアクティビティを測定できます。

[Adobe Analyticsレポートを表示してAdobe Analytics統合をテストする](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)を参照してください。
