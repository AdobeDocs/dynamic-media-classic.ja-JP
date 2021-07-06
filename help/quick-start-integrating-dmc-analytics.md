---
title: 「クイックスタート：Dynamic Media ClassicとAdobe Analyticsの統合»
description: Dynamic Media ClassicとAdobe Analyticsを統合し、すぐに使い始めるのに役立つ概要とクイックスタートです。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 41%

---

# クイックスタート：Dynamic Media ClassicとAdobe Analyticsの統合 {#quick-start-integrating-dmc-analytics}

Adobe Analytics は、複数のマーケティングチャンネルからのすべてのオンライン業務の統合データを、マーケット担当者が一箇所で測定、分析、最適化できる、業界トップクラスの製品です。

Adobe AnalyticsとDynamic Media Classicの統合後、Webサイト上でDynamic Media Classicビューアを使用してWebサイトを訪問した訪問者の行動に関するレポートを取得できます。 例えば、Dynamic MediaクラシックズームビューアでWebサイト訪問者がズームターゲットをクリックすると、Adobe Analyticsはこのアクションを記録します。 Adobe Analyticsレポートでは、Dynamic Media Classicビューアのユーザーアクティビティに関する累積情報を収集できます。

Adobe Analytics レポートを使用して、Web サイト上でのユーザーアクティビティの全体像を明確に把握できます。どの製品プレゼンテーションがコンバージョンにつながり、どの製品プレゼンテーションが顧客の関心を引かないかを判断できます。

「[Adobe Analytics でのビデオの測定](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)」も参照してください。

>[!NOTE]
>
>AnalyticsをDynamic Media Classicと統合してAnalyticsレポートを生成するには、有効なAdobe Analyticsアカウントが必要です。

ここでは、Adobe Analytics 計測キットをすばやく習得できるように、手順について簡潔に説明します。

## 1. Dynamic Media Classicを使用してAdobe Analyticsにログインし、Adobe Analyticsレポート変数をダウンロードする

>[!NOTE]
>
>Adobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をDynamic Media Classicイベントに対応させるには、Adobe Analyticsの「Webサービスアクセス」グループのメンバーとして追加されていることを確認します。 このグループのメンバーは、インターフェイスで設定された権限に関係なく、Marketing Cloud の Web Services API 経由で指定したレポートスイートの全レポートにアクセスできます。グループにメンバーを追加するには、Adobe Analytics で、**[!UICONTROL 管理ツール]**／**[!UICONTROL ユーザー管理]**／**[!UICONTROL グループの編集]**&#x200B;をクリックします。

自分がWebサービスアクセスグループのメンバーであることを確認したら、Dynamic Media Classicで、**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL Adobe Analytics]**&#x200B;をクリックします。 Adobe Analytics 設定ページで、「**[!UICONTROL Adobe Analytics ログイン]**」をクリックします。

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

Adobe Analyticsログインダイアログボックスで、Marketing Cloud組織ID（オプション）と完全な資格情報を入力し、「**[!UICONTROL ログイン]**」をクリックします。 「レポートスイート」ドロップダウンメニューで、使用するレポートスイートの名前を選択します。

## 2. Dynamic Media ClassicビューアイベントとDynamic Media Classic変数にAdobe Analyticsレポート変数を割り当てる

Adobe Analytics 設定ページで、Adobe Analytics レポートに表示する情報を指定します。情報が必要なDynamic Media Classicビューアイベントごとに、Adobe Analytics変数（レポートスイートから）とDynamic Media Classic変数を選択します。

* ビューアイベントは、レポートで測定するユーザアクティビティを表します。
* Dynamic Media Classic変数は、レポートに配信するユーザーイベントに関するデータを記述します。

Adobe Analytics 設定には、ビューアイベントのアクティブ化、編集および削除のためのツールもあります。

Adobe Analytics設定ページで「**[!UICONTROL 保存]**」をクリックすると、ユーザーアクティビティを測定するためのカスタマイズされたトラッキングコードがDynamic Media Classicビューアに挿入されます。 この機能により、ユーザーアクティビティを Adobe Analytics レポートで追跡できるようになります。

詳しくは、[Adobe Analytics レポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)を参照してください。

## 3. Dynamic Media Classicビューアを公開する

Dynamic Media Classicビューアを公開して、ビューア(Adobe Analyticsレポートのユーザーアクティビティを追跡するコードを含む)をDynamic Media Classicサーバーに読み込むようにします。 公開した後、この情報はビューアに取り込まれ、Adobe Analytics 分析に使用できます。

詳しくは、[設定情報の公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

## 4. WebサイトにDynamic Media Classicビューアを配置する

Dynamic Media ClassicビューアとAdobe AnalyticsトラッキングコードをWebサイトに配置する。

## 5. Adobe Analyticsレポートを表示してAdobe Analytics統合をテストする

Adobe Analytics レポートを表示するには、Adobe Analytics Web サイトにアクセスします。「レポート」ページでは、データを表示し、グラフとチャートを生成して様々なビューアでユーザーアクティビティを測定できます。

詳しくは、[Adobe Analytics レポートの表示による Adobe Analytics 統合のテスト](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)を参照してください。
