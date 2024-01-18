---
title: Adobe Analyticsにログオンします。
description: Adobe Dynamic Media ClassicからAdobe Analyticsにログオンする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: e5b510a8-8b7f-4c60-869e-d664a8157e63
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---

# Adobe Analyticsにログオンします。{#log-in-to-adobe-analytics}

ログインしてAdobe Analyticsレポートを設定し、Adobe Analyticsレポート変数をAdobe Dynamic Media Classicイベントに一致させる前に、Adobe Analyticsの Web サービスアクセスグループのメンバーであることを確認します。 このグループのメンバーは、インターフェイスで設定されている権限に関係なく、Experience Cloudの Web Services API を通じて、指定したレポートスイート内のすべてのレポートにアクセスできます。 メンバーをグループに追加するには、Adobe Analyticsで、 **[!UICONTROL 管理ツール]** > **[!UICONTROL ユーザー管理]** > **[!UICONTROL グループの編集]**.

ログインする際に、最新のビデオ分析実装を使用するために、Experience Cloudの組織 ID を入力することもできます。 ID を入力しない場合、ビデオレポートは引き続き機能します。 ただし、Adobe Dynamic Media Classic外部のクライアントの他のデータとデータが正しく統合されない場合があります。

>[!NOTE]
>
>Adobe Analyticsアカウントがログイン用にAdobe IMSベースの認証 (Identity Management System) に移行されている場合、直接の資格情報の入力は機能しません。

## Adobe Dynamic Media ClassicからAdobe Analyticsにログオンします。 {#log-in-to-analytics-from-dmc}

まず、Dynamic Media ClassicをAdobe Analytics OAuth と統合します。 Adobe Analytics OAuth とDynamic Media Classicの統合は、通常、ユーザーごとに 1 回だけおこなわれます。

1. アクセス [Adobe Developer Console](https://developer.adobe.com/console). アカウントに、統合が必要な組織の管理者権限があることを確認します。
1. ホームページの右上隅付近にあるドロップダウンリストから、適切な会社を選択します。 （以下のスクリーンショットは、情報を提供する目的でのみ使用されます。選択する実際の会社名は異なる場合があります。）

   ![新しいプロジェクトを作成](assets/analytics-oauth1.png)

1. 次のいずれかの操作を行います。

   * ページ上部の、 **[!UICONTROL ホーム]** タブ、選択 **[!UICONTROL 新規プロジェクトを作成]**.
   * ページ上部の、 **[!UICONTROL プロジェクト]** タブをクリックします。 ページの右隅にある「 」を選択します。 **[!UICONTROL 新規プロジェクトを作成]**.

1. プロジェクトのページで、「 」を選択します。 **[!UICONTROL API を追加]**.
1. 次の日： **[!UICONTROL API を追加]** ページ、選択 **[!UICONTROL Adobe Analytics]**.
1. ページの右下隅にある「 」を選択します。 **[!UICONTROL 次へ]**.

   ![API を追加](assets/analytics-oauth2.png)

1. 次の日： **[!UICONTROL API の設定]** ページ、選択 **[!UICONTROL ユーザー認証 OAuth]**.
1. ページの右下隅にある「 」を選択します。 **[!UICONTROL 次へ]**.
1. 次の日： **[!UICONTROL API の設定]** ページ、選択 **[!UICONTROL OAUTH 2.0 Web]**.
1. Adobe Analytics の **[!UICONTROL デフォルトのリダイレクト URI]** テキストフィールドに、次のパスを次のように正確に入力します。

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. Adobe Analytics の **[!UICONTROL リダイレクト URI パターン]** テキストフィールドに、次のパスを次のように正確に入力します。

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. ページの右下隅で、「 **[!UICONTROL 設定済み API を保存]**.
1. ナビゲーションパネルで、Adobe Analyticsページの左側の、 **[!UICONTROL 資格情報]**&#x200B;を選択します。 **[!UICONTROL OAuth Web]**.
1. の下 **[!UICONTROL 資格情報の詳細]**、次の操作を実行します。
   * の下 **[!UICONTROL クライアント ID]**&#x200B;を選択します。 **[!UICONTROL コピー]** をクリックして、値をコピーします。 後続のDynamic Media Classicデスクトップアプリケーションでの Analytics 設定にこの値が必要です。
   * の下 **[!UICONTROL クライアントの秘密鍵]**&#x200B;を選択します。 **[!UICONTROL クライアント秘密鍵を取得]** をクリックすると、関連する値が表示されます。 選択 **[!UICONTROL コピー]** をクリックして、値をコピーします。 後続のDynamic Media ClassicデスクトップアプリケーションでのAdobe Analytics設定にこの値が必要です。

## Adobe Dynamic Media ClassicでのAdobe Analyticsの設定 {#configure-analytics-in-dmc}

>[!NOTE]
>
>Dynamic Media ClassicでのAdobe Analyticsの初期設定後、設定をやり直す必要があるのは次の場合のみです。
>
>* Analytics に新しいレポートが追加され、その新しいレポートへのデータの送信を開始しようとしています。
>* トラッキングサーバーがAdobe Analyticsで更新されました。
>* レポートに新しいトラッキング変数が導入され、Dynamic Media Classicユーザーインターフェイスの特定のビューア変数をその新しい Analytics 変数にリンクする場合。
>

1. Adobe Dynamic Media Classicデスクトップアプリケーションの右上隅近くにある、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]**.
1. 左側のパネルで、 **[!UICONTROL アプリケーション設定]**&#x200B;を選択します。 **[!UICONTROL Adobe Analytics]**.
1. 次の日： **[!UICONTROL Adobe Analytics Configuration]** ページ、選択 **[!UICONTROL Adobe Analytics Login]**.
1. Adobe Analytics の **[!UICONTROL Adobe Analytics Login]** ダイアログボックス、 **[!UICONTROL クライアント ID]** フィールドと **[!UICONTROL クライアント秘密鍵]** 「 」フィールドに、前にコピーしたそれぞれの値を貼り付けます。
1. ダイアログボックスの右下隅で、 **[!UICONTROL ログイン]** Adobe IMS(Identity Management Services) ログインを実行します。

   正常にログインすると、Adobe Analyticsログインダイアログボックスが再び表示され、 **[!UICONTROL 会社]** ドロップダウンリスト（自分が使用できる会社によって開始）。

1. 次から： **[!UICONTROL 会社]** 」ドロップダウンリストから、会社を選択します。

   会社を選択すると、 **[!UICONTROL スイーツ]** 選択した会社で使用可能なレポートスイートによって開始されたドロップダウンリストが表示されます。

1. 次から： **[!UICONTROL スイーツ]** 」ドロップダウンリストから、レポートスイートを選択します。

   >[!NOTE]
   >
   >デフォルトでは、ユーザーは、 **[!UICONTROL 会社]** および **[!UICONTROL スイーツ]** ドロップダウンリストが空です。 したがって、ユーザーは各リストから値を選択する必要があります。

1. 選択 **[!UICONTROL OK]** 設定を保存できます。

   >[!NOTE]
   >
   >The **[!UICONTROL Adobe Analytics Server]** フィールドには、 **[!UICONTROL OK]**. 別のトラッキングサーバーを使用する場合は、データの損失を避けるために、このフィールドで更新します。

1. Adobe Analytics設定ページの左下隅で、「 **[!UICONTROL 保存]** Adobe Analyticsアカウントの設定を確実に更新する場合。

>[!MORELIKETHIS]
>
>* [Adobe Analyticsレポートの設定](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
