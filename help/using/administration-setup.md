---
title: 管理設定
description: Adobe Dynamic Media Classicの管理領域の設定方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1974'
ht-degree: 32%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理設定{#administration-setup}

管理設定画面は、Adobe Dynamic Media Classic ユーザーを管理するためのものです。 これらの画面を使用すると、ユーザーはAdobe Dynamic Media Classicで作業したり、他のユーザーと電子メールで通信したりできます。

1. 管理設定オプションにアクセスするには、**設定**/**個人設定**/**管理設定** に移動します。

## ユーザ管理 {#user-administration}

すべてのAdobe Dynamic Media Classic ユーザーには、Adobe Dynamic Media Classicの機能への権限とアクセス権を決定する役割が割り当てられます。 管理者が、割り当てられている会社に対する各ユーザの役割や責任を決定します。

通常、Adobe Dynamic Media Classicは最初の会社セットを設定し、会社管理者を割り当てます。 次に、会社管理者は、Adobe Dynamic Media Classic ユーザーを設定および管理します。

Adobe Dynamic Media Classicは、複数のユーザーの役割をサポートしています。 これらの役割は、Adobe Dynamic Media Classic用に設定された会社にアクセスできます。

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic ユーザー** 割り当てられている会社にアクセスできます。管理上の義務を負うことはできません。

**Adobe Dynamic Media Classic会社管理者** 自分の会社のみを表示および管理できます。 また、管理者やユーザの追加といったすべての管理機能を実行できます。会社管理者は、DMC の会社管理者アカウントにユーザーを追加できます。 （この役割は、初期設定のユーザの役割です）。

ユーザーを追加すると、Adobe Dynamic Media Classicからようこそメールがユーザーに送信されます。 このメッセージには、パスワードとAdobe Dynamic Media Classic URL が含まれています。

### ユーザーまたは管理者を追加 {#adding-a-user-or-administrator}

1. **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 管理設定]**/**[!UICONTROL ユーザー管理]** に移動します。
1. 「**[!UICONTROL 追加]**」を選択します。
1. 追加するユーザーまたは管理者の名前とメールアドレスを入力し、「**[!UICONTROL 次へ]**」を選択します。

   >[!NOTE]
   >
   >アポストロフィ文字（`'`）はメールアドレスでは使用できません。

1. ユーザーに役割を割り当てるには、「役割」オプションを選択します。

   詳しくは、[Adobe Dynamic Media Classicのユーザーの役割と権限 ](administration-setup.md#user_administration) を参照してください。

1. ユーザーを会社に追加するには、会社名を選択します。
1. ユーザーをグループに追加する場合（Media Portal ユーザーまたはコントリビューターを追加する場合）、「**[!UICONTROL 次へ]**」を選択し、ユーザーを追加します。
1. 「**[!UICONTROL 保存]**」を選択して、ユーザー設定を完了します。

   保存後、ユーザを別の会社に追加するかどうかを確認するメッセージが表示されます。ユーザーを会社に追加する場合は、「**[!UICONTROL 追加]**」を選択します。

   すべての新規ユーザーには、ランダムに生成されたパスワードが与えられます。ユーザーは、Adobe Dynamic Media Classic デスクトップアプリケーションに初めてログインしたときにパスワードを変更する必要があります。

   新規ユーザを追加した後、新規ユーザにご案内の電子メールが送信されます。このメールには、一時パスワードと、Adobe Dynamic Media Classicへのログイン方法が記載されています。

   お知らせメールが届かない場合は、Adobe Dynamic Media Classicのログインページ（https://s7sps1.scene7.com）で「**[!UICONTROL パスワードを忘れた場合]**」を選択します。 パスワードがリセットされ、新しい電子メールが送信されます。ユーザが電子メールを受信せず、迷惑メールフォルダにもない場合は、テクニカルサポートに問い合わせてください。

   新しい Media Portal ユーザーを追加する際は、**[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL ユーザー管理]** に移動して **[!UICONTROL ユーザーリストをアップロード]** を選択し、500 人以下のユーザーを含む.csv ファイルを選択することもできます。

### ユーザの削除 {#delet-a-user}

ユーザーを無効にすることで、Adobe Dynamic Media Classicから削除できます。 無効なユーザは、システムとすべてのアカウントから削除されます。

1. **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 管理設定]**/**[!UICONTROL ユーザー管理]** に移動します。
1. リストからユーザーを選択し、「**[!UICONTROL 編集]**」を選択します。
1. 「有効」の選択を解除します。
1. **[!UICONTROL 保存]** を選択します。

