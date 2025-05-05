---
title: 「クイックスタート：Adobe Dynamic Media ClassicとAdobe Analyticsの統合」
description: Adobe Dynamic Media ClassicとAdobe Analyticsの統合方法に関する概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 21%

---

# クイックスタート：Adobe Dynamic Media ClassicとAdobe Analyticsの統合 {#quick-start-integrating-dmc-analytics}

Adobe Analytics は、複数のマーケティングチャンネルからのすべてのオンライン業務の統合データを、マーケット担当者が一箇所で測定、分析、最適化できる、業界トップクラスの製品です。

Adobe AnalyticsをAdobe Dynamic Media Classicと統合すると、web サイトでAdobe Dynamic Media Classic ビューアを使用して、web サイトの訪問者の行動に関するレポートを取得できます。 例えば、web サイトの訪問者がAdobe Dynamic Media Classic ズームビューアでズームターゲットを選択すると、Adobe Analyticsにこのアクションが記録されます。 Adobe Analytics レポートは、Adobe Dynamic Media Classic ビューアでのユーザーアクティビティに関する累積情報を収集できます。

Adobe Analytics レポートを使用して、Web サイト上でのユーザーアクティビティの全体像を明確に把握できます。どの製品プレゼンテーションがコンバージョンにつながり、どの製品プレゼンテーションが顧客の関心を引かないかを判断できます。

[Adobe Analyticsでのビデオの測定 ](https://experienceleague.adobe.com/ja/docs/media-analytics/using/media-overview) も参照してください。

>[!NOTE]
>
>Analytics をAdobe Analyticsと統合し、Analytics レポートを生成するには、有効なAdobe Dynamic Media Classic アカウントが必要です。

このクイックスタートは、Adobe Analytics インストルメンテーションキットをすぐに使い始めることを目的としています。

## 1. Adobe Dynamic Media Classic経由でAdobe Analyticsにログオンし、Adobe Analytics レポート変数をダウンロードします

>[!NOTE]
>
>Adobe Analyticsの web サービスアクセスグループのメンバーとして追加されていることを確認します。 Adobe Analytics レポートを設定する前に、この検証を行います。 また、Adobe Analytics レポート変数をAdobe Dynamic Media Classic イベントと照合する前に、 このグループのメンバーは、指定されたレポートスイート内のすべてのレポートにアクセスできます。 インターフェイスで設定された権限に関係なく、Experience Cloudの Web サービス API を使用して行うことができます。 グループにメンバーを追加するには、Adobe Analyticsで **[!UICONTROL 管理ツール]**/**[!UICONTROL User Management]**/**[!UICONTROL グループを編集]** に移動します。

Web サービスアクセスグループのメンバーであることを確認したら、Adobe Dynamic Media Classicで **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**4&rbrace;Adobe Analytics&rbrace; に移動します。** Adobe Analytics設定ページで、「**[!UICONTROL Adobe Analytics Login]**」を選択します。

[Adobe Analyticsへのログオン ](log-analytics.md#log_in_to_adobe_analytics) を参照してください。

Adobe Analyticsのログインダイアログボックスで、Experience Cloud組織 ID （オプション）、完全な資格情報を入力し、「**[!UICONTROL ログイン]**」を選択します。 「レポートスイート」ドロップダウンメニューで、使用するレポートスイートの名前を選択します。

## 2. Adobe Analytics レポート変数をAdobe Dynamic Media Classic ビューアイベントとAdobe Dynamic Media Classic変数に割り当てる

Adobe Analytics 設定ページで、Adobe Analytics レポートに表示する情報を指定します。情報を取得するAdobe Dynamic Media Classic ビューアイベントごとに、Adobe Analytics変数（レポートスイートから）とAdobe Dynamic Media Classic変数を選択します。

* ビューアイベントは、レポートで測定するユーザアクティビティを表します。
* Adobe Dynamic Media Classic変数は、レポートで提供するユーザーイベントに関するデータを記述します。

Adobe Analytics 設定には、ビューアイベントのアクティブ化、編集および削除のためのツールもあります。

Adobe Analytics設定ページで「**[!UICONTROL 保存]**」を選択すると、ユーザーアクティビティを測定するためのカスタマイズされたトラッキングコードがAdobe Dynamic Media Classic ビューアに挿入されます。 この機能により、ユーザーアクティビティを Adobe Analytics レポートで追跡できるようになります。

[Adobe Analytics レポートの設定 ](configuring-analytics-reports.md#configuring_adobe_analytics_reports) を参照してください。

## 3. Adobe Dynamic Media Classic ビューアをPublishする

ビューア（Adobe Analytics レポートでのユーザーアクティビティをトラッキングするコードを含む）がAdobe Dynamic Media Classic サーバーに読み込まれるように、Adobe Dynamic Media Classic ビューアをPublishします。 公開後、この情報はビューアに含まれます。 Adobe Analyticsの分析に使用します。

[Publishの設定に関する情報 ](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information) を参照してください。

## 4. Web サイトへのAdobe Dynamic Media Classic ビューアの配置

Adobe Analytics トラッキングコードを使用したAdobe Dynamic Media Classic ビューアを Web サイトに配置します。

## 5. Adobe Analytics レポートを表示してAdobe Analytics統合をテストする

Adobe Analytics レポートを表示するには、Adobe Analytics Web サイトにアクセスします。「レポート」ページでは、データを表示し、グラフとチャートを生成して様々なビューアでユーザーアクティビティを測定できます。

[Adobe Analytics レポートを表示してAdobe Analytics統合をテストする ](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report) を参照してください。
