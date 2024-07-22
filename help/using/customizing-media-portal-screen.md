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
source-git-commit: 00591bdbe721035e25d3dea245a2110f978d19aa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 17%

---

# メディアポータル画面のカスタマイズ{#customizing-the-media-portal-screen}

Media Portal スタイル設定によって、Media Portal 画面に自社ロゴとカラーを使用してブランド化できます。スタイル設定を使用して、メディアポータルに会社のブランディングを配置します。

スタイル設定にアクセスするには、**[!UICONTROL 設定]**/**[!UICONTROL メディアポータル設定]**/**[!UICONTROL スタイル設定]** に移動します。 設定を行った後は、必ず「**[!UICONTROL 保存]**」を選択して設定を保存してください。 「**[!UICONTROL 復元]**」を選択して、デフォルト設定に戻すことができます。 選択すると、プレビューパネルにその表示方法が表示されます。

* **[!UICONTROL ロゴ]**:「**[!UICONTROL 参照]**」を選択して、ロゴ画像を選択ウィンドウでグラフィックを選択します。

* **[!UICONTROL アプリケーション]**：背景のグラデーションカラーのメニューで選択して、グラデーションカラーブレンドを作成します。

* **[!UICONTROL ツリー]**：ロールオーバーカラーと選択カラーを選択します。

* **[!UICONTROL アコーディオン]**：詳細表示で画面の右側に表示されるアコーディオンについて、背景色、境界線のスタイル、ロールオーバーおよび選択した色を選択します。

* **[!UICONTROL アコーディオンヘッダー]**：アコーディオンヘッダーの太字でテキストを作成するかどうかを選択します。

* **[!UICONTROL Datagrid]**：データグリッドのヘッダー行の色を選択します。

* **[!UICONTROL アラート]**：アラートメッセージボックスの背景色を選択します。

* **[!UICONTROL プログレスバー]**：アップロードおよびダウンロードの進行状況を示すバーの色を選択します。

Media Portal ユーザーに選択したスタイル設定が表示されるようにするには、Media Portal にアクセスする URL に `?company=(company name)` を追加する必要があります。 例えば、スタイル設定を確認するには、以下で PortalCo 会社にアクセスする Media Portal ユーザーを参照してください。

`https://s7sps1.scene7.com/MediaPortal`

代わりに、次の URL を使用します。

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

URL に会社名を含めると、Media Portal はユーザーがアクセスを希望している会社を認識し、それに応じて会社のスタイル設定を適用することができます。

Media Portal ユーザーに URL の変更について伝え、新しいユーザーが正確な Media Portal URL を受け取るようにご案内の電子メールメッセージを設定する方法については、他の項で詳しく説明しています。

[Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。