### ユーザーのアクティベートまたはアクティベート解除 {#activating-or-deactivating-users}

ユーザを非アクティブにすると、アクセスするアカウントを選択メニューの一番上に表示されるアカウントにアクセスする権限がなくなります。

1. **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 管理設定]**/**[!UICONTROL ユーザー管理]** に移動します。
1. ユーザーリストで、ユーザー名の横にある「**[!UICONTROL アクティブ]**」オプションを選択または選択解除します。

### ユーザ情報の編集 {#editing-user-information}

編集できるユーザ情報は、管理者としての役割、および情報編集先であるユーザに対して割り当てられた役割によって異なります。グレー表示（使用できない）オプションは、編集できません。

1. **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 管理設定]**/**[!UICONTROL ユーザー管理]** に移動します。
1. リストからユーザーを選択し、「**[!UICONTROL 編集]**」を選択します。
1. 権限またはアクセス権を変更しようとしている会社を示すテーブルのエントリを選択し、「**[!UICONTROL 会社を管理]**」を選択します。
1. ユーザの役割を選択します。
1. ユーザーのグループ メンバーシップを変更する場合（Media Portal ユーザーまたはコントリビューターを編集または追加する場合）、[**[!UICONTROL 次へ]**] を選択し、グループ メンバーシップを編集します。
1. **[!UICONTROL 保存]** を選択します。

### ユーザリストのフィルタリングと並べ替え {#filtering-and-sorting-the-user-list}

ユーザリストのフィルタリングや並べ替えを行ってユーザを探すことができます。ユーザリストには、アクセスするアカウントを選択メニューで選択されているアカウントに関係なく、管理下のすべてのアカウント内のすべてのユーザが表示されます。

次のユーザーリストフィルタリング手法を使用できます。

* **グループでフィルター**:「**[!UICONTROL グループ別]**」メニューを選択し、グループのユーザーにリストを絞り込むオプションを選択します。

* **ユーザーロールでフィルター**:「**[!UICONTROL ユーザーロール別]**」メニューを選択し、リストを様々なタイプのユーザーまたは管理者に絞り込むオプションを選択します。

* **フィールド名でフィルター**:「**[!UICONTROL フィールドでフィルターを有効にする]** を選択します。 次に、「**[!UICONTROL フィールド名]** メニューを選択し、リストをフィルタリングする列を選択して、「文字をフィルター」メニューを選択し、レターを選択します。 リストは、選択したレターによって列の 1 つにフィルターされます。 完全なリストを表示するには、「**[!UICONTROL フィールドによるフィルターを有効にする]** オプションの選択を解除します。

* **無効なユーザーを除外**：選択を解除 **[!UICONTROL 無効を含める]**。 検索結果には、システム内のユーザだけが表示されます。無効なユーザーがシステムおよび管理するアカウントから削除されました。

* **列見出しで並べ替え**：すべてのユーザーをステータス（名、姓、メールのアルファベット順）で並べ替える見出しを選択します。 または、ユーザーの役割または有効/無効なステータスで並べ替えます。

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

      Replace "N" in the above path with the number for your IPS company region. That is, N = 1 for North America; 3 for EMEA; or 5 for JAPAC.
 -->

## 帯域幅とストレージ {#bandwidth-storage}

Adobe Dynamic Media Classic管理者は、管理対象の会社に対して、帯域幅、ストレージ、その他のタイプのレポートを作成できます。 これらのレポートは、「帯域幅とストレージ」ページで利用できます。

