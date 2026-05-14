---
title: クイックスタート：Adobe Dynamic Media ClassicとAdobe Analyticsの統合
description: Adobe Dynamic Media ClassicとAdobe Analyticsの統合方法に関する概要とクイックスタート。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: a8fa2414-af01-4a58-bb33-dfd12c1056cc
topic: Integrations
level: Experienced
autotag-review: '2026-05-13T20:10:08.073Z'
TQID: 'https://experienceleague.adobe.com/DnpXpIqOz1HSLxZAoEOTHG65PSqTWLK7R--OzJj3FcY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 699
ht-degree: 23%

---

# クイックスタート：Adobe Dynamic Media ClassicとAdobe Analyticsの統合 {#quick-start-integrating-dmc-analytics}

Adobe Analytics は、複数のマーケティングチャンネルからのすべてのオンライン業務の統合データを、マーケット担当者が一箇所で測定、分析、最適化できる、業界トップクラスの製品です。

Adobe AnalyticsとAdobe Dynamic Media Classicを統合すると、web サイトでAdobe Dynamic Media Classic ビューアを使用しているweb サイト訪問者の行動に関するレポートを取得できます。 例えば、web サイト訪問者がAdobe Dynamic Media Classic ズームビューアでズームターゲットを選択すると、Adobe Analyticsはこのアクションを記録します。 Adobe Analytics レポートは、Adobe Dynamic Media Classic ビューアでのユーザーアクティビティに関する累積情報を収集できます。

Adobe Analytics レポートを使用して、Web サイト上でのユーザーアクティビティの全体像を明確に把握できます。 どの製品プレゼンテーションがコンバージョンにつながり、どの製品が顧客の興味を引かないかを判断できます。

Adobe Analyticsの[Measure ビデオ &#x200B;](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview)も参照してください。

>[!NOTE]
>
>AnalyticsとAdobe Dynamic Media Classicを統合し、Analytics レポートを生成するには、有効なAdobe Analytics アカウントが必要です。

このクイックスタートは、Adobe Analytics Instrumentation Kitを使用して、すばやく起動できるように設計されています。

## &#x200B;1. Adobe Dynamic Media Classic経由でAdobe Analyticsにログオンし、Adobe Analytics レポート変数をダウンロードします

>[!NOTE]
>
>Adobe AnalyticsのWeb サービスアクセスグループのメンバーとして追加されていることを確認します。 Adobe Analytics レポートを設定する前に、この検証を行います。 また、Adobe Analytics レポート変数をAdobe Dynamic Media Classic イベントに一致させる前に。 このグループのメンバーは、指定したレポートスイートのすべてのレポートにアクセスできます。 インターフェイスで設定された権限に関係なく、Experience CloudのWeb サービス APIを使用して行うことができます。 グループにメンバーを追加するには、Adobe Analyticsで、**[!UICONTROL 管理ツール]** > **[!UICONTROL ユーザー管理]** > **[!UICONTROL グループを編集]**&#x200B;に移動します。

お客様がWeb サービス アクセス グループのメンバーであることを確認したら、Adobe Dynamic Media Classicで、**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Adobe Analytics]**&#x200B;に移動します。 Adobe Analytics Configuration ページで、**[!UICONTROL Adobe Analytics Login]**&#x200B;を選択します。

[Adobe Analyticsにログオンする](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

Adobe Analytics ログインダイアログボックスで、Experience Cloud組織ID （オプション）と完全な資格情報を入力し、「**[!UICONTROL ログイン]**」を選択します。 「レポートスイート」ドロップダウンメニューで、使用するレポートスイートの名前を選択します。

## &#x200B;2. Adobe Analytics レポート変数のAdobe Dynamic Media Classic ビューアイベントおよびAdobe Dynamic Media Classic変数への割り当て

Adobe Analytics 設定ページで、Adobe Analytics レポートに表示する情報を指定します。 Adobe Dynamic Media Classic ビューアイベントごとに、（レポートスイートから）Adobe Analytics変数とAdobe Dynamic Media Classic変数を選択します。

* ビューアイベントは、レポートで測定するユーザアクティビティを表します。
* Adobe Dynamic Media Classic変数は、レポートで配信するユーザーイベントに関するデータを表します。

Adobe Analytics 設定には、ビューアイベントのアクティブ化、編集および削除のためのツールもあります。

Adobe Analytics Configuration ページで&#x200B;**[!UICONTROL Save]**&#x200B;を選択すると、Adobe Dynamic Media Classic ビューアにユーザーのアクティビティを測定するためのカスタマイズされたトラッキングコードが挿入されます。 この機能により、ユーザーアクティビティを Adobe Analytics レポートで追跡できるようになります。

[Adobe Analytics レポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)を参照してください。

## &#x200B;3. Adobe Dynamic Media Classic ビューアの公開

Adobe Dynamic Media Classic ビューアを公開して、ビューア（Adobe Analytics レポートでユーザーアクティビティをトラッキングするためのコードを含む）がAdobe Dynamic Media Classic サーバーに読み込まれるようにします。 公開後、この情報はビューアに含まれます。 Adobe Analyticsで分析する場合に使用します。

[構成情報の公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

## &#x200B;4. Adobe Dynamic Media Classic ビューアをweb サイトに配置する

Adobe Analytics トラッキングコードを使用して、Adobe Dynamic Media Classic ビューアをweb サイトに配置します。

## &#x200B;5. Adobe Analytics レポートを表示して Adobe Analytics 統合をテストする

Adobe Analytics レポートを表示するには、Adobe Analytics Web サイトにアクセスします。 「レポート」ページでは、データを表示し、グラフとチャートを生成して様々なビューアでユーザーアクティビティを測定できます。

Adobe Analytics レポートを表示して、[Adobe Analytics統合をテストする](testing-integration-viewing-analytics-report.md#testing_the_integration_by_viewing_an_adobe_analytics_report)を参照してください。
