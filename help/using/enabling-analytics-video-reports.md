---
title: Adobe Analytics ビデオレポートを有効にする
description: Adobe Dynamic Media ClassicでAdobe Analytics ビデオレポートを有効にする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9d017742-1ed2-411d-a8a6-438102bf1557
topic: Development, Integrations
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Adobe Analytics ビデオレポートを有効にする{#enabling-adobe-analytics-video-reports}

Adobe Analytics ハートビートベースのビデオレポートを使用して、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、4 つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要がなくなりました。 ビデオハートビートは、標準のAdobe Dynamic Media Classic HTML5 ビデオビューアと混在メディアビューアで機能します。 ビデオプレーヤーは、Adobe Analytics ビデオレポート内で表示するためのトラッキングデータを生成します。

* ストリーミングメディアと「ハートビート測定」の概要については、を参照してください。 [ストリーミングメディア用 Adobe Analyticsについて](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* Adobe Analytics ビデオレポートとAdobe Dynamic Media Classicの統合では、ソリューション変数をサポートしていますが、カスタム変数はサポートしていません。

  参照： [オーディオおよびビデオパラメーター](https://experienceleague.adobe.com/en/docs/media-analytics/using/implementation/variables/audio-video-parameters) ソリューション変数とカスタム変数について詳しくは、こちらを参照してください。

* 標準提供の 1 分単位のセグメントがサポートされています。 ただし、時間増分、マイルストーン率（%）、オフセットマイルストーンに基づく顧客定義のマイルストーンなど、カスタムセグメントレポートはサポートされていません。

  ストリーミングメディアの要件と設定について詳しくは、を参照してください。 [Adobe Analyticsの Steaming Media を測定](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-overview).

* カスタム変数とソリューション変数については、を参照してください。 [メディアレポートの有効化](https://experienceleague.adobe.com/en/docs/media-analytics/using/media-reports/media-reports-enable#media-reports).

>[!NOTE]
>
>ライセンス取得済みのAdobe Analytics ソリューションにビデオハートビートが含まれていない場合は、この章で説明している手順を引き続き使用して、Adobe Analytics変数をAdobe Dynamic Media Classic ビューアイベントおよび変数に割り当てます。
