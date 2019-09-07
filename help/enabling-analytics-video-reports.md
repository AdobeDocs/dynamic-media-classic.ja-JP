---
title: Adobe Analytics ビデオレポートの有効化
seo-title: Adobe Analytics ビデオレポートの有効化
description: 'null'
seo-description: Adobe Analyticsビデオレポートを有効にする方法について説明します。
uuid: 078594b2-7d53-4714-8128- ff3b5c3a5e36
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/adobe_ analytics_ recurtion_ kit
discoiquuid: 18644a53-92da-40ab- b961-318d8332c54d
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Adobe Analytics ビデオレポートの有効化{#enabling-adobe-analytics-video-reports}

Adobe Analyticsハートビートベースのビデオレポートを使用して、Dynamic Media ClassicでAdobe Analyticsを設定する際に4つのビデオビューアイベント（再生、一時停止、停止、マイルストーン）を有効にする必要がなくなりました。ビデオハートビートは、標準搭載のダイナミックメディアクラシックHTML5ビデオおよびMixedMediaビューアで動作します。ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。

* Adobe Analyticsビデオレポートの統合は、ソリューション変数をサポートしますが、カスタム変数はサポートしません。

   See [Configure Analytics Video Reporting](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/video_analytics_config.html) for more information about solution variables and custom variables.

* 標準搭載された 1 分単位のセグメントはサポートされますが、カスタムセグメントレポート（時間単位に基づいたユーザー定義のマイルストーン、％マイルストーン、オフセットマイルストーンなど）はサポートされません。

For more information about Video Heartbeat requirements and setup, see [Measuring Video in Adobe Analytics using Video Heartbeat](https://microsite.omniture.com/t2/help/en_US/sc/appmeasurement/hbvideo/).

>[!NOTE]
>
>ライセンスされているAdobe Analyticsソリューションにビデオハートビートが含まれていない場合は、この章で説明する手順を使用して、Adobe Analytics変数をDynamic Media Classicビューアイベントおよび変数に割り当てる必要があります。

