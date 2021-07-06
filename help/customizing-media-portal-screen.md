---
title: Media Portal 画面のカスタマイズ
description: Media Portal画面をカスタマイズする方法を説明します。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 46%

---

# Media Portal 画面のカスタマイズ{#customizing-the-media-portal-screen}

Media Portal スタイル設定によって、Media Portal 画面に自社ロゴとカラーを使用してブランド化できます。スタイル設定を使用して、会社のブランディングをMedia Portalに配置します。

スタイル設定にアクセスするには、**[!UICONTROL 設定]**／**[!UICONTROL Media Portal 設定]**／**[!UICONTROL スタイル設定]**&#x200B;を選択します。変更を加えたら、必ず&#x200B;**[!UICONTROL 「保存」]**&#x200B;をクリックして設定を保存します。**[!UICONTROL 「復元」]**&#x200B;をクリックすると、デフォルト設定に戻ります。選択する際、プレビューパネルで選択内容のプレビューを確認できます。

* **ロゴ**  - 「参照」をク **** リックし、ロゴ画像を選択ウィンドウでグラフィックを選択します。

* **適用**  — 背景のグラデーションの色メニューで選択を行い、グラデーションカラーのブレンドを作成します。

* **ツリー**  — ロールオーバーカラー（ポインターを項目の上に移動すると表示されるカラー）と選択カラー（項目を選択すると表示されるカラー）を選択します。

* **アコーディオン**  — 詳細ビューの画面の右側に表示されるアコーディオンの背景色、境界線のスタイル、ロールオーバーおよび選択した色を選択します。

* **アコーディオンヘッダー**  — アコーディオンヘッダーの太字でテキストを作成するかどうかを選択します。

* **Datagrid**  — データグリッドのヘッダー行の色を選択します。

* **アラート**  — アラートメッセージボックスの背景色を選択します。

* **プログレスバー**  — アップロードおよびダウンロードの進行状況を示すバーの色を選択します。

Media Portalユーザーが選択したスタイル設定を表示するには、Media PortalにアクセスするURLに`?company=(company name)`を追加する必要があります。 例えば、次の URL にある PortalCo という会社にアクセスする Media Portal ユーザーがスタイル設定を表示するとします。

`https://s7sps1.scene7.com/MediaPortal`

代わりに、次のURLを使用します。

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

会社名に URL を含めることで、Media Portal はユーザがアクセスしようとしている会社を認識して、その会社のスタイル設定を適用できるようになります。

Media Portal ユーザーに URL の変更について伝え、新しいユーザーが正確な Media Portal URL を受け取るようにご案内の電子メールメッセージを設定する方法については、他の項で詳しく説明しています。

[Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。
