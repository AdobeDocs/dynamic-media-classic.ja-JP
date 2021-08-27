---
title: 管理の設定
description: Dynamic Media Classicの管理領域を設定する方法について説明します。
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
source-git-commit: 44045daa35052f01a26c67e0b2a0fb1405c53292
workflow-type: tm+mt
source-wordcount: '1965'
ht-degree: 36%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理設定{#administration-setup}

管理設定画面は、AdobeDynamic Media Classicユーザーを管理するためのものです。 これらの画面を使用して、ユーザーがDynamic Media Classicで作業したり、Adobeと電子メールでコミュニケーションしたりできます。

1. 管理設定のオプションにアクセスするには、**設定** > **個人設定** > **管理設定**&#x200B;に移動します。

## ユーザ管理 {#user-administration}

すべてのAdobeDynamic Media Classicユーザーに、AdobeDynamic Media Classicの機能に対する権限とアクセス権を決定する役割が割り当てられます。 管理者が、割り当てられている会社に対する各ユーザの役割や責任を決定します。

通常、AdobeDynamic Media Classicは最初の会社セットを設定し、会社の管理者を割り当てます。 その後、会社の管理者がDynamic Media ClassicユーザーのAdobeを設定および管理します。

AdobeDynamic Media Classicは、複数のユーザーの役割をサポートしています。 これらの役割は、Dynamic Media ClassicのAdobeを設定した会社にアクセスできます。

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**AdobeDynamic Media Classicユ** ーザーは、割り当てられた会社にアクセスできます。管理作業を実行できません。

**AdobeDynamic Media Classicカンパニー** 管理者は、自分の会社のみを表示および管理できます。また、管理者やユーザの追加といったすべての管理機能を実行できます。会社管理者は、DMC会社の管理者アカウントにユーザーを追加できます。 （この役割は、初期設定のユーザの役割です）。

ユーザーを追加すると、AdobeDynamic Media Classicはユーザーに「ようこそ」の電子メールメッセージを送信します。 このメッセージには、パスワードとAdobeDynamic Media Classic URLが含まれます。

### ユーザーまたは管理者の追加 {#adding-a-user-or-administrator}

1. **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL ユーザー管理]**&#x200B;に移動します。
1. 「**[!UICONTROL 追加]**」を選択します。
1. 追加するユーザーまたは管理者の名前と電子メールアドレスを入力し、「**[!UICONTROL 次へ]**」を選択します。

   >[!NOTE]
   >
   >電子メールアドレスでは、アポストロフィ文字(`‘`)は使用できません。

1. ユーザーにロールを割り当てるには、「ロール」オプションを選択します。

   [Dynamic Media Classicユーザーの役割と権限のAdobe](administration-setup.md#user_administration)を参照してください。

1. ユーザーを会社に追加するには、会社名を選択します。
1. ユーザーをグループに追加する場合（Media Portalユーザーまたはコントリビューターを追加する場合）、「**[!UICONTROL 次へ]**」を選択して、ユーザーを追加します。
1. 「**[!UICONTROL 保存]**」を選択して、ユーザー設定を完了します。

   保存後、ユーザを別の会社に追加するかどうかを確認するメッセージが表示されます。ユーザーを会社に追加する場合は、「**[!UICONTROL 追加]**」を選択します。

   すべての新規ユーザーに、ランダムに生成されたパスワードが与えられます。ユーザーは、Dynamic Media Classicデスクトップアプリケーションで初めてログインする際に、Adobeを変更する必要があります。

   新規ユーザを追加した後、新規ユーザにご案内の電子メールが送信されます。この電子メールは、一時的なパスワードを提供し、Dynamic Media Classicにログインする方法を説明します。

   ユーザーに「ようこそ」の電子メールが届かない場合は、Dynamic Media ClassicのAdobeログインページ(https://s7sps1.scene7.com)に移動し、「**[!UICONTROL パスワードを忘れた場合]**」を選択します。 パスワードがリセットされ、新しい電子メールが送信されます。ユーザが電子メールを受信せず、迷惑メールフォルダにもない場合は、テクニカルサポートに問い合わせてください。

   新しいMedia Portalユーザーを追加する場合は、**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL ユーザー管理]**&#x200B;に移動し、「**[!UICONTROL ユーザーリストをアップロード]**」を選択して、500人以下のユーザーを含む.csvファイルを選択します。

### ユーザの削除 {#deleting-a-user}

ユーザーを無効にすることで、AdobeDynamic Media Classicからユーザーを削除できます。 無効なユーザは、システムとすべてのアカウントから削除されます。

1. **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL ユーザー管理]**&#x200B;に移動します。
1. リストからユーザーを選択し、「**[!UICONTROL 編集]**」を選択します。
1. 「有効」の選択を解除します。
1. 「**[!UICONTROL 保存]**」を選択します。

