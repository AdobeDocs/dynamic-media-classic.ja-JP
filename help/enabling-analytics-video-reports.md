---
title: Adobe Analytics ビデオレポートの有効化
seo-title: Adobe Analytics ビデオレポートの有効化
description: 'null'
seo-description: Adobe Analyticsのビデオレポートを有効にする方法を説明します。
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

Adobe Analyticsハートビートベースのビデオレポートを使用すると、Dynamic MediaクラシックでAdobe Analyticsを設定する際に、4つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要がなくなりました。 ビデオハートビートは、標準搭載のDynamic MediaクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。

* Adobe AnalyticsビデオレポートとDynamic Mediaクラシックの統合では、ソリューション変数はサポートされますが、カスタム変数はサポートされません。

   ソリューション変数とカスタム変数について詳しくは、[Analyticsビデオレポートの設定](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html)を参照してください。

* 標準搭載された 1 分単位のセグメントはサポートされますが、カスタムセグメントレポート（時間単位に基づいたユーザー定義のマイルストーン、％マイルストーン、オフセットマイルストーンなど）はサポートされません。

ビデオハートビートの要件とセットアップについて詳しくは、[ビデオハートビートを使用したAdobe Analyticsでのビデオの測定](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/)を参照してください。

>[!NOTE]
>
>ライセンスを取得したAdobe AnalyticsのソリューションにVideo Heartbeatが含まれていない場合は、この章で説明する手順に従って、Adobe Analytics変数をDynamic Mediaクラシックビューアのイベントと変数に割り当てる必要があります。

