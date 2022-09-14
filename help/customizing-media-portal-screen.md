---
title: Media Portal 画面のカスタマイズ
description: Adobe Dynamic Media Classicの Media Portal 画面をカスタマイズする方法を説明します。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 32%

---

# Media Portal 画面のカスタマイズ{#customizing-the-media-portal-screen}

Media Portal スタイル設定によって、Media Portal 画面に自社ロゴとカラーを使用してブランド化できます。スタイル設定を使用して、会社のブランディングを Media Portal に配置します。

スタイル設定にアクセスするには、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal の設定]** > **[!UICONTROL スタイル設定]**. 必ず **[!UICONTROL 保存]** 設定を保存します。 次を選択できます。 **[!UICONTROL 復元]** をクリックしてデフォルト設定を元に戻します。 選択を行うと、プレビューパネルにその外観が表示されます。

* **[!UICONTROL ロゴ]**  — 選択 **[!UICONTROL 参照]**&#x200B;をクリックし、ロゴイメージを選択ウィンドウでグラフィックを選択します。

* **[!UICONTROL アプリ]**  — 背景のグラデーションの色メニューで選択を行い、グラデーションの色のブレンドを作成します。

* **[!UICONTROL ツリー]**  — ロールオーバーカラー（ポインターを項目の上に移動したときに表示されるカラー）と選択カラー（項目を選択したときに表示されるカラー）を選択します。

* **[!UICONTROL アコーディオン]**  — 詳細ビューの画面の右側に表示されるアコーディオンの背景色、境界線のスタイル、ロールオーバーおよび選択した色を選択します。

* **[!UICONTROL アコーディオンヘッダー]**  — アコーディオンヘッダーの太字でテキストを作成するかどうかを選択します。

* **[!UICONTROL Datagrid]**  — データグリッドのヘッダー行の色を選択します。

* **[!UICONTROL アラート]**  — 警告メッセージボックスの背景色を選択します。

* **[!UICONTROL プログレスバー]**  — アップロードおよびダウンロードの進行状況を示すバーの色を選択します。

Media Portal ユーザーが選択したスタイル設定を表示するには、追加する必要があります `?company=(company name)` を Media Portal にアクセスする際の URL に追加します。 例えば、次の URL にある PortalCo という会社にアクセスする Media Portal ユーザーがスタイル設定を表示するとします。

`https://s7sps1.scene7.com/MediaPortal`

代わりに、次の URL を使用します。

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

会社名に URL を含めることで、Media Portal はユーザがアクセスしようとしている会社を認識して、その会社のスタイル設定を適用できるようになります。

Media Portal ユーザーに URL の変更について伝え、新しいユーザーが正確な Media Portal URL を受け取るようにご案内の電子メールメッセージを設定する方法については、他の項で詳しく説明しています。

[Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。