### ユーザーのアクティベートまたはアクティベート解除 {#activating-or-deactivating-users}

ユーザを非アクティブにすると、アクセスするアカウントを選択メニューの一番上に表示されるアカウントにアクセスする権限がなくなります。

1. **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL ユーザー管理]**&#x200B;に移動します。
1. ユーザーリストで、ユーザー名の横にある「**[!UICONTROL アクティブ]**」オプションを選択または選択解除します。

### ユーザ情報の編集 {#editing-user-information}

編集できるユーザ情報は、管理者としての役割、および情報編集先であるユーザに対して割り当てられた役割によって異なります。グレー表示（使用できない）オプションは、編集できません。

1. **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL ユーザー管理]**&#x200B;に移動します。
1. リストからユーザーを選択し、「**[!UICONTROL 編集]**」を選択します。
1. 権限またはアクセスを変更する会社を表示するテーブル内のエントリを選択し、「**[!UICONTROL 会社の管理]**」を選択します。
1. ユーザの役割を選択します。
1. ユーザーのグループメンバーシップを変更する場合（Media Portalユーザーまたはコントリビューターを編集または追加する場合）、「**[!UICONTROL 次へ]**」を選択し、グループメンバーシップを編集します。
1. 「**[!UICONTROL 保存]**」を選択します。

### ユーザリストのフィルタリングと並べ替え {#filtering-and-sorting-the-user-list}

ユーザリストのフィルタリングや並べ替えを行ってユーザを探すことができます。ユーザリストには、アクセスするアカウントを選択メニューで選択されているアカウントに関係なく、管理下のすべてのアカウント内のすべてのユーザが表示されます。

次のユーザリストフィルタリング方法を使用できます。

* **グループでフィルター**  — グループで **[!UICONTROL フ]** ィルターメニューを選択し、リストをグループ内のユーザーに絞り込むオプションを選択します。

* **ユーザーの役割でフィルター**  - 「ユーザー **[!UICONTROL の役割でフ]** ィルター」メニューを選択し、様々なタイプのユーザーまたは管理者にリストを絞り込むオプションを選択します。

* **フィールド名でフィルター**  - 「フィールドでフ **[!UICONTROL ィルター」を選択します]**。次に、「**[!UICONTROL フィールド名別]**」メニューを選択し、リストのフィルタリングに使用する列を選択し、フィルター文字メニューを選択して文字を選択します。 いずれかの列で、選択した文字によってリストがフィルタリングされます。完全なリストを表示するには、「**[!UICONTROL フィールドでフィルター]**」オプションの選択を解除します。

* **無効なユーザーを除外**  - 「無効なユーザーを含め **[!UICONTROL る」の選択を解除します]**。検索結果には、システム内のユーザだけが表示されます。無効なユーザはシステムおよび管理下のアカウントから削除されています。

* **列見出しで並べ替え**  — すべてのユーザーをステータス、名、姓、電子メールのアルファベット順、ユーザーの役割別、有効/無効なステータスで並べ替える見出しを選択します。

