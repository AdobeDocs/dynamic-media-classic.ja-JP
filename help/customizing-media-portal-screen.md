---
title: Media Portal 画面のカスタマイズ
description: Media Portal画面をカスタマイズする方法を説明します。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
feature: Dynamic Mediaクラシック，コラボレーション，アセット管理
role: Administrator,Business Practitioner
exl-id: b0c5f70a-2388-42aa-a1ed-fd745ff90518
translation-type: tm+mt
source-git-commit: 4e79c98b92dfa4e1a9890ed8a291cdf564126466
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 46%

---

# Media Portal 画面のカスタマイズ{#customizing-the-media-portal-screen}

Media Portal スタイル設定によって、Media Portal 画面に自社ロゴとカラーを使用してブランド化できます。スタイル設定を使用して、Media Portalに会社のブランドを設定します。

スタイル設定にアクセスするには、**[!UICONTROL 設定]**／**[!UICONTROL Media Portal 設定]**／**[!UICONTROL スタイル設定]**&#x200B;を選択します。変更を加えたら、必ず&#x200B;**[!UICONTROL 「保存」]**&#x200B;をクリックして設定を保存します。**[!UICONTROL 「復元」]**&#x200B;をクリックすると、デフォルト設定に戻ります。選択する際、プレビューパネルで選択内容のプレビューを確認できます。

* **Logo**  - 「 **** 参照」をクリックし、ロゴイメージを選択ウィンドウでグラフィックを選択します。

* **アプリケーション**  — 背景のグラデーションの色メニューで選択を行い、グラデーションカラーブレンドを作成します。

* **ツリー**  — ロールオーバーのカラー（ポインタを項目の上に移動したときに表示されるカラー）と選択のカラー（項目を選択したときに表示されるカラー）を選択します。

* **アコーディオン**  — 詳細表示の画面の右側に表示されるアコーディオンの背景色、境界線のスタイル、ロールオーバーおよび選択色を選択します。

* **アコーディオンヘッダ**  — アコーディオンヘッダ内のテキストを太字にするかどうかを選択します。

* **Datagrid**  — データグリッドのヘッダー行の色を選択します。

* **警告**  — 警告メッセージボックスの背景色を選択します。

* **プログレスバー**  — アップロードおよびダウンロードの進行状況を示すバーの色を選択します。

Media Portalユーザが選択したスタイル設定を表示するには、Media PortalにアクセスするURLに`?company=(company name)`を追加する必要があります。 例えば、次の URL にある PortalCo という会社にアクセスする Media Portal ユーザーがスタイル設定を表示するとします。

`https://s7sps1.scene7.com/MediaPortal`

代わりに、次のURLを使用します。

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

会社名に URL を含めることで、Media Portal はユーザがアクセスしようとしている会社を認識して、その会社のスタイル設定を適用できるようになります。

Media Portal ユーザーに URL の変更について伝え、新しいユーザーが正確な Media Portal URL を受け取るようにご案内の電子メールメッセージを設定する方法については、他の項で詳しく説明しています。

[Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。
