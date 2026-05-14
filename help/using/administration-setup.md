---
title: 管理設定
description: Adobe Dynamic Media Classicの管理領域の設定方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin
exl-id: 14e3d8be-f265-4cec-aa8e-19ef71526b68
topic: Administration
level: Intermediate
autotag-review: '2026-05-13T17:38:22.364Z'
TQID: 'https://experienceleague.adobe.com/UbxE4vDKYB-6CsdV2d4lX2WeOMYPe9caewOQD-MBark'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 2004
ht-degree: 29%

---

<!-- UPDATE TOPIC AFTER DECEMBER 31, 2020!!!! -->

# 管理の設定{#administration-setup}

管理設定の画面は、Adobe Dynamic Media Classic ユーザーを管理するためのものです。 これらの画面を使用すると、Adobe Dynamic Media Classicで作業したり、他のユーザーと電子メールで通信したりできます。

1. 管理設定オプションにアクセスするには、**設定** > **個人設定** > **管理設定**&#x200B;に移動します。

## ユーザー管理 {#user-administration}

すべてのAdobe Dynamic Media Classic ユーザーには、Adobe Dynamic Media Classicの機能に対する権限とアクセス権を決定するロールが割り当てられます。 管理者が、割り当てられている会社に対する各ユーザの役割や責任を決定します。

通常、Adobe Dynamic Media Classicは最初の会社セットを設定し、会社管理者を割り当てます。 次に、会社管理者がAdobe Dynamic Media Classic ユーザーを設定して管理します。

Adobe Dynamic Media Classicでは、複数のユーザーの役割をサポートしています。 次の役割は、Adobe Dynamic Media Classic用に設定された会社にアクセスできます。

<!-- **Adobe Dynamic Media Classic Administrator** Can view and administer all features in Adobe Dynamic Media Classic, as well as set up companies and add administrators and users. -->

**Adobe Dynamic Media Classic ユーザー**&#x200B;は、割り当てられた会社にアクセスできます。管理業務を行うことはできません。

**Adobe Dynamic Media Classic Company Admin**&#x200B;は、自分の会社のみを表示および管理できます。 また、管理者やユーザの追加といったすべての管理機能を実行できます。 会社の管理者は、ユーザーをDMC会社の管理者アカウントに追加できます。 （この役割は、初期設定のユーザの役割です）。

ユーザーを追加すると、Adobe Dynamic Media Classicはユーザーにウェルカムメールメッセージを送信します。 メッセージには、パスワードとAdobe Dynamic Media ClassicのURLが含まれています。

### ユーザーまたは管理者の追加 {#adding-a-user-or-administrator}

1. **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動します。
1. 「**[!UICONTROL 追加]**」を選択します。
1. 追加するユーザーまたは管理者の名前と電子メールアドレスを入力し、**[!UICONTROL 次へ]**&#x200B;を選択します。

   >[!NOTE]
   >
   >アポストロフィ文字（`'`）は、電子メールアドレスでは使用できません。

