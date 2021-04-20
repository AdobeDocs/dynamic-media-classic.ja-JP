---
title: 「クイック開始:Dynamic MediaクラシックとAdobe Analyticsの統合»
description: Dynamic MediaクラシックとAdobe Analyticsを統合して、すばやく作業を始めるのに役立つ紹介とクイック開始です。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 45%

---


# クイック開始:Dynamic MediaクラシックとAdobe Analyticsの統合{#quick-start-integrating-dmc-analytics}

Adobe Analytics は、複数のマーケティングチャンネルからのすべてのオンライン業務の統合データを、マーケット担当者が一箇所で測定、分析、最適化できる、業界トップクラスの製品です。

Adobe AnalyticsとDynamic Mediaクラシックを統合すると、Webサイト上でDynamic Mediaクラシックビューアを使用して、Webサイト訪問者の行動に関するレポートを取得できます。 例えば、Webサイトの訪問者がDynamic Mediaクラシックズームビューアのズームターゲットをクリックすると、Adobe Analyticsはこの操作を記録します。 Adobe Analyticsレポートでは、Dynamic Mediaクラシックビューアでのユーザアクティビティに関する累積情報を収集できます。

Adobe Analytics レポートを使用して、Web サイト上でのユーザーアクティビティの全体像を明確に把握できます。どの製品プレゼンテーションが売上につながり、どのプレゼンテーションが顧客の興味を引きつけないかがわかります。

「[Adobe Analytics でのビデオの測定](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)」も参照してください。

>[!NOTE]
>
>AnalyticsをDynamic Mediaクラシックと統合してAnalyticsレポートを生成するには、有効なAdobe Analyticsアカウントが必要です。

**クイック開始**

ここでは、Adobe Analytics 計測キットをすばやく習得できるように、手順について簡潔に説明します。

**1.Dynamic Mediaクラシックを使ってAdobe Analyticsにログインし、Adobe Analyticsレポート変数をダウンロード**

>[!NOTE]
>
>Adobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をDynamic Mediaクラシックイベントに一致させる前に、Adobe Analyticsの[Webサービスへのアクセス]グループのメンバーとして追加されていることを確認します。 このグループのメンバーは、インターフェイスで設定された権限に関係なく、Marketing Cloud の Web Services API 経由で指定したレポートスイートの全レポートにアクセスできます。グループにメンバーを追加するには、Adobe Analytics で、**管理ツール**／**ユーザー管理**／**グループの編集**&#x200B;をクリックします。

「Webサービスアクセス」グループのメンバーであることを確認したら、「Dynamic Mediaクラシック」で、**セットアップ**/**アプリケーション設定**/**Adobe Analytics**」をクリックします。 Adobe Analytics 設定ページで、「**Adobe Analytics ログイン**」をクリックします。

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

[Adobe Analyticsログイン]ダイアログボックスで、Marketing Cloud組織ID （オプション）と完全な資格情報を入力し、[**ログイン**]をクリックします。 「レポートスイート」ドロップダウンメニューで、使用するレポートスイートの名前を選択します。

**2．Adobe Analyticsレポート変数をDynamic MediaクラシックビューアイベントとDynamic Mediaクラシック変数に割り当てる**

Adobe Analytics 設定ページで、Adobe Analytics レポートに表示する情報を指定します。情報を取得する各Dynamic MediaクラシックViewerイベントに対して、Adobe Analytics変数（レポートスイートから）とDynamic Mediaクラシック変数を選択します。

* ビューアイベントは、レポートで測定するユーザアクティビティを表します。
* Dynamic Mediaクラシック変数は、レポートで配信するユーザーイベントに関するデータを記述します。

Adobe Analytics 設定には、ビューアイベントのアクティブ化、編集および削除のためのツールもあります。

Adobe Analytics設定画面で「保存」をクリックした後、ユーザアクティビティを測定するためのカスタマイズされた追跡コードがDynamic Mediaクラシックビューアに挿入されます。 この機能により、ユーザーアクティビティを Adobe Analytics レポートで追跡できるようになります。

詳しくは、[Adobe Analytics レポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)を参照してください。

**3.Dynamic Mediaクラシックビューアを公開する**

Dynamic Mediaクラシックビューアを公開して、ビューア(Adobe Analyticsレポートのユーザアクティビティを追跡するコード付き)がDynamic Mediaクラシックサーバに読み込まれるようにします。 公開した後、この情報はビューアに取り込まれ、Adobe Analytics 分析に使用できます。

詳しくは、[設定情報の公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

**4.Dynamic MediaクラシックビューアをWebサイトに配置する**

Adobe Analyticsトラッキングコードが付いたDynamic MediaクラシックビューアをWebサイトに配置します。

**5.Adobe Analytics レポートを表示して Adobe Analytics 統合をテストする**

Adobe Analytics レポートを表示するには、Adobe Analytics Web サイトにアクセスします。「レポート」ページでは、データを表示し、グラフとチャートを生成して様々なビューアでユーザーアクティビティを測定できます。

詳しくは、[Adobe Analytics レポートの表示による Adobe Analytics 統合のテスト](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)を参照してください。
