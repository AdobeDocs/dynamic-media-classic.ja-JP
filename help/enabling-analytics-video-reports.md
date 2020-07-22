---
title: Adobe Analytics ビデオレポートの有効化
seo-title: Adobe Analytics ビデオレポートの有効化
description: 'null'
seo-description: アドビのAnalyticsビデオレポートを有効にする方法を説明します。
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 25%

---


# Adobe Analytics ビデオレポートの有効化{#enabling-adobe-analytics-video-reports}

AdobeAnalyticsハートビートベースのビデオレポートを使用すると、Adobe ClassicのDynamic MediaでAdobe Classicを設定する際に、4つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要がなくなりました。 ビデオハートビートは、標準搭載のDynamic MediaClassic HTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。

* アドビのAnalyticsビデオレポートとDynamic Mediaクラシックの統合では、ソリューション変数はサポートされますが、カスタム変数はサポートされません。

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* 標準搭載された 1 分単位のセグメントはサポートされますが、カスタムセグメントレポート（時間単位に基づいたユーザー定義のマイルストーン、％マイルストーン、オフセットマイルストーンなど）はサポートされません。

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>ライセンスを購入したAdobe Heartbeatソリューションにビデオハートビートが含まれていない場合は、この章で説明する手順に従って、AdobeAnalytics変数をDynamic MediaClassic Viewerのイベントと変数に割り当てる必要があります。

