---
title: Adobe Analytics ビデオレポートの有効化
seo-title: Adobe Analytics ビデオレポートの有効化
description: 'null'
seo-description: Adobe Analyticsビデオレポートを有効にする方法を説明します。
uuid: 078594b2-7d53-4714-8128-ff3b5c3a5e36
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 18644a53-92da-40ab-b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Adobe Analytics ビデオレポートの有効化{#enabling-adobe-analytics-video-reports}

Adobe Analyticsハートビートベースのビデオレポートを使用する場合、Dynamic Media ClassicでAdobe Analyticsを設定する際に、4つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要はなくなりました。 ビデオハートビートは、標準搭載のダイナミックメディアクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。

* Adobe AnalyticsビデオレポートとDynamic Media Classicの統合では、ソリューション変数がサポートされますが、カスタム変数はサポートされません。

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* 標準搭載された 1 分単位のセグメントはサポートされますが、カスタムセグメントレポート（時間単位に基づいたユーザー定義のマイルストーン、％マイルストーン、オフセットマイルストーンなど）はサポートされません。

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>Adobe Analyticsのライセンスを受けたソリューションにビデオハートビートが含まれていない場合は、この章で説明する手順を使用し続けて、Adobe Analytics変数をDynamic Media Classicビューアのイベントと変数に割り当てる必要があります。

