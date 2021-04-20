---
title: Adobe Analytics へのログイン
description: Adobe Analyticsへのログイン方法を説明します。
uuid: 5614babe-1097-4228-a3dc-27e5a25366d5
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Administrator,Business Practitioner
translation-type: tm+mt
source-git-commit: e727c1b5fb43c7def842ff1bafcc8b3ef3437cde
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 35%

---


# Adobe Analytics へのログイン{#log-in-to-adobe-analytics}

ログインしてAdobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をDynamic Mediaクラシックイベントに一致させる前に、Adobe Analyticsの[Webサービスへのアクセス]グループのメンバーとして追加されていることを確認します。 このグループのメンバーは、インターフェイスで設定された権限に関係なく、Marketing Cloud の Web Services API 経由で指定したレポートスイートの全レポートにアクセスできます。グループにメンバーを追加するには、Adobe Analytics で、**管理ツール**／**ユーザー管理**／**グループの編集**&#x200B;をクリックします。

ログイン時に、Marketing Cloud組織IDを入力して、最新のビデオ分析を使用することもできます。 IDを入力しない場合でも、ビデオレポートは機能します。 ただし、Data Classicの外部のクライアントの他のデータとデータが正しく統合されない可能性があります。

>[!NOTE]
>
>Adobe Analyticsアカウントがログイン用にAdobeIMSベースの認証(Identity Managementシステム)に移行された場合、直接的な資格情報の入力は機能しません。

**Adobe Analytics にログインするには**

1. Dynamic Mediaクラシックページの右上隅近くにある&#x200B;**[!UICONTROL セットアップ/アプリケーション設定]**&#x200B;をタップします。
1. 左側のウィンドウの「**[!UICONTROL アプリケーション設定]**」で、**[!UICONTROL Adobe Analytics]**&#x200B;をタップします。
1. Adobe Analytics設定ページで、**[!UICONTROL Adobe Analyticsログイン]**&#x200B;をタップします。
1. **[!UICONTROL Adobe Analyticsログイン]**&#x200B;ダイアログボックスで、会社名、Marketing Cloud組織ID（オプション）、ユーザー名、*共有秘密*&#x200B;キーを&#x200B;**[!UICONTROL パスワード]**&#x200B;テキストフィールドに入力します。

   Analytics管理コンソールから&#x200B;*共有暗号鍵*&#x200B;キーを取得できます。 [ユーザーアカウントのAPI資格情報を取得する方法](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md)を参照してください。

1. 「**[!UICONTROL ログイン]**」をクリックします。
1. **[!UICONTROL レポートスイート]**&#x200B;ドロップダウンメニューで、レポートスイートを選択し、**[!UICONTROL 「OK]**」をクリックします。

   >[!NOTE]
   >
   >Adobe Analytics に初めてログインしたとき、「レポートスイート」ドロップダウンリストは空白です。初めてログインしたときにはレポートスイートを選択しません。初めてログインした後、いったんログアウトしてから、Adobe Analytics 画面に戻ります。もう一度ログインすると、レポートスイートを選択できるようになります。

>[!MORELIKETHIS]
>
>* [Adobe Analytics レポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

