---
title: Adobe Analytics ビデオレポートの有効化
description: Adobe Dynamic Media ClassicでAdobe Analytics ビデオレポートを有効にする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
autotag-review: '2026-05-13T19:47:00.853Z'
TQID: 'https://experienceleague.adobe.com/bXlrGU0zMEyfa-E-x-29-biChC17GJTEViBP8GoouTU'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 270
ht-degree: 0%

---

# Adobe Analytics ビデオレポートの有効化{#enabling-adobe-analytics-video-reports}

Adobe Analytics ハートビートベースのビデオレポートを使用すると、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、4つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要がなくなりました。 ビデオ ハートビートは、Adobe Dynamic Media Classic HTML5のビデオおよびミックスメディアビューアで動作します。 ビデオプレーヤーは、Adobe Analytics ビデオレポート内で表示するためのトラッキングデータを生成します。

* ストリーミングメディアと「ハートビート測定」の概要については、[&#x200B; ストリーミングメディア用Adobe Analyticsについて](https://experienceleague.adobe.com/ja/docs/media-analytics/using/media-overview)を参照してください。

* Adobe Analytics ビデオレポートとAdobe Dynamic Media Classicの統合では、ソリューション変数はサポートされますが、カスタム変数はサポートされません。

  ソリューション変数とカスタム変数について詳しくは、[&#x200B; オーディオとビデオのパラメーター](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters)を参照してください。

* 1分インクリメントのすぐに使用できるセグメントがサポートされています。 ただし、時間増分に基づく顧客定義のマイルストーン、% マイルストーン、オフセットマイルストーンなどのカスタムセグメントレポートはサポートされていません。

  ストリーミングメディアの要件と設定について詳しくは、[Adobe Analyticsでのストリーミングメディアの測定](https://experienceleague.adobe.com/ja/docs/media-analytics/using/media-overview)を参照してください。

* カスタム変数とソリューション変数について詳しくは、[&#x200B; メディアレポートの有効化](https://experienceleague.adobe.com/ja/docs/media-analytics/using/media-reports/media-reports-enable#media-reports)を参照してください。

>[!NOTE]
>
>Adobe Analyticsのライセンス済みソリューションにビデオハートビートが含まれていない場合は、この章で説明する手順を引き続き使用して、Adobe Analytics変数をAdobe Dynamic Media Classic ビューアイベントおよび変数に割り当てます。
