---
title: 管理設定
seo-title: 管理設定
description: 'null'
seo-description: Dynamic Media Classicの管理領域を設定する方法について説明します。
uuid: 16ba9fed-b5c6-4991-83b3-8d7d7129013a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 3c9ee4ec-dd37-498d-98d6-1339b80177ff
translation-type: tm+mt
source-git-commit: 1ee586fab6a4e10a946848fd079438ade38490d9
workflow-type: tm+mt
source-wordcount: '1945'
ht-degree: 64%

---


<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理設定{#administration-setup}

管理設定画面は、Dynamic Media Classicユーザの管理に使用します。 これらの画面は、ユーザーがDynamic Media Classicで作業できるようにしたり、電子メールでユーザーとやり取りできるようにする場合に使用します。

1. To access Administration Setup options, click **Setup** > **Personal Setup** > **Administration Setup**.

## ユーザ管理 {#user-administration}

すべてのDynamic Media Classicユーザーに、Dynamic Media Classicの機能に対する権限およびアクセス権を決定する役割が割り当てられます。 管理者が、割り当てられている会社に対する各ユーザの役割や責任を決定します。

通常、Dynamic Media Classicでは、最初の一連の会社が設定され、会社管理者が割り当てられます。 次に、会社管理者がDynamic Media Classicユーザーを設定および管理します。

Dynamic Media Classicは、複数のユーザーの役割をサポートしています。 これらのロールは、Dynamic Media Classic用に設定された会社にアクセスできます。

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobeダイナミックメディアクラシックユーザ** は、割り当てられた会社にアクセスできます。管理作業を実行できません。

**Adobeのダイナミックメディアクラシック会社管理者** ：自分の会社のみを表示および管理できます。 また、管理者やユーザの追加といったすべての管理機能を実行できます。会社管理者は、DMC会社管理者アカウントにユーザを追加できます。 （この役割は、初期設定のユーザの役割です）。

ユーザーを追加すると、追加を通知する電子メールメッセージがDynamic Media Classicからユーザーに送信されます。 メッセージには、パスワードとダイナミックメディアクラシックURLが含まれます。

### ユーザまたは管理者の追加 {#adding-a-user-or-administrator}

1. 設定／アプリケーション設定／管理設定／ユーザ管理をクリックします。
1. 「追加」をクリックします。
1. 追加するユーザまたは管理者の名前と電子メールアドレスを入力し、「次へ」をクリックします。

   >[!NOTE]
   >
   >電子メールアドレスにアポストロフィ（&#39;）は使用できません。

1. 「役割」オプションを選択して、役割をユーザに割り当てます。

   詳しくは、 [Dynamic Media Classicユーザーの役割と権限を参照してください](administration-setup.md#user_administration)。

1. ユーザを追加する会社の名前を選択します。
1. ユーザをグループに追加する場合（Media Portal ユーザまたは寄稿者を追加している場合）、「次へ」をクリックしてユーザを追加します。
1. 「保存」をクリックして、ユーザ設定を終了します。

   保存後、ユーザを別の会社に追加するかどうかを確認するメッセージが表示されます。ユーザを会社に追加する場合は、「追加」をクリックします。

   すべての新規ユーザーに、ランダムに生成されたパスワードが与えられます。ユーザーは、初めてDynamic Media Classicにログインしたときにパスワードを変更する必要があります。

   新規ユーザを追加した後、新規ユーザにご案内の電子メールが送信されます。この電子メールには、一時パスワードと、Scene7 Publishing System へのログオン方法が記載されています。

   ご案内の電子メールを受信しない場合は、Dynamic Media Classicのログインページ(https://s7sps1.scene7.com)に移動し、「パスワードを忘れた場合」をクリックするようにユーザーに指示します。 パスワードがリセットされ、新しい電子メールが送信されます。ユーザが電子メールを受信せず、迷惑メールフォルダにもない場合は、テクニカルサポートに問い合わせてください。

   新規 Media Portal ユーザを追加する場合は、設定／アプリケーション設定／ユーザ管理に進んで、「ユーザリストをアップロード」をクリックして、含まれているユーザの数が 500 ユーザ以下の .csv ファイルを選択することもできます。

### ユーザの削除 {#deleting-a-user}

ユーザーをDynamic Media Classicから削除するには、ユーザーを無効にします。 無効なユーザは、システムとすべてのアカウントから削除されます。

1. **設定**／**アプリケーション設定**／**管理設定**／**ユーザ管理**&#x200B;をクリックします。
1. リストからユーザを選択し、**「編集」**&#x200B;をクリックします。
1. 「有効」の選択を解除します。
1. **「保存」**&#x200B;をクリックします。

### ユーザのアクティブ化または非アクティブ化 {#activating-or-deactivating-users}

ユーザを非アクティブにすると、アクセスするアカウントを選択メニューの一番上に表示されるアカウントにアクセスする権限がなくなります。

1. **設定**／**アプリケーション設定**／**管理設定**／**ユーザ管理**&#x200B;をクリックします。
1. ユーザリストで、ユーザ名の横に表示される「アクティブ」オプションを選択または選択解除します。

### ユーザ情報の編集 {#editing-user-information}

編集できるユーザ情報は、管理者としての役割、および情報編集先であるユーザに対して割り当てられた役割によって異なります。グレー表示（使用できない）オプションは、編集できません。

1. **設定**／**アプリケーション設定**／**管理設定**／**ユーザ管理**&#x200B;に移動します。
1. ユーザを選択して、**「編集」**&#x200B;を選択します。
1. 権限またはアクセスを変更する会社が表示されているテーブルのエントリを選択し、「会社の管理」リンクをクリックします。
1. ユーザの役割を選択します。
1. ユーザのグループメンバーシップを変更する場合（Media Portal ユーザまたは寄稿者を編集または追加している場合）、「次へ」をクリックしてグループメンバーシップを編集します。
1. **「保存」**&#x200B;をクリックします。

### ユーザリストのフィルタリングと並べ替え {#filtering-and-sorting-the-user-list}

ユーザリストのフィルタリングや並べ替えを行ってユーザを探すことができます。ユーザリストには、アクセスするアカウントを選択メニューで選択されているアカウントに関係なく、管理下のすべてのアカウント内のすべてのユーザが表示されます。

次のユーザリストフィルタリング方法を使用できます。

**グループでフィルタリング** ：グループでフィルタリングメニューを選択し、グループ内のユーザーにリストを絞り込むオプションを選択します。

**ユーザーの役割でフィルタリング** ：ユーザーの役割でフィルタリングメニューを選択し、異なる種類のユーザーまたは管理者にリストを絞り込むオプションを選択します。

**フィールド名でフィルタする** [フィールドでフィルタを適用する]オプションを選択します。 次に、「フィールド名が」メニューを選択して、リストをフィルタリングする列を選択し、フィルタリングする文字メニューを選択して文字を選択します。いずれかの列で、選択した文字によってリストがフィルタリングされます。リスト全体を表示するには、「フィールドによるフィルタを有効にする」オプションを選択解除します。

**無効なユーザを除外する「無効なユーザを含める** 」オプションの選択を解除します。 検索結果には、システム内のユーザだけが表示されます。無効なユーザはシステムおよび管理下のアカウントから削除されています。

**列見出しで並べ替え** ：見出しをクリックすると、すべてのユーザーを、ステータス、名、姓、電子メールのアルファベット順、ユーザーの役割、有効/無効なステータスで並べ替えることができます。

ユーザ数が多い場合は、最大リストサイズメニューを選択し、数値を選択することで、リストのサイズを制限できます。

<!-- CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to a Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

You can link an Adobe IMS user identity to a Dynamic Media Classic IPS user account so you can use SSO (Single Sign On) to log on and launch Scene7 Publishing System from within Adobe Marketing Cloud.

1. Adobe should already have setup your account with an Adobe Marketing Cloud organization and linked it to your Scene7 Publishing System product context. If this setup is not yet done or you are unsure if it has been done, contact Adobe Customer Care.

   When the setup is complete, you can can log on to Adobe Marketing Cloud and link your Adobe Marketing Cloud identity to your Dynamic Media Classic user account by doing the following.

1. In Adobe Marketing Cloud, navigate to your account settings.
1. Click **Manage Organizations**.
1. Click **Link Account** or **Get Access**.
1. Select **Experience Manager**, and then type your credentials.

   Your credentials include your IPS company region, email address, and password.

1. Click **Link**.
1. When the link is set, you can launch Scene7 Publishing System from within Adobe Marketing Cloud, or you can launch it directly.

   Do one of the following:

    * To launch Dynamic Media Classic from within Adobe Marketing Cloud, in the left rail of Adobe Marketing Cloud, click **Solutions** &gt; **Experience Manager**. Under the Dynamic Media Classic card, click **Launch**.
    * To log on to Scene7 Publishing System directly using your IMS credentials, use the following website:

      https://s7spsN.scene7.com/IpsWeb?ims=1

      Replace “N” in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 帯域幅とストレージ {#bandwidth-storage}

Dynamic Media Classic管理者は、管理している会社に対して、帯域幅、ストレージおよびその他のタイプのレポートを生成できます。 これらのレポートは、帯域幅とストレージ画面で表示できます。

この画面を開くには、設定／個人設定をクリックします。管理設定を展開し、「帯域幅とストレージ」をクリックします。

### レポートのタイプ {#types-of-reports}

次の表で、帯域幅とストレージ画面から生成できるレポートについて説明します。

| レポート | 情報 | 使用方法 |
|:--- |:--- |:--- |
| 帯域幅 | 帯域幅使用量（会社別） | 特定の日付範囲にわたる帯域幅使用量を会社別に追跡して、トラフィックパターンを判断します。 |
| ストレージ | ストレージ使用量 | アップロードされたデータの量を会社別に追跡します。 |
| 画像コンテンツ | 画像要求数（タイプ別） | 様々な画像タイプの要求数と使用量を追跡します。 |
| ドメイン | URL 要求数（ドメイン別） | 特定の会社の画像要求のドメインに基づいて画像の使用量を追跡します(Dynamic Media Classicでは、アカウントごとに複数のドメインを提供できます。 詳しくは、テクニカルサポートにお問い合わせください）。 |
| ビデオストリーミング | ストリーミングビデオの帯域幅使用量 | 特定の日付範囲にわたるストリーミングビデオ使用量を会社別に追跡して、トラフィックパターンを判断します。 |
| ビデオコンテンツ | 様々なビデオの再生時間 | 最も視聴回数の多かったビデオと最も視聴回数が少なかったビデオを判断します。 |


画像コンテンツレポートは、以下の画像タイプの要求に関する情報を提供します。

**画像要求** ：画像の要求です。

**サムネール要求** ：ビューア内のスウォッチまたは代替画像の要求です。

**マスク要求** ：グレースケールマスクを返す画像に対する要求です。

**ビューアタイル要求** ：ビューアによって読み込まれた画像要求です。

**Vntオブジェクト要求** ：要求されたビネット内の指定されたオブジェクトを含む画像を返す画像レンダリング要求です。

**Vnt情報要求** ：要求されたビネットに関する情報を返す画像レンダリング要求です。

>[!NOTE]
>
>ビデオストリーミングレポートは、ストリーミングビデオにのみ該当します。プログレッシブビデオの視聴は追跡しません。

### レポートの生成 {#generating-a-report}

帯域幅、ストレージ、画像コンテンツ、ドメイン、ビデオストリーミングまたはビデオコンテンツのレポートを生成するには：

1. 設定／個人設定を選択します。
1. 管理設定を展開し、「帯域幅とストレージ」をクリックします。
1. 「帯域幅」、「ストレージ」、「画像コンテンツ」、「ドメイン」、「ビデオストリーミング」または「ビデオコンテンツ」タブをクリックします。

   [レポートのタイプ](administration-setup.md#types_of_reports)を参照してください。

### 様々な方法でのデータの表示 {#viewing-data-in-different-ways}

帯域幅とストレージページでレポートを生成した後に、情報を表示するためのオプションを選択できます。情報の種類、情報の表示方法（グラフまたはデータグリッド）および情報の収集期間を指定できます。データビューで、情報を並べ替えたり、列の順番を変更することができます。

**グラフまたはデータ・グリッドでのデータの表示** 「グラフ・表示」オプションをクリックすると、グラフ内の表示・データが表示されます。データグリッド内のデータを表示するには、「データ表示」オプションをクリックします。

**レポート表示タイプの選択** [レポートタイプ]メニューで[概要]、[日別]、または[月別]を選択し、データを概要形式、日別、または月別に整理します。 一部のレポートには、このオプションはありません。

**期間の指定** ：オプションを選択してレポートの期間を定義し、「更新」をクリックします。

**定義済みの期間** ：定義済みレポートメニューで、オプションを選択します。 例えば、先月からのデータを収集するには、「先月」を選択します。

**カスタム期間** ：事前定義済みレポートメニューで「カスタム」を選択します。 開始月または開始日メニューで月または日を選択して、月数または日数メニューで値を選択します。ドメインレポートおよびビデオコンテンツレポートでは、レポート情報を収集するための特定の開始日と終了日を選択できます。

**データの並べ替え(データ表示のみ)** 列の情報を並べ替えるには、列の見出しをクリックします。 もう一度クリックすると、降順で並べ替えられます。

**列の並べ替え(データ表示のみ)** ：列をデータグリッド上の別の位置に移動するには、見出しをドラッグします。

### レポートの書き出しと印刷 {#exporting-and-printing-reports}

レポートの生成後に、スプレッドシートやその他のアプリケーションで使用できるようにデータを書き出すことができます。また、レポートを印刷することもできます。

**レポートデータのエクスポート** ：データ表示で、必要に応じてデータを並べ替えたり、配置したりします。 書き出しメニューを開いて、「タブ区切り」、「カンマ区切り」または「HTML フォーマット済み」の形式を選択します。選択した形式でデータがクリップボードにコピーされます。これでデータをスプレッドシートやアプリケーションにペーストできます。

**レポートを印刷する** [印刷]をクリックし、印刷ダイアログボックスで必要なオプションを選択して、[OK]をクリックします。

## 画像エラー {#image-errors}

ダイナミックMedia Classic管理者は、画像エラーレポートを生成できます。 画像エラーレポートは、現在ログインしている会社について、直近 24 時間以内で最も頻度の高い画像エラー 20 個をリストで表示します。画像エラーレポートを生成するには、次の手順に従います。

1. 設定／個人設定をクリックします。
1. 管理設定を展開し、「画像エラー」をクリックします。
1. 必要に応じて次の操作を行います。

   * 見出しをクリックして、見出し情報ごとにエラーを並べ替えます。初期設定では、エラーは発生頻度の高い順に並んでいます。
   * カーソルをエラーの「応答」フィールド上に移動すると、詳細なエラーメッセージが表示されます。
   * カーソルを「URL」フィールドまたは「リファラ」フィールド上に移動すると、画像またはリファラ Web ページへのリンクが表示されます。
   * URL の「URL をコピー」をクリックして、実際の画像へのリンクをコピーします。このリンクをブラウザウィンドウにペーストして画像のページに移動し、エラーを調べることができます。
   * リファラの「URL をコピー」をクリックして、リファラ Web ページへのリンクをコピーします。

表示されたエラーは、現在ログインしている会社のエラーです。各エラーには次の情報が含まれます。

**問題のある画像の画像ID** 。

**Time** ：最初にエラーが報告された時間と、最後にエラーが報告された時間との間の、過去24時間内の時間範囲です。

**[カウント** ]イメージで報告されたエラーの数です。

**応答** ：具体的なエラーメッセージです。 エラーは 4xx または 5xx です。

**URLは** 、Scene7上の画像のURLをリストします。

**転送者** ：最初の要求元のWebサイトのURLを指定します。 リファラには、画像へのリンクがある Web サイトが表示されます。

「URL」列および「リファラ」列には、テストを簡略化するための「URL をコピー」が関連付けられています。
