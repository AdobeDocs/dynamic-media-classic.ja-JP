---
title: Adobe Analytics ビデオレポートの有効化
description: Adobe Analyticsのビデオレポートを有効にする方法を説明します。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Mediaクラシック
role: Data Engineer,Administrator,Business Practitioner
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 17%

---

# Adobe Analytics ビデオレポートの有効化{#enabling-adobe-analytics-video-reports}

Adobe Analyticsハートビートベースのビデオレポートを使用する場合、Dynamic MediaクラシックでAdobe Analyticsを設定する際に、4つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要はなくなりました。 ビデオハートビートは、標準搭載のDynamic MediaクラシックHTML5ビデオビューアおよび混在メディアビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。

* ストリーミングメディアと「ハートビート指標」の概要については、[ストリーミングメディア用のAdobe Analyticsについて](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)を参照してください。

* Adobe AnalyticsビデオレポートとDynamic Mediaクラシックの統合では、ソリューション変数はサポートされますが、カスタム変数はサポートされません。

   ソリューション変数とカスタム変数について詳しくは、[オーディオとビデオのパラメーター](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata)を参照してください。

* 1分刻みの既成のセグメントがサポートされます。 カスタムセグメントレポート（時間単位に基づいたユーザー定義のマイルストーン、％マイルストーン、オフセットマイルストーンなど）はサポートされません。

   ストリーミングメディアの要件と設定について詳しくは、[Adobe Analyticsでのストリーミングメディアの測定](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)を参照してください。

* カスタム変数とソリューション変数について詳しくは、[メディアレポートの有効化](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)を参照してください。

>[!NOTE]
>
>ライセンスを取得したAdobe AnalyticsのソリューションにVideo Heartbeatが含まれていない場合は、この章で説明する手順に従って、Adobe Analytics変数をDynamic Mediaクラシックビューアのイベントと変数に割り当てる必要があります。
