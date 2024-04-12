---
title: メディアポータル画面のカスタマイズ
description: Adobe Dynamic Media Classicのメディアポータル画面をカスタマイズする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 16%

---

# メディアポータル画面のカスタマイズ{#customizing-the-media-portal-screen}

Media Portal スタイル設定によって、Media Portal 画面に自社ロゴとカラーを使用してブランド化できます。スタイル設定を使用して、メディアポータルに会社のブランディングを配置します。

スタイル設定にアクセスするには、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL メディアポータルの設定]** > **[!UICONTROL スタイル設定]**. 必ずを選択してください **[!UICONTROL 保存]** をクリックして、設定後に保存します。 以下を選択できます。 **[!UICONTROL 復元]** をクリックして、デフォルト設定に戻します。 選択すると、プレビューパネルにその表示方法が表示されます。

* **[!UICONTROL ロゴ]**  – を選択 **[!UICONTROL 参照]**&#x200B;を選択し、ロゴ画像を選択ウィンドウでグラフィックを選択します。

* **[!UICONTROL 用途]**  – 背景のグラデーションカラーのメニューを選択して、グラデーションカラーブレンドを作成します。

* **[!UICONTROL ツリー]** - ロールオーバーカラー（ポインターを項目の上に移動したときに表示されるカラー）と選択カラー（項目を選択したときに表示されるカラー）を選択します。

* **[!UICONTROL アコーディオン]**  – 詳細表示で画面の右側に表示されるアコーディオンについて、背景色、境界線のスタイル、ロールオーバーおよび選択した色を選択します。

* **[!UICONTROL アコーディオンヘッダー]** - アコーディオンヘッダーの太字でテキストを作成するかどうかを選択します。

* **[!UICONTROL Datagrid]** - データグリッドのヘッダー行の色を選択します。

* **[!UICONTROL アラート]** - アラートメッセージボックスの背景色を選択します。

* **[!UICONTROL プログレスバー]** - アップロードおよびダウンロードの進行状況を示すバーの色を選択します。

Media Portal ユーザーに選択したスタイル設定が表示されるようにするには、次を追加する必要があります `?company=(company name)` からメディアポータルにアクセスする URL。 例えば、スタイル設定を確認するには、以下で PortalCo 会社にアクセスする Media Portal ユーザーを参照してください。

`https://s7sps1.scene7.com/MediaPortal`

代わりに、次の URL を使用します。

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

URL に会社名を含めると、Media Portal はユーザーがアクセスを希望している会社を認識し、それに応じて会社のスタイル設定を適用することができます。

Media Portal ユーザーに URL の変更について伝え、新しいユーザーが正確な Media Portal URL を受け取るようにご案内の電子メールメッセージを設定する方法については、他の項で詳しく説明しています。

[Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。
