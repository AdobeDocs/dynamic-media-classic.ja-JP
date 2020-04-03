---
title: 「クイック開始:Dynamic Media ClassicとAdobe Analyticsの統合」
seo-title: 「クイック開始:Dynamic Media ClassicとAdobe Analyticsの統合」
description: 'null'
seo-description: Dynamic Media ClassicとAdobe Analyticを統合し、すばやく使い始めるための概要とクイック開始です。
uuid: 3f9e2c91-15d4-4b53-8220-9b1ca57c0b1d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: abec9a85-013c-4030-b129-bf27a89cb464
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# クイック開始:Dynamic Media ClassicとAdobe Analyticsの統合 {#quick-start-integrating-scene-and-adobe-analytics}

Adobe Analytics は、複数のマーケティングチャンネルからのすべてのオンライン業務の統合データを、マーケット担当者が一箇所で測定、分析、最適化できる、業界トップクラスの製品です。

Adobe AnalyticsをScene7 Publishing Systemと統合すると、Webサイト上でDynamic Media Classicビューアを使用してWebサイト訪問者の動作に関するレポートを取得できます。 例えば、Webサイトの訪問者がダイナミックメディアクラシックズームビューアのズームターゲットをクリックすると、Adobe Analyticsはこの操作を記録します。 Adobe Analyticsレポートは、Dynamic Media Classic Viewerのユーザーアクティビティに関する累積情報を収集できます。

Adobe Analytics レポートを使用して、Web サイト上でのユーザーアクティビティの全体像を明確に把握できます。どの製品プレゼンテーションが売上につながり、どのプレゼンテーションが顧客の興味を引きつけないかがわかります。

「[Adobe Analytics でのビデオの測定](https://marketing.adobe.com/resources/help/en_US/sc/appmeasurement/hbvideo/)」も参照してください。

>[!NOTE]
>
>Analytics を Scene7 Publishing System と統合して Analytics レポートを生成するには、有効な Adobe Analytics アカウントが必要です。

**クイック開始**

ここでは、Adobe Analytics 計測キットをすばやく習得できるように、手順について簡潔に説明します。

**1.Log in to Adobe Analytics by way of Dynamic Media Classic and download Adobe Analytics report variables**

>[!NOTE]
>
>Adobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をDynamic Media Classicイベントに一致させる前に、Adobe Analyticsの「Webサービスへのアクセス」グループのメンバーとして追加されていることを確認します。 このグループのメンバーは、インターフェイスで設定された権限に関係なく、Marketing Cloud の Web Services API 経由で指定したレポートスイートの全レポートにアクセスできます。グループにメンバーを追加するには、Adobe Analytics で、**管理ツール**／**ユーザー管理**／**グループの編集**&#x200B;をクリックします。

After you have verified that you are a member of the Web Service Access group, in Dynamic Media Classic, click **Setup** > **Application Setup** > **Adobe Analytics**. Adobe Analytics 設定ページで、「**Adobe Analytics ログイン**」をクリックします。

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

Adobe Analyticsのログインダイアログボックスで、Marketing Cloud組織ID（オプション）と完全な資格情報を入力し、「ログイン」をクリック **します**。 「レポートスイート」ドロップダウンメニューで、使用するレポートスイートの名前を選択します。

**2．Adobe Analyticsレポート変数をダイナミックMedia ClassicビューアイベントとダイナミックMedia Classic変数に割り当てる**

Adobe Analytics 設定ページで、Adobe Analytics レポートに表示する情報を指定します。必要な各Dynamic Media Classicビューアイベントに対して、Adobe Analytics変数（レポートスイートから）とDynamic Media Classic変数を選択します。

* ビューアイベントは、レポートで測定するユーザアクティビティを表します。
* ダイナミックMedia Classic変数は、レポートで配信するユーザーイベントに関するデータを記述します。

Adobe Analytics 設定には、ビューアイベントのアクティブ化、編集および削除のためのツールもあります。

Adobe Analytics設定画面で「保存」をクリックすると、ユーザーアクティビティを測定するためのカスタマイズされた追跡コードがDynamic Media Classicビューアに挿入されます。 この機能により、ユーザーアクティビティを Adobe Analytics レポートで追跡できるようになります。

詳しくは、[Adobe Analytics レポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)を参照してください。

**3. ダイナミックメディアクラシックビューアの公開**

Dynamic Media Classicビューアを公開し、ビューア(Adobe Analyticsレポートのユーザーアクティビティを追跡するコード付き)がDynamic Media Classicサーバーに読み込まれるようにします。 公開した後、この情報はビューアに取り込まれ、Adobe Analytics 分析に使用できます。

詳しくは、[設定情報の公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

**4. Dynamic Media ClassicビューアをWebサイトに配置する**

Adobe Analytics追跡コードを含むDynamic Media ClassicビューアをWebサイトに配置します。

**5. Adobe Analytics レポートを表示して Adobe Analytics 統合をテストする**

Adobe Analytics レポートを表示するには、Adobe Analytics Web サイトにアクセスします。「レポート」ページでは、データを表示し、グラフとチャートを生成して様々なビューアでユーザーアクティビティを測定できます。

詳しくは、[Adobe Analytics レポートの表示による Adobe Analytics 統合のテスト](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)を参照してください。