このページを開くには、**[!UICONTROL 設定]**/**[!UICONTROL 個人設定]** に移動します。 **[!UICONTROL 管理設定]** を展開し、**[!UICONTROL 帯域幅とストレージ]** を選択します。

### レポートのタイプ {#types-of-reports}

次の表に、「帯域幅とストレージ」ページから生成できるレポートを示します。

| レポート | 情報 | 使用方法 |
|:--- |:--- |:--- |
| 帯域幅 | 帯域幅使用量（会社別） | 特定の日付範囲にわたる帯域幅使用量を会社別に追跡して、トラフィックパターンを判断します。 |
| ストレージ | ストレージ使用量 | 会社がアップロードしたデータ量をトラッキングします。 |
| 画像コンテンツ | 画像要求数（タイプ別） | 様々な画像タイプの要求数と使用量を追跡します。 |
| ドメイン | URL 要求数（ドメイン別） | 特定の会社の画像要求のドメインに基づいて画像の使用量を追跡します（Adobe Dynamic Media Classicは、アカウントごとに複数のドメインを提供できます。 詳しくは、テクニカルサポートにお問い合わせください）。 |
| ビデオストリーミング | ストリーミングビデオの帯域幅使用量 | 特定の日付範囲にわたるストリーミングビデオ使用量を会社別に追跡して、トラフィックパターンを判断します。 |
| ビデオコンテンツ | 様々なビデオの再生時間 | 最も視聴回数の多かったビデオと最も視聴回数が少なかったビデオを判断します。 |

画像コンテンツレポートは、以下の画像タイプの要求に関する情報を提供します。

* **画像リクエスト**：画像のリクエスト。

* **サムネールリクエスト**：ビューアでのスウォッチまたは代替画像のリクエスト。

* **マスクリクエスト**：グレースケールのマスクを返す画像へのリクエスト。

* **ビューアタイルリクエスト**：ビューアによって読み込まれたイメージリクエスト。

* **VNT Object Request**：要求されたビネット内の指定されたオブジェクトを含む画像を返す画像レンダリングリクエスト。

* **VNT Info Request**：要求されたビネットに関する情報を返す画像レンダリングリクエスト。

>[!NOTE]
>
>ビデオストリーミングレポートは、ストリーミングビデオにのみ該当します。プログレッシブビデオの視聴は追跡されません。

### レポートの生成 {#generating-a-report}

帯域幅、ストレージ、画像コンテンツ、ドメイン、ビデオストリーミングまたはビデオコンテンツのレポートを生成するには：

1. **[!UICONTROL 設定]**/**[!UICONTROL 個人設定]** に移動します。
1. 「管理設定」を展開し、「**[!UICONTROL 帯域幅とストレージ]**」を選択します。
1. タブ（**[!UICONTROL 帯域幅]**、**[!UICONTROL ストレージ]**、**[!UICONTROL 画像コンテンツ]**、**[!UICONTROL ドメイン]**、**[!UICONTROL ビデオストリーミング]** または **[!UICONTROL ビデオコンテンツ]** を選択します。

   [レポートのタイプ](administration-setup.md#types_of_reports)を参照してください。

### 様々な方法でのデータの表示 {#viewing-data-in-different-ways}

帯域幅とストレージページでレポートを生成した後に、情報を表示するためのオプションを選択できます。情報の種類、情報の表示方法（グラフまたはデータグリッド）および情報の収集期間を指定できます。データビューで、情報を並べ替えたり、列の順番を変更することができます。

* **データをグラフまたはデータグリッドに表示**: **[!UICONTROL グラフ表示]** を選択するとグラフにデータが表示され、**[!UICONTROL データ表示]** を選択するとデータグリッドにデータが表示されます。

* **レポート表示タイプを選択**: レポートタイプ メニューで、**[!UICONTROL 概要]**、**[!UICONTROL 毎日]**、または **[!UICONTROL 毎月]** を選択して、データを概要形式、日別、または月別に整理します。 一部のレポートには、このオプションはありません。

* **期間の指定**: レポートの期間を定義するオプションを選択し、期間を定義した後で「**[!UICONTROL 更新]**」を選択します。

* **事前定義済みの期間**:「事前定義済みのレポート」メニューで、オプションを選択します。 例えば、先月からのデータを収集するには、「先月」を選択します。

* **カスタム期間**：事前定義済みレポート メニューで、「**[!UICONTROL カスタム]**」を選択します。 次に、**[!UICONTROL 開始月]** （または **[!UICONTROL 開始日]**） メニューの日付と月数（#または日） メニューの日付を選択します。 ドメインレポートおよびビデオコンテンツレポートでは、レポート情報を収集するための特定の開始日と終了日を選択できます。

* **データの並べ替え（データビューのみ）**：列内の情報を並べ替えます。 列の見出しを選択します。 降順で並べ替えるには、もう一度選択します。

* **列の並べ替え（データ表示のみ）**：列をデータグリッド上の別の場所に移動するには、列の見出しをドラッグします。

### レポートのエクスポートと印刷 {#exporting-and-printing-reports}

レポートの生成後に、スプレッドシートやその他のアプリケーションで使用できるようにデータを書き出すことができます。また、レポートを印刷することもできます。

* **レポートデータの書き出し**：データ表示では、必要に応じてデータを並べ替え、配置します。 次に、**[!UICONTROL 書き出し]** メニューを開き、**[!UICONTROL タブ区切り]**、**[!UICONTROL コンマ区切り]**、**[!UICONTROL HTML形式]** のいずれかの形式を選択します。 データは、選択した形式でクリップボードにコピーされます。 これでデータをスプレッドシートやアプリケーションにペーストできます。

* **レポートを印刷する**: **[!UICONTROL 印刷]** を選択し、[ 印刷 ] ダイアログ ボックスで必要なオプションを選択して、[**[!UICONTROL OK]**] を選択します。

## 画像エラー {#image-errors}

Adobe Dynamic Media Classic管理者は、画像エラーレポートを生成できます。 画像エラーレポートは、現在ログインしている会社について、直近 24 時間以内で最も頻度の高い画像エラー 20 個をリストで表示します。画像エラーレポートを生成するには、次の手順を実行します。

1. **[!UICONTROL 設定]**/**[!UICONTROL 個人設定]** に移動します。
1. [ 管理設定 ] を展開し、[**[!UICONTROL イメージ エラー]**] を選択します。
1. 必要に応じて次の操作を行います。

   * 見出し情報に基づいてエラーを並べ替えるには、見出しを選択します。 初期設定では、エラーは発生頻度の高い順に並んでいます。
   * カーソルをエラーの「応答」フィールド上に移動すると、詳細なエラーメッセージが表示されます。
   * 画像またはリファラー Web ページへのリンクを表示するには、「URL」フィールドまたは「リファラー」フィールドにカーソルを移動します。
   * 実際の画像へのリンクをコピーするには、「**[!UICONTROL URL コピー URL]**」を選択します。 このリンクをブラウザウィンドウにペーストして画像のページに移動し、エラーを調べることができます。
   * リファラー Web ページへのリンクをコピーするには、「**[!UICONTROL リファラーコピー URL]**」を選択します。

表示されるエラーは、現在ログインしている会社に関するものです。 各エラーには次の情報が含まれます。

* **画像 ID**：問題のある画像の ID。

* **時間**：過去 24 時間以内に、エラーが最初に報告された時刻から最後にエラーが報告された時刻までの時間範囲。

* **カウント**：画像に関してレポートされるエラーの数。

* **応答**：特定のエラーメッセージ。 エラーは 4xx または 5xx です。

* **URL**:Adobe Dynamic Media Classic上の画像の URL を表示します。

* **リファラー**：最初のリクエストが行われた Web サイトの URL を指定します。 リファラーは、画像へのリンクを持つ任意の Web サイトにすることができます。

「URL」列および「リファラ」列には、テストを簡略化するための「URL をコピー」が関連付けられています。
