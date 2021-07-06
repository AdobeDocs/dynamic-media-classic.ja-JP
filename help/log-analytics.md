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
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
source-git-commit: 885fcd16559d31d3b9bad88705b4b6bec18515ee
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 27%

---

# Adobe Analytics へのログイン{#log-in-to-adobe-analytics}

ログインしてAdobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をDynamic Media Classicイベントに設定する前に、Adobe AnalyticsのWebサービスアクセスグループのメンバーであることを確認します。 このグループのメンバーは、インターフェイスで設定されている権限に関係なく、Experience CloudのWebサービスAPIを介して、指定したレポートスイートのすべてのレポートにアクセスできます。 グループにメンバーを追加するには、Adobe Analytics で、**[!UICONTROL 管理ツール]**／**[!UICONTROL ユーザー管理]**／**[!UICONTROL グループの編集]**&#x200B;をクリックします。

ログインする際に、最新のビデオ分析実装を使用するために、Experience Cloud組織IDを入力するオプションがあります。 IDを入力しない場合、ビデオレポートは引き続き機能します。 ただし、Dynamic Media Classicの外部からそのクライアントの他のデータとデータが正しく統合されない可能性があります。

>[!NOTE]
>
>Adobe AnalyticsアカウントがAdobeIMSベースの認証(Identity Managementシステム)に移行されてログインした場合、直接の資格情報の入力は機能しません。

**Adobe Analytics にログインするには:**

1. Dynamic Media Classicページの右上隅付近にある「**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]**」をタップします。
1. 左側のウィンドウの「**[!UICONTROL アプリケーション設定]**」で、「**[!UICONTROL Adobe Analytics]**」をタップします。
1. Adobe Analytics設定ページで、「**[!UICONTROL Adobe Analyticsログイン]**」をタップします。
1. 「**[!UICONTROL Adobe Analyticsログイン]**」ダイアログボックスで、会社名、Experience Cloud組織ID（オプション）、ユーザー名および&#x200B;*共有暗号鍵*&#x200B;を「**[!UICONTROL パスワード]**」テキストフィールドに入力します。

   *共有暗号鍵*&#x200B;をAnalyticsAdmin Consoleから取得できます。 [ユーザーアカウントのAPI資格情報を取得する方法](https://github.com/AdobeDocs/analytics-2.0-apis/blob/master/create-oauth-client.md)を参照してください。

1. 「**[!UICONTROL ログイン]**」をクリックします。
1. **[!UICONTROL レポートスイート]**&#x200B;ドロップダウンメニューで、レポートスイートを選択し、「**[!UICONTROL OK]**」をクリックします。

   >[!NOTE]
   >
   >Adobe Analytics に初めてログインしたとき、「レポートスイート」ドロップダウンリストは空白です。初めてログインしたときにはレポートスイートを選択しません。初めてログインした後、いったんログアウトしてから、Adobe Analytics 画面に戻ります。もう一度ログインすると、レポートスイートを選択できるようになります。

>[!MORELIKETHIS]
>
>* [Adobe Analytics レポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)

