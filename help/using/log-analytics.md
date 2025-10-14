---
title: Adobe Analyticsへのログオン
description: Adobe Dynamic Media ClassicからAdobe Analyticsにログオンする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 261b8f7c-c61c-4ce3-b9dc-8549347aca2e
topic: Integrations, Development
level: Experienced
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 0%

---

# Adobe Analyticsへのログオン{#log-in-to-adobe-analytics}

Adobe Analyticsの Web サービスアクセスグループのメンバーであることを確認します。 Adobe Analytics レポートを設定し、Adobe Analytics レポート変数をAdobe Dynamic Media Classic イベントと照合するには、ログインする前に行います。 このグループのメンバーは、指定されたレポートスイートのすべてのレポートにアクセスできます。 インターフェイスで設定されている権限に関係なく、Experience Cloud Web サービス API を使用して設定します。 グループにメンバーを追加するには、Adobe Analyticsで **[!UICONTROL 管理ツール]**/**[!UICONTROL User Management]**/**[!UICONTROL グループを編集]** に移動します。

ログインしたら、Experience Cloud組織 ID を入力して最新のビデオ分析実装を使用することもできます。 ID を入力しない場合でも、ビデオレポートは機能します。 ただし、Adobe Dynamic Media Classicの外部からのそのクライアントの他のデータと正しく統合されない可能性があります。

>[!NOTE]
>
>ログインのためにAdobe Analytics アカウントがAdobe IMSベースの認証（Identity Management System）に移行されている場合、直接資格情報の入力は機能しません。

## Adobe Dynamic Media ClassicからAdobe Analyticsへのログオン {#log-in-to-analytics-from-dmc}

最初に、Dynamic Media ClassicをAdobe Analytics OAuth と統合します。 Dynamic Media ClassicとのAdobe Analytics OAuth 統合は、通常、ユーザーごとに 1 回だけ行われます。

