---
title: Media Portal 画面のカスタマイズ
seo-title: Media Portal 画面のカスタマイズ
description: 'null'
seo-description: Media Portal画面のカスタマイズ方法を説明します。
uuid: bd1a65a6-723b-49d0-8eac-849da00e0e1a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 8b000c25-c9c3-481e-9b25-96257471571f
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# Media Portal 画面のカスタマイズ{#customizing-the-media-portal-screen}

Media Portal スタイル設定によって、Media Portal 画面に自社ロゴとカラーを使用してブランド化できます。スタイル設定を使用して Media Portal に会社のスタンプを配置します。

スタイル設定にアクセスするには、**設定**／**Media Portal 設定**／**スタイル設定**&#x200B;を選択します。変更を加えたら、必ず&#x200B;**「保存」**&#x200B;をクリックして設定を保存します。**「復元」**&#x200B;をクリックすると、デフォルト設定に戻ります。選択する際、プレビューパネルで選択内容のプレビューを確認できます。

**ロゴ** 「参照」をクリックし、ロゴイメージを選択ウィンドウでグラフィックを選択します。

**アプリケーション** [背景のグラデーションの色]メニューで選択を行い、グラデーションの色をブレンドします。

**ツリー** ：ロールオーバーカラー（ポインタをアイテムの上に移動したときに表示されるカラー）と選択カラー（アイテムを選択したときに表示されるカラー）を選択します。

**アコーディオン** ：詳細表示の画面の右側に表示されるアコーディオンの背景色、境界線のスタイル、ロールオーバーおよび選択した色を選択します。

**アコーディオンヘッダ** ：アコーディオンヘッダのテキストを太字にするかどうかを選択します。

**Datagrid** データグリッドのヘッダー行の色を選択します。

**警告** ：警告メッセージボックスの背景色を選択します。

**プログレスバー** ：アップロードとダウンロードの進行状況を示すバーの色を選択します。

For Media Portal users to see the style settings you choose, they must append `?company=(company name)` to the URL with which they access Media Portal. 例えば、次の URL にある PortalCo という会社にアクセスする Media Portal ユーザーがスタイル設定を表示するとします。

`https://s7sps1.scene7.com/MediaPortal`

その場合、代わりに次の URL を使用することになります。

`https://s7sps1.scene7.com/MediaPortal?company=PortalCo`

会社名に URL を含めることで、Media Portal はユーザがアクセスしようとしている会社を認識して、その会社のスタイル設定を適用できるようになります。

Media Portal ユーザーに URL の変更について伝え、新しいユーザーが正確な Media Portal URL を受け取るようにご案内の電子メールメッセージを設定する方法については、他の項で詳しく説明しています。

[Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。
