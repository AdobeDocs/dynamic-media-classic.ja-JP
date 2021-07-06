---
title: Adobe Analytics ビデオレポートの有効化
description: Adobe Analyticsビデオレポートを有効にする方法を説明します。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 17%

---

# Adobe Analytics ビデオレポートの有効化{#enabling-adobe-analytics-video-reports}

Adobe Analyticsハートビートベースのビデオレポートを使用する場合、Dynamic Media ClassicでAdobe Analyticsを設定する際に、4つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要がなくなりました。 ビデオハートビートは、標準搭載のDynamic Media Classic HTML5ビデオビューアおよび混在メディアビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。

* ストリーミングメディアと「ハートビート測定」の概要については、[Adobe Analytics for Streaming Mediaについて](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html#about-adobe-analytics-for-streaming-media)を参照してください。

* Adobe AnalyticsビデオレポートとDynamic Media Classicの統合では、ソリューション変数はサポートされますが、カスタム変数はサポートされません。

   ソリューション変数とカスタム変数について詳しくは、[オーディオおよびビデオパラメーター](https://experienceleague.adobe.com/docs/media-analytics/using/metrics-and-metadata/audio-video-parameters.html#metrics-and-metadata)を参照してください。

* 1分単位の増分で、そのまま使用できるセグメントがサポートされます。 カスタムセグメントレポート（時間単位に基づいたユーザー定義のマイルストーン、％マイルストーン、オフセットマイルストーンなど）はサポートされません。

   ストリーミングメディアの要件と設定について詳しくは、[Adobe Analyticsでのストリーミングメディアの測定](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html)を参照してください。

* カスタム変数とソリューション変数について詳しくは、[メディアレポートの有効化](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports)を参照してください。

>[!NOTE]
>
>Adobe Analyticsのライセンスソリューションにビデオハートビートが含まれていない場合は、この章で説明する手順を続行して、Adobe Analytics変数をDynamic Media Classicビューアのイベントと変数に割り当てる必要があります。
