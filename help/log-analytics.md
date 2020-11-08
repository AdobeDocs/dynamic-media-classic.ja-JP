---
title: Adobe Analytics へのログイン
seo-title: Adobe Analytics へのログイン
description: 'null'
seo-description: Adobe Analyticsへのログイン方法を説明します。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 36%

---


# Adobe Analytics へのログイン{#log-in-to-adobe-analytics}

ログインしてAdobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をDynamic Media Classicイベントに対応付ける前に、Adobe Analyticsの「Webサービスへのアクセス」グループのメンバーとして追加されていることを確認します。 このグループのメンバーは、インターフェイスで設定された権限に関係なく、Marketing Cloud の Web Services API 経由で指定したレポートスイートの全レポートにアクセスできます。グループにメンバーを追加するには、Adobe Analytics で、**管理ツール**／**ユーザー管理**／**グループの編集**&#x200B;をクリックします。

ログイン時に、Marketing Cloud組織IDを入力して、最新のビデオ分析を使用することもできます。 IDを入力しない場合でも、ビデオレポートは機能します。 ただし、Dynamic Media Classicの外部のクライアントの他のデータとデータが正しく統合されない可能性があります。

>[!NOTE]
>
>Adobe Analyticsアカウントがログイン用にAdobeIMSベースの認証(Identity Managementシステム)に移行された場合、直接的な資格情報の入力は機能しません。

**Adobe Analytics にログインするには**

1. ダイナミックメディアクラシックページの右上隅近くにある設定/アプリケーション **[!UICONTROL 設定をタップします]**。
1. In the left pane, under **[!UICONTROL Application Setup]**, tap **[!UICONTROL Adobe Analytics]**.
1. In the Adobe Analytics Configuration page, tap **[!UICONTROL Adobe Analytics Login]**.
1. [ **[!UICONTROL Adobe Analyticsログイン]** ]ダイアログボックスで、[パスワード ** ]テキストフィールドに会社名、Marketing Cloud組織ID （オプション）、ユーザ名、 **** 共有秘密キーを入力します。

   Analytics管理コンソールから *共有秘密* キーを取得できます。 ユーザーアカウントのAPI証明書の取得 [方法を参照してください](https://helpx.adobe.com/analytics/kb/how-to-get-api-credentials-for-user-accounts-.html)。

1. 「**[!UICONTROL ログイン]**」をクリックします。
1. 「 **[!UICONTROL レポートスイート]** 」ドロップダウンメニューで、レポートスイートを選択し、「 **[!UICONTROL OK]**」をクリックします。

   >[!NOTE]
   >
   >Adobe Analytics に初めてログインしたとき、「レポートスイート」ドロップダウンリストは空白です。初めてログインしたときにはレポートスイートを選択しません。初めてログインした後、いったんログアウトしてから、Adobe Analytics 画面に戻ります。もう一度ログインすると、レポートスイートを選択できるようになります。

>[!MORELIKETHIS]
>
>* [Adobe Analytics レポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

