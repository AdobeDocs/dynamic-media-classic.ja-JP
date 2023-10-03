---
title: Adobe Analyticsビデオレポートを有効にする
description: Adobe Dynamic Media ClassicでAdobe Analyticsビデオレポートを有効にする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 5%

---

# Adobe Analyticsビデオレポートを有効にする{#enabling-adobe-analytics-video-reports}

Adobe Analyticsハートビートベースのビデオレポートを使用して、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、4 つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要がなくなりました。 ビデオハートビートは、標準搭載のAdobe Dynamic Media ClassicHTML5 ビデオビューアおよび混在メディアビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。

* ストリーミングメディアと「ハートビート指標」の概要については、 [ストリーミングメディア用 Adobe Analyticsについて](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* Adobe AnalyticsビデオレポートとAdobe Dynamic Media Classicの統合では、ソリューション変数はサポートされますが、カスタム変数はサポートされません。

  詳しくは、 [オーディオおよびビデオパラメーター](https://experienceleague.adobe.com/docs/media-analytics/using/implementation/variables/audio-video-parameters.html) ソリューション変数とカスタム変数の詳細を参照してください。

* 1 分単位の増分で、すぐに使用できるセグメントがサポートされます。 ただし、時間増分、%マイルストーン、オフセットマイルストーンに基づく顧客定義のマイルストーンなどのカスタムセグメントレポートはサポートされていません。

  ストリーミングメディアの要件と設定について詳しくは、 [Adobe Analyticsでのストリーミングメディアの測定](https://experienceleague.adobe.com/docs/media-analytics/using/media-overview.html).

* カスタム変数とソリューション変数について詳しくは、 [メディアレポートの有効化](https://experienceleague.adobe.com/docs/media-analytics/using/media-reports/media-reports-enable.html?lang=en#media-reports).

>[!NOTE]
>
>Adobe Analyticsのライセンス版ソリューションにビデオハートビートが含まれていない場合は、この章で説明する手順を続行して、Adobe Analytics変数をAdobe Dynamic Media Classicビューアのイベントと変数に割り当てる必要があります。
