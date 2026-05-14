---
title: Media Portal画面のカスタマイズ
description: Adobe Dynamic Media ClassicでMedia Portal画面をカスタマイズする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:43:32.877Z'
TQID: 'https://experienceleague.adobe.com/tIJ90TIWEvVbRT1LR-z8ajTrx2zEXg33V8Q9SgOfzKY'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 329
ht-degree: 18%

---

# Media Portal画面のカスタマイズ{#customizing-the-media-portal-screen}

Media Portal スタイル設定によって、Media Portal 画面に自社ロゴとカラーを使用してブランド化できます。 スタイル設定を使用して、Media Portalで会社のブランディングを設定します。

スタイル設定にアクセスするには、**[!UICONTROL 設定]** > **[!UICONTROL メディアポータル設定]** > **[!UICONTROL スタイル設定]**&#x200B;に移動します。 設定を作成した後で、設定を保存するには、**[!UICONTROL 保存]**&#x200B;を選択してください。 **[!UICONTROL 復元]**&#x200B;を選択して、デフォルト設定を復元できます。 選択すると、プレビューパネルに表示される内容が表示されます。

* **[!UICONTROL ロゴ]**:「**[!UICONTROL 参照]**」を選択し、「ロゴ画像を選択」ウィンドウでグラフィックを選択します。

* **[!UICONTROL アプリケーション]**：背景グラデーションカラーのメニューで選択して、グラデーションカラーブレンドを作成します。

* **[!UICONTROL ツリー]**: ロールオーバーの色と選択範囲の色を選択します。

* **[!UICONTROL アコーディオン]**：詳細表示で画面の右側に表示されるアコーディオンの背景色、境界線スタイル、ロールオーバーおよび選択した色を選択します。

* **[!UICONTROL アコーディオンヘッダー]**: アコーディオンヘッダーの太字のテキストを作成するかどうかを選択します。

* **[!UICONTROL データグリッド]**: データグリッドのヘッダー行の色を選択します。

* **[!UICONTROL アラート]**：アラートメッセージボックスの背景色を選択します。

* **[!UICONTROL 進行状況バー]**: アップロードとダウンロードの進行状況を示すバーの色を選択します。

Media Portal ユーザーが選択したスタイル設定を表示するには、Media PortalにアクセスするURLに`?company=(company name)`を追加する必要があります。 例えば、スタイル設定を表示するには、次の場所にあるPortalCo会社にアクセスするMedia Portal ユーザーを指定します。

`https://s7sps1.scene7.com/MediaPortal`

代わりに、次のURLを使用してください。

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

URLに会社名を含めると、Media Portalはユーザーがどの会社にアクセスしたいかを認識し、それに応じて会社のスタイル設定を適用できます。

Media Portal ユーザーに URL の変更について伝え、新しいユーザーが正確な Media Portal URL を受け取るようにご案内の電子メールメッセージを設定する方法については、他の項で詳しく説明しています。

[Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。
