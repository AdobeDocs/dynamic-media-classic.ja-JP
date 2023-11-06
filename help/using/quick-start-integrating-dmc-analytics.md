---
title: クイックスタート：Adobe Dynamic Media ClassicとAdobe Analyticsの統合
description: Adobe Dynamic Media ClassicとAdobe Analyticsを統合してすばやく使い始めるのに役立つ方法の概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: faa1784e1d19b1167cad5749dc04227e3ff388e5
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 27%

---

# クイックスタート： Adobe Dynamic Media ClassicとAdobe Analyticsの統合 {#quick-start-integrating-dmc-analytics}

Adobe Analytics は、複数のマーケティングチャンネルからのすべてのオンライン業務の統合データを、マーケット担当者が一箇所で測定、分析、最適化できる、業界トップクラスの製品です。

Adobe AnalyticsをAdobe Dynamic Media Classicと統合した後、Web サイトでAdobe Dynamic Media Classicビューアを使用して、Web サイトの訪問者の行動に関するレポートを取得できます。 例えば、Web サイトの訪問者がAdobe Dynamic Media Classicズームビューアでズームターゲットを選択すると、Adobe Analyticsはこの操作を記録します。 Adobe Analyticsレポートは、Adobe Dynamic Media Classicビューアのユーザーアクティビティに関する累積情報を収集できます。

Adobe Analytics レポートを使用して、Web サイト上でのユーザーアクティビティの全体像を明確に把握できます。どの製品プレゼンテーションがコンバージョンにつながり、どのプレゼンテーションが顧客の関心を引き付けないかを判断できます。

関連トピック [Adobe Analyticsでビデオを測定](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

>[!NOTE]
>
>Analytics とAdobe Dynamic Media Classicを統合し、Analytics レポートを生成するには、有効なAdobe Analyticsアカウントが必要です。

ここでは、Adobe Analytics 計測キットをすばやく習得できるように、手順について簡潔に説明します。

## 1. Adobe Dynamic Media Classicを使用してAdobe Analyticsにログインし、Adobe Analyticsレポート変数をダウンロードする

>[!NOTE]
>
>Adobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をAdobe Dynamic Media Classicイベントに一致させるには、まず、Adobe Analyticsで Web サービスアクセスグループのメンバーとして追加されていることを確認します。 このグループのメンバーは、インターフェイスで設定されている権限に関係なく、Experience Cloudの Web Services API を通じて、指定したレポートスイート内のすべてのレポートにアクセスできます。 メンバーをグループに追加するには、Adobe Analyticsで、 **[!UICONTROL 管理ツール]** > **[!UICONTROL ユーザー管理]** > **[!UICONTROL グループの編集]**.

自分が Web サービスアクセスグループのメンバーであることを確認したら、Adobe Dynamic Media Classicで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL Adobe Analytics]**. Adobe Analytics設定ページで、「 」を選択します。 **[!UICONTROL Adobe Analytics Login]**.

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

Adobe Analyticsログインダイアログボックスで、Experience Cloud組織 ID（オプション）と完全な資格情報を入力し、「 」を選択します。 **[!UICONTROL ログイン]**. 「レポートスイート」ドロップダウンメニューで、使用するレポートスイートの名前を選択します。

## 2. Adobe Analyticsレポート変数をAdobe Dynamic Media ClassicビューアイベントとAdobe Dynamic Media Classic変数に割り当てる

Adobe Analytics 設定ページで、Adobe Analytics レポートに表示する情報を指定します。情報が必要なAdobe Dynamic Media Classicビューアイベントごとに、Adobe Analytics変数（レポートスイートから）とAdobe Dynamic Media Classic変数を選択します。

* ビューアイベントは、レポートで測定するユーザアクティビティを表します。
* Adobe Dynamic Media Classic変数は、レポートに配信するユーザーイベントに関するデータを記述します。

Adobe Analytics 設定には、ビューアイベントのアクティブ化、編集および削除のためのツールもあります。

次を選択した後： **[!UICONTROL 保存]** Adobe Analyticsの設定ページで、ユーザーアクティビティを測定するためのカスタマイズされたトラッキングコードがAdobe Dynamic Media Classicビューアに挿入されます。 この機能により、ユーザーアクティビティを Adobe Analytics レポートで追跡できるようになります。

詳しくは、 [Adobe Analyticsレポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports).

## 3. Adobe Dynamic Media Classicビューアを公開する

Adobe Dynamic Media Classicビューアを公開して、ビューア (Adobe Analyticsレポートのユーザーアクティビティを追跡するコード ) がAdobe Dynamic Media Classicサーバーに読み込まれるようにします。 公開した後、この情報はビューアに取り込まれ、Adobe Analytics 分析に使用できます。

詳しくは、 [設定情報を公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## 4. Web サイトにAdobe Dynamic Media Classicビューアを配置する

Adobe Dynamic Media ClassicビューアにAdobe Analyticsトラッキングコードを配置します。

## 5. Adobe Analyticsレポートを表示してAdobe Analytics統合をテストする

Adobe Analytics レポートを表示するには、Adobe Analytics Web サイトにアクセスします。「レポート」ページでは、データを表示し、グラフとチャートを生成して様々なビューアでユーザーアクティビティを測定できます。

詳しくは、 [Adobe Analyticsレポートを表示してAdobe Analytics統合をテストする](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report).
