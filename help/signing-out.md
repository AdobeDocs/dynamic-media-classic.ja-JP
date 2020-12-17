---
title: AdobeDynamic Mediaクラシックへのサインインとログアウト
description: AdobeDynamic Mediaクラシックへのログインとクラシックからのサインアウト、および北米(NA)、ヨーロッパ、中東、アフリカ(EMEA)、アジア太平洋(APAC)の本番環境サーバーへの接続について説明します。
uuid: eaf51ab7-d17a-4b7b-b6a4-1ec78bfee36b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: ad418881-ff31-43b1-bbb6-ab2fbcf89bea
translation-type: tm+mt
source-git-commit: d3c9b805f5d17c130fe5b4590bd7864351dc9d24
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 4%

---


<!-- UPDATE THIS TOPIC AFTER DECEMBER 31, 2020!!!!! -->

# AdobeDynamic Mediaクラシック{#sign-in}にサインイン

Dynamic Mediaクラシックへのサインインとログアウトは、デスクトップアプリケーション[と[Webブラウザー](#sign-out)のどちらを使用しているかによって異なります。](#sign-in-dmc-app)

サインイン方法に関係なく、Dynamic Mediaクラシックを使用する前に、次の設定を確認してください。

* **ユーザー**
名電子メールアドレスをログイン名として使用します。

* **パ**
スワード一時パスワードは、Dynamic Mediaクラシックからのご案内の電子メールまたはDynamic Mediaクラシック管理者から取得します。初回のサインイン時に、この一時パスワードを変更するよう求められます。

## デスクトップアプリを使用してDynamic Mediaクラシックにサインインする{#sign-in-dmc-app}

1. AdobeDynamic Mediaクラシックデスクトップアプリケーションを開きます。

   ![Dynamic Mediaクラシックサインイン](/help/assets/dmclassic-login1.png)

1. 「**[!UICONTROL ユーザー名]**」フィールドに、電子メールアドレスを入力します。
1. 「**[!UICONTROL パスワード]**」フィールドにパスワードを入力します。
1. **[!UICONTROL Server]**ドロップダウンリストで、サーバーを選択します。
次のマッピングを使用して、使用する実稼働環境を選択します。

   | ブラウザーURL | デスクトップアプリサーバー名 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北米）プロダクション |
   | https://s7sps3.scene7.com/ | EMEA（ヨーロッパ、中東、アフリカ）プロダクション |
   | https://s7sps5.scene7.com/ | APAC（アジア太平洋）生産 |

1. 「**[!UICONTROL サインイン]**」をタップします。

### デスクトップアプリを使用してDynamic Mediaからサインアウト{#sign-out-dmc-app}

1. Dynamic Mediaクラシックデスクトップアプリケーションの右上隅にある「**[!UICONTROL サインアウト]**」をタップし、「**[!UICONTROL サインアウト]**」を再度タップします。

## Webブラウザーを使用してDynamic Mediaクラシックにサインインする{#signing-in-and-out}

WebブラウザーでDynamic Mediaクラシックを使用する前に、ユーザー名とパスワードに加えて、次の点も確認してください。

* ****
セットアップ管理者がDynamic Mediaクラシックを使用するように設定している必要があります。

* ****
URLY ClassicにアクセスするURLの場所を持っている必要があります。このURLは、 
*ご* 案内の電子メールまたはDynamic Mediaクラシック管理者から送信した電子メール。

Dynamic MediaクラシックはWebベースなので、別のWebサイトに移動するとシステムが終了します。 例えば、ブラウザーウィンドウの戻るボタンをクリックすると、Dynamic Mediaクラシックは終了します。

1. Web ブラウザを起動します。
1. （ご案内の電子メールから）Dynamic MediaクラシックログインURLに移動します。 または、Dynamic MediaクラシックWebサイト([www.adobe.com/products/scene7.html](https://www.adobe.com/products/scene7.html))で「お客様ログイン」ボタンを選択してサインインすることもできます。
1. 「**[!UICONTROL ユーザー名]**」テキストフィールドに、電子メールアドレスを入力します。
1. 「**[!UICONTROL パスワード]**」テキストフィールドに、パスワードを入力します。
1. 必要に応じて、「**[!UICONTROL ユーザー名を記憶]**」オプションを選択して、電子メールアドレスをコンピュータに記憶させることができます。
1. 「**[!UICONTROL サインイン]**」をタップします。

### Webブラウザーを介してDynamic Mediaからサインアウト{#sign-out}

1. 次のいずれかの操作を行います。

   * グローバルナビゲーションバーの右側で、「**[!UICONTROL サインアウト]**」をタップします。
   * ブラウザの終了

>[!MORELIKETHIS]
>
>* [個人設定](personal-setup.md#personal_setup)