1. ユーザーに役割を割り当てるには、「役割」オプションを選択します。

   [Adobe Dynamic Media Classic ユーザーの役割と権限](administration-setup.md#user_administration)を参照してください。

1. ユーザーを会社に追加するには、会社名を選択します。
1. ユーザーをグループに追加する場合（Media Portal ユーザーまたはコントリビューターを追加する場合）、**[!UICONTROL 次へ]**&#x200B;を選択してユーザーを追加します。
1. 「**[!UICONTROL 保存]**」を選択して、ユーザー設定を完了します。

   保存後、ユーザを別の会社に追加するかどうかを確認するメッセージが表示されます。 ユーザーを会社に追加する場合は、**[!UICONTROL 追加]**&#x200B;を選択します。

   新規ユーザーには、ランダムに生成されたパスワードが付与されます。Adobe Dynamic Media Classic デスクトップアプリケーションに初めてログインする場合は、パスワードを変更する必要があります。

   新規ユーザを追加した後、新規ユーザにご案内の電子メールが送信されます。 このメールには、一時的なパスワードが記載されており、Adobe Dynamic Media Classicへのログイン方法が説明されています。

   ユーザーがウェルカムメールを受信しない場合は、Adobe Dynamic Media Classicのサインインページ（https://s7sps1.scene7.com）に移動し、「**[!UICONTROL パスワードを忘れた場合]**」を選択します。 パスワードがリセットされ、新しい電子メールが送信されます。 ユーザが電子メールを受信せず、迷惑メールフォルダにもない場合は、テクニカルサポートに問い合わせてください。

   新しいMedia Portal ユーザーを追加する場合は、**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動し、**[!UICONTROL Upload User List]**&#x200B;を選択して、500人以下のユーザーを含む.csv ファイルを選択することもできます。

### ユーザの削除 {#delet-a-user}

Adobe Dynamic Media Classicからユーザーを削除するには、ユーザーを無効にします。 無効なユーザは、システムとすべてのアカウントから削除されます。

1. **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動します。
1. リストからユーザーを選択し、**[!UICONTROL 編集]**&#x200B;を選択します。
1. 「有効」の選択を解除します。
1. **[!UICONTROL 保存]**&#x200B;を選択します。

### ユーザーの有効化または無効化 {#activating-or-deactivating-users}

ユーザを非アクティブにすると、アクセスするアカウントを選択メニューの一番上に表示されるアカウントにアクセスする権限がなくなります。

1. **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動します。
1. ユーザーリストで、ユーザー名の横にある「**[!UICONTROL アクティブ]**」オプションを選択または選択解除します。

### ユーザ情報の編集 {#editing-user-information}

編集できるユーザ情報は、管理者としての役割、および情報編集先であるユーザに対して割り当てられた役割によって異なります。 グレー表示（使用できない）オプションは、編集できません。

1. **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動します。
1. リストからユーザーを選択し、**[!UICONTROL 編集]**&#x200B;を選択します。
1. 権限またはアクセス権を変更しようとしている会社を示すテーブルのエントリを選択し、**[!UICONTROL 会社を管理]**&#x200B;を選択します。
1. ユーザの役割を選択します。
1. ユーザーのグループメンバーシップを変更する場合（Media Portal ユーザーまたはコントリビューターを編集または追加する場合）、**[!UICONTROL 次へ]**&#x200B;を選択してグループメンバーシップを編集します。
1. **[!UICONTROL 保存]**&#x200B;を選択します。

### ユーザリストのフィルタリングと並べ替え {#filtering-and-sorting-the-user-list}

ユーザリストのフィルタリングや並べ替えを行ってユーザを探すことができます。 ユーザリストには、アクセスするアカウントを選択メニューで選択されているアカウントに関係なく、管理下のすべてのアカウント内のすべてのユーザが表示されます。

次のユーザーリストフィルタリング手法を使用できます。

* **グループ別にフィルター**: **[!UICONTROL グループ別]** メニューを選択し、グループ内のユーザーにリストを絞り込むオプションを選択します。

* **ユーザーの役割でフィルター**:「**[!UICONTROL ユーザーの役割]**」メニューを選択し、様々なタイプのユーザーまたは管理者にリストを絞り込むオプションを選択します。

* **フィールド名でフィルター**:「**[!UICONTROL フィールドでフィルターを有効にする]**」を選択します。 次に、**[!UICONTROL フィールド名]** メニューを選択し、リストをフィルタリングする列を選択し、「文字をフィルター」メニューを選択してレターを選択します。 リストは、選択した文字によって、いずれかの列でフィルタリングされます。 完全なリストを表示するには、**`Enable Filter By Field`** オプションの選択を解除します。

* **無効なユーザーを除外**：選択解除&#x200B;**[!UICONTROL 無効なユーザーを含める]**。 検索結果には、システム内のユーザだけが表示されます。 無効なユーザーがシステムおよび管理するアカウントから削除されました。

* **列見出しで並べ替え**：すべてのユーザーをステータスで、アルファベット順に名、姓、または電子メールで並べ替える見出しを選択します。 または、ユーザーの役割、または有効/無効なステータスでソートします。

ユーザ数が多い場合は、最大リストサイズメニューを選択し、数値を選択することで、リストのサイズを制限できます。

<!-- 
CQDOC-16690 TOPIC REMOVED AS PER JIRA TICKET INSTRUCTIONS ### Linking an IMS user identity to an Adobe Dynamic Media Classic IPS user account {#linking-an-ims-user-identity-to-a-scene-ips-user-account}

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

Adobe Dynamic Media Classic管理者は、管理会社の帯域幅、ストレージ、その他の種類のレポートを生成できます。 これらのレポートは、「帯域幅とストレージ」ページで入手できます。

このページを開くには、**[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**&#x200B;に移動します。 **[!UICONTROL 管理セットアップ]**&#x200B;を展開し、**[!UICONTROL 帯域幅とストレージ]**&#x200B;を選択します。

### レポートのタイプ {#types-of-reports}

次の表に、「帯域幅とストレージ」ページから生成できるレポートを示します。

| レポート | 情報 | 使用方法 |
| --- | --- | --- |
| 帯域幅 | | **重要**:「帯域幅」タブはサポートされなくなりました。 UIにはまだ表示されますが、帯域幅データは使用できず、すべての値は`0`として表示されます。 |
| ストレージ | ストレージ使用量 | 企業がアップロードしたデータ量を追跡します。 |
| 画像コンテンツ | リクエストタイプとサブタイプ別に、ヒット数と画像の配信数の合計が表示されます。 | ビデオ以外のアセットの指標を含む、様々な画像タイプのリクエスト数とボリュームを追跡します。 |
| ドメイン | URL 要求数（ドメイン別） | 特定の会社の画像要求のドメインに基づいて画像の使用量を追跡します （Adobe Dynamic Media Classicは、アカウントごとに複数のドメインを提供できます。 詳しくは、テクニカルサポートにお問い合わせください）。 |
| ビデオストリーミング | ストリーミングビデオの帯域幅使用量 | 特定の日付範囲にわたるストリーミングビデオ使用量を会社別に追跡して、トラフィックパターンを判断します。 |
| ビデオコンテンツ | 様々なビデオの再生時間 | 最も視聴回数の多かったビデオと最も視聴回数が少なかったビデオを判断します。 |

画像コンテンツレポートは、以下の画像タイプの要求に関する情報を提供します。

* **画像リクエスト**：画像のリクエスト。

* **サムネール要求**：視聴者のスウォッチまたは代替画像の要求。

* **マスク要求**：画像に対する要求がグレースケール マスクを返しています。

* **ビューア タイル リクエスト**：ビューアによって読み込まれた画像リクエスト。

* **VNT オブジェクト要求**：要求された周辺光量内の指定されたオブジェクトを含む画像を返す画像レンダリング要求。

* **VNT情報要求**：要求された周辺光量補正に関する情報を返す画像レンダリング要求。

>[!NOTE]
>
>ビデオストリーミングレポートは、ストリーミングビデオにのみ該当します。 プログレッシブ動画の視聴を追跡することはありません。

### レポートの生成 {#generating-a-report}

帯域幅、ストレージ、画像コンテンツ、ドメイン、ビデオストリーミングまたはビデオコンテンツのレポートを生成するには：

1. **[!UICONTROL セットアップ]** / **[!UICONTROL 個人設定]**&#x200B;に移動します。
1. 管理セットアップを展開し、**[!UICONTROL 帯域幅とストレージ]**&#x200B;を選択します。
1. タブを選択：**[!UICONTROL 帯域幅]**、**[!UICONTROL ストレージ]**、**[!UICONTROL 画像コンテンツ]**、**[!UICONTROL ドメイン]**、**[!UICONTROL ビデオストリーミング]**、または&#x200B;**[!UICONTROL ビデオコンテンツ]**。

   [レポートのタイプ](administration-setup.md#types_of_reports)を参照してください。

### データを様々な方法で表示 {#viewing-data-in-different-ways}

帯域幅とストレージページでレポートを生成した後に、情報を表示するためのオプションを選択できます。 情報の種類、情報の表示方法（グラフまたはデータグリッド）および情報の収集期間を指定できます。 データビューで、情報を並べ替えたり、列の順番を変更することができます。

* **グラフまたはデータグリッドでデータを表示**: グラフでデータを表示するには&#x200B;**[!UICONTROL チャートビュー]**&#x200B;を選択し、データグリッドでデータを表示するには&#x200B;**[!UICONTROL データビュー]**&#x200B;を選択します。

* **レポートのプレゼンテーションの種類を選択**: レポートの種類メニューで、**[!UICONTROL 概要]**、**[!UICONTROL 日次]**、または&#x200B;**[!UICONTROL 月次]**&#x200B;を選択して、概要形式、日別、月別にデータを整理します。 一部のレポートには、このオプションはありません。

* **期間を指定**: レポートの期間を定義するオプションを選択し、期間を定義した後で&#x200B;**[!UICONTROL 更新]**&#x200B;を選択します。

* **定義済み期間**：定義済みレポートメニューで、オプションを選択します。 例えば、先月からのデータを収集するには、「先月」を選択します。

* **カスタム期間**：定義済みレポートメニューで、**[!UICONTROL カスタム]**&#x200B;を選択します。 次に、**[!UICONTROL 開始月]** （または&#x200B;**[!UICONTROL 開始日]**）メニューの日付と、月数（#または#日）メニューの日付を選択します。 ドメインレポートおよびビデオコンテンツレポートでは、レポート情報を収集するための特定の開始日と終了日を選択できます。

* **データの並べ替え（データビューのみ）**：列の情報の並べ替え。 列の見出しを選択します。 降順に並べ替えるには、もう一度選択します。

* **列の並べ替え（データビューのみ）**：列をデータグリッド上の別の場所に移動するには、その見出しをドラッグします。

### レポートの書き出しと印刷 {#exporting-and-printing-reports}

レポートの生成後に、スプレッドシートやその他のアプリケーションで使用できるようにデータを書き出すことができます。 また、レポートを印刷することもできます。

* **レポート データの書き出し**: データ ビューで、必要に応じてデータを並べ替え、並べ替えます。 次に、**[!UICONTROL 書き出し]** メニューを開き、書式を選択します：**[!UICONTROL タブ区切り]**、**[!UICONTROL コンマ区切り]**、または&#x200B;**[!UICONTROL HTML書式設定]**。 データは、選択した形式でクリップボードにコピーされます。 これでデータをスプレッドシートやアプリケーションにペーストできます。

* **レポートを印刷**: **[!UICONTROL 印刷]**&#x200B;を選択し、印刷ダイアログボックスで必要なオプションを選択してから、**[!UICONTROL OK]**&#x200B;を選択します。

## 画像エラー {#image-errors}

Adobe Dynamic Media Classic管理者は、画像エラーレポートを生成できます。 画像エラーレポートは、現在ログインしている会社について、直近 24 時間以内で最も頻度の高い画像エラー 20 個をリストで表示します。 画像エラーレポートを生成するには、次の操作を行います。

1. **[!UICONTROL セットアップ]** / **[!UICONTROL 個人設定]**&#x200B;に移動します。
1. 管理設定を展開し、**[!UICONTROL 画像エラー]**&#x200B;を選択します。
1. 必要に応じて次の操作を行います。

   * 見出し情報でエラーを並べ替えるには、見出しを選択します。 初期設定では、エラーは発生頻度の高い順に並んでいます。
   * カーソルをエラーの「応答」フィールド上に移動すると、詳細なエラーメッセージが表示されます。
   * 画像またはリファラーのWeb ページへのリンクを表示するには、URL フィールドまたはリファラーフィールドにカーソルを移動します。
   * リンクを実際の画像にコピーするには、**[!UICONTROL URL コピーURL]**&#x200B;を選択します。 このリンクをブラウザウィンドウにペーストして画像のページに移動し、エラーを調べることができます。
   * リンクをリファラーWeb ページにコピーするには、**[!UICONTROL リファラーコピーURL]**&#x200B;を選択します。

表示されるエラーは、現在ログインしている会社のものです。 各エラーには次の情報が含まれます。

* **画像ID**：問題のある画像のID。

* **時刻**：最初にエラーが報告された時刻の時間範囲（最後の24時間以内）。

* **Count**：画像で報告されたエラーの数。

* **応答**：特定のエラーメッセージ。 エラーは 4xx または 5xx です。

* **URL**: Adobe Dynamic Media Classicの画像のURLを一覧表示します。

* **Referrer**：最初のリクエストの送信元となるWeb サイトのURLを指定します。 リファラーは、画像へのリンクを持つ任意のWeb サイトにすることができます。

「URL」列および「リファラ」列には、テストを簡略化するための「URL をコピー」が関連付けられています。