ユーザ数が多い場合は、最大リストサイズメニューを選択し、数値を選択することで、リストのサイズを制限できます。

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to an Adobe Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Adobe Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Select **Manage Organizations**.
1. Select **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Select **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Adobe Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, select **Solutions** > **Experience Manager**. Under the Adobe Dynamic Media Classic card, select **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 帯域幅とストレージ {#bandwidth-storage}

AdobeDynamic Media Classic管理者は、管理する会社の帯域幅、ストレージ、その他のタイプのレポートを生成できます。 これらのレポートは、帯域幅とストレージページで利用できます。

このページを開くには、**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**&#x200B;に移動します。 「**[!UICONTROL 管理設定]**」を展開し、「**[!UICONTROL 帯域幅とストレージ]**」を選択します。

### レポートのタイプ {#types-of-reports}

次の表に、帯域幅とストレージページから生成できるレポートを示します。

| レポート | 情報 | 使用方法 |
|:--- |:--- |:--- |
| 帯域幅 | 帯域幅使用量（会社別） | 特定の日付範囲にわたる帯域幅使用量を会社別に追跡して、トラフィックパターンを判断します。 |
| ストレージ | ストレージ使用量 | アップロードされたデータの量を会社別に追跡します。 |
| 画像コンテンツ | 画像要求数（タイプ別） | 様々な画像タイプの要求数と使用量を追跡します。 |
| ドメイン | URL 要求数（ドメイン別） | 特定の会社の画像要求のドメインに基づいて画像の使用量を追跡します(AdobeDynamic Media Classicは、アカウントごとに複数のドメインを提供できます。 詳しくは、テクニカルサポートにお問い合わせください）。 |
| ビデオストリーミング | ストリーミングビデオの帯域幅使用量 | 特定の日付範囲にわたるストリーミングビデオ使用量を会社別に追跡して、トラフィックパターンを判断します。 |
| ビデオコンテンツ | 様々なビデオの再生時間 | 最も視聴回数の多かったビデオと最も視聴回数が少なかったビデオを判断します。 |

画像コンテンツレポートは、以下の画像タイプの要求に関する情報を提供します。

* **イメージリクエスト**  — イメージのリクエスト。

* **サムネールの要求**  — ビューア内のスウォッチまたは代替画像の要求。

* **マスクリクエスト**  — 画像に対するリクエストで、グレースケールのマスクが返されます。

* **ビューアタイルの要求**  — ビューアによって読み込まれた画像要求。

* **Vnt Object Request**  — 要求されたビネット内の指定されたオブジェクトを含む画像を返す画像レンダリングリクエスト。

* **Vnt Info Request**  — 要求されたビネットに関する情報を返す画像レンダリングリクエスト。

>[!NOTE]
>
>ビデオストリーミングレポートは、ストリーミングビデオにのみ該当します。プログレッシブビデオの視聴は追跡しません。

### レポートの生成 {#generating-a-report}

帯域幅、ストレージ、画像コンテンツ、ドメイン、ビデオストリーミングまたはビデオコンテンツのレポートを生成するには：

1. **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**&#x200B;に移動します。
1. [管理設定]を展開し、[**[!UICONTROL 帯域幅とストレージ]**]を選択します。
1. タブを選択：**[!UICONTROL 帯域幅]**、**[!UICONTROL ストレージ]**、**[!UICONTROL 画像コンテンツ]**、**[!UICONTROL ドメイン]**、**[!UICONTROL ビデオストリーミング]**、または&#x200B;**[!UICONTROL ビデオコンテンツ]**。

   [レポートのタイプ](administration-setup.md#types_of_reports)を参照してください。

### 様々な方法でのデータの表示 {#viewing-data-in-different-ways}

帯域幅とストレージページでレポートを生成した後に、情報を表示するためのオプションを選択できます。情報の種類、情報の表示方法（グラフまたはデータグリッド）および情報の収集期間を指定できます。データビューで、情報を並べ替えたり、列の順番を変更することができます。

* **グラフまたはデータ・グリッドでのデータの表示**  - 「グラフ表示」を選択 **[!UICONTROL し]** て、グラフにデータを表示します。データグ **[!UICONTROL リッ]** ドでデータを表示するには、「データ表示」を選択します。

* **レポートの表示タイプを選択します**  — レポートタイプメニューで、「 **[!UICONTROL 概要]**」、「 **[!UICONTROL 毎日]**」または「月」を選択し **** て、データを要約形式、日別、月別に整理します。一部のレポートには、このオプションはありません。

* **期間の指定**  — オプションを選択してレポートの期間を定義し、「期間を定義した後に更 **** 新」を選択します。

* **事前定義済み期間**  — 事前定義済みレポートメニューで、オプションを選択します。例えば、先月からのデータを収集するには、「先月」を選択します。

* **カスタム期間**  — 事前定義済みのレポートメニューで、「カスタム」を **[!UICONTROL 選択します]**。次に、「**[!UICONTROL 開始月]**」（または&#x200B;**[!UICONTROL 開始日]**）メニューで日付を選択し、「月数」（または「#」または「日数」）メニューで日付を選択します。 ドメインレポートおよびビデオコンテンツレポートでは、レポート情報を収集するための特定の開始日と終了日を選択できます。

* **データを並べ替え（データビューのみ）**  — 列の情報を並べ替えるには、列の見出しを選択します。降順に並べ替えるには、もう一度「 」を選択します。

* **列の並べ替え（データビューのみ）**  — 列をデータグリッド上の別の場所に移動するには、見出しをドラッグします。

### レポートの書き出しと印刷 {#exporting-and-printing-reports}

レポートの生成後に、スプレッドシートやその他のアプリケーションで使用できるようにデータを書き出すことができます。また、レポートを印刷することもできます。

* **レポートデータのエクスポート**  — データビューで、必要に応じてデータを並べ替え、並べ替えます。次に、**[!UICONTROL エクスポート]**&#x200B;メニューを開き、次の形式を選択します。**[!UICONTROL タブ区切り]**、**[!UICONTROL コンマ区切り]**、または&#x200B;**[!UICONTROL HTML形式]**。 選択した形式でデータがクリップボードにコピーされます。これでデータをスプレッドシートやアプリケーションにペーストできます。

* **レポートの印刷**  - 「印刷」を選択 **[!UICONTROL し、印刷ダイアログボックスで必要なオプションを選択して、「]** OK ****」を選択します。

## 画像エラー {#image-errors}

AdobeDynamic Media Classic管理者は、画像エラーレポートを生成できます。 画像エラーレポートは、現在ログインしている会社について、直近 24 時間以内で最も頻度の高い画像エラー 20 個をリストで表示します。画像エラーレポートを生成するには、次の手順を実行します。

1. **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**&#x200B;に移動します。
1. [管理設定]を展開し、[**[!UICONTROL イメージエラー]**]を選択します。
1. 必要に応じて次の操作を行います。

   * 見出し情報別にエラーを並べ替えるには、見出しを選択します。 初期設定では、エラーは発生頻度の高い順に並んでいます。
   * カーソルをエラーの「応答」フィールド上に移動すると、詳細なエラーメッセージが表示されます。
   * 画像またはリファラーWebページへのリンクを確認するには、URLフィールドまたはリファラーフィールドの上にカーソルを移動します。
   * リンクを実際の画像にコピーするには、「**[!UICONTROL URLコピーURL]**」を選択します。 このリンクをブラウザウィンドウにペーストして画像のページに移動し、エラーを調べることができます。
   * リファラーWebページへのリンクをコピーするには、「**[!UICONTROL リファラーコピーURL]**」を選択します。

表示されたエラーは、現在ログインしている会社のエラーです。各エラーには次の情報が含まれます。

* **画像ID**  — 問題のある画像のID。

* **時間**  — 直近24時間以内に、エラーが最初にレポートされた時間から最後にレポートされた時間までの時間範囲。

* **カウント**  — 画像で報告されたエラーの数。

* **応答**  — 特定のエラーメッセージ。エラーは 4xx または 5xx です。

* **URL**  -AdobeDynamic Media Classic上の画像のURLをリストします。

* **リファラー**  — 最初のリクエストの送信元のWebサイトのURLを指定します。リファラには、画像へのリンクがある Web サイトが表示されます。

「URL」列および「リファラ」列には、テストを簡略化するための「URL をコピー」が関連付けられています。