1. [Adobe Developer Console](https://developer.adobe.com/console) にアクセスします。 統合が必要な組織の管理者権限がアカウントにあることを確認します。
1. ホームページの右上隅付近にあるドロップダウンリストで適切な会社を選択します。 （以下のスクリーンショットは情報提供のみを目的としています。選択した実際の会社名は異なる場合があります。）

   ![&#x200B; 新規プロジェクトの作成 &#x200B;](assets/analytics-oauth1.png)

1. 次のいずれかの操作をおこないます。

   * ページの上部にある「**[!UICONTROL ホーム]**」タブで「**[!UICONTROL 新規プロジェクトを作成]**」を選択します。
   * ページの上部にある「**[!UICONTROL プロジェクト]** タブから。 ページの右隅付近にある「**[!UICONTROL 新規プロジェクトを作成]**」を選択します。

1. プロジェクトのページで、「**[!UICONTROL API を追加]**」を選択します。
1. **[!UICONTROL API を追加]** ページで、「**[!UICONTROL Adobe Analytics]**」を選択します。
1. ページの右下隅付近にある「**[!UICONTROL 次へ]**」を選択します。

   ![API を追加 &#x200B;](assets/analytics-oauth2.png)

1. **[!UICONTROL `Configure API`]** ページで、「**[!UICONTROL ユーザー認証 OAuth]**」を選択します。
1. ページの右下隅付近にある「**[!UICONTROL 次へ]**」を選択します。
1. **[!UICONTROL `Configure API`]** ページで、「**[!UICONTROL OAUTH 2.0 Web]**」を選択します。
1. 「**[!UICONTROL デフォルトのリダイレクト URI]**」テキストフィールドに、次のパスを示すように正確に入力します。

   `https://exploreadobe.com/dynamic-media-upgrade/`

1. 「**[!UICONTROL リダイレクト URI パターン]**」テキストフィールドに、次のパスを正確に入力します。

   `https://exploreadobe\.com/dynamic-media-upgrade/`

1. ページの右下隅の「**[!UICONTROL 設定済み API を保存]**」を選択します。
1. ナビゲーションパネルのAdobe Analyticsページの左側にある「**[!UICONTROL 資格情報]** の下で、「**[!UICONTROL OAuth Web]**」を選択します。
1. **[!UICONTROL 資格情報の詳細]** で、次の操作を行います。
   * 「**[!UICONTROL クライアント ID]**」で、「**[!UICONTROL コピー]**」を選択して値をコピーします。 この値は、後続のDynamic Media Classic デスクトップアプリケーションで Analytics を設定する際に必要になります。
   * 「**[!UICONTROL クライアント秘密鍵]**」で「**[!UICONTROL クライアント秘密鍵を取得]**」を選択し、関連する値を表示します。 「**[!UICONTROL コピー]**」を選択して、値をコピーします。 この値は、後続のDynamic Media Classic デスクトップアプリケーションでAdobe Analyticsを設定する際に必要になります。

## Adobe Dynamic Media ClassicでのAdobe Analyticsの設定 {#configure-analytics-in-dmc}

>[!NOTE]
>
>Dynamic Media ClassicでのAdobe Analyticsの初期設定後、設定をやり直す必要があるのは次の場合のみです。
>
>* Analytics に新しいレポートが追加され、ユーザーはその新しいレポートへのデータ送信を開始したいと考えています。
>* トラッキングサーバーがAdobe Analyticsで更新されます。
>* レポートに新しいトラッキング変数が導入され、Dynamic Media Classic ユーザーインターフェイスの特定のビューア変数を、その新しい Analytics 変数にリンクするとします。
>

1. Adobe Dynamic Media Classic デスクトップアプリケーションの右上隅付近で、**[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]** に移動します。
1. 左側のパネルの **[!UICONTROL アプリケーション設定]** で、「**[!UICONTROL Adobe Analytics]**」を選択します。
1. **[!UICONTROL Adobe Analytics設定]** ページで、「**[!UICONTROL Adobe Analytics Login]**」を選択します。
1. **[!UICONTROL Adobe Analyticsのログイン]** ダイアログボックスで、「**[!UICONTROL クライアント ID]**」フィールドと「**[!UICONTROL クライアント秘密鍵]**」フィールドに、前にコピーしたそれぞれの値を貼り付けます。
1. ダイアログボックスの右下隅にある「**[!UICONTROL ログイン]**」を選択し、Adobe IMS（Identity Management Services）へのログインを実行します。

   正常にログインすると、使用可能な会社によって開始された **[!UICONTROL 会社]** ドロップダウンリストと共に、Adobe Analyticsのログインダイアログボックスが再び表示されます。

1. **[!UICONTROL 会社]** ドロップダウンリストから、会社を選択します。

   会社を選択すると、選択した会社で使用可能なレポートスイートによって開始される **[!UICONTROL スイート]** ドロップダウンリストが表示されます。

1. **[!UICONTROL スイート]** ドロップダウンリストから、レポートスイートを選択します。

   >[!NOTE]
   >
   >デフォルトでは、「会社」ドロップダウンリストと「**[!UICONTROL スイート]** ドロップダウンリストの両方が空であるという事実をユーザーが認識する必要があります **[!UICONTROL 。]** そのため、ユーザーは各リストから値を選択する必要があります。

1. **[!UICONTROL OK]** を選択して、設定を保存します。

   >[!NOTE]
   >
   >「**[!UICONTROL Adobe Analytics サーバー]**」フィールドには、「**[!UICONTROL OK]**」を選択すると Analytics 名前空間に一致するサードパーティのトラッキングサーバーが候補として表示されます。 別のトラッキングサーバーを使用している場合は、データの損失を避けるために、このフィールドで更新してください。

1. Adobe Analytics設定ページの左下隅の「**[!UICONTROL 保存]**」を選択して、Adobe Analytics アカウント設定が更新されていることを確認します。

>[!MORELIKETHIS]
>
>* [Adobe Analytics レポートの設定 &#x200B;](configuring-analytics-reports.md#configuring_adobe_analytics_reports)
