---
title: メディアポータルユーザーの追加と管理
description: Adobe Dynamic Media Classicで Media Portal ユーザーを追加および管理する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
topic: Administration
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 50%

---

# メディアポータルユーザーの追加と管理{#adding-and-managing-media-portal-users}

管理者は、ユーザの追加と管理、ユーザによるパスワードの変更を許可するかどうかの指定、ユーザ情報の編集、ユーザリストのアップロードを実行できます。これらのタスクは、ユーザ管理画面で実行されます。この画面にアクセスするには、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL ユーザー管理]**.

>[!NOTE]
>
>ユーザを追加する前に、ユーザを管理するためのグループを設定します。Media Portal では、ユーザーを 1 つ以上のグループに割り当てることでユーザーを追加できます。 詳しくは、を参照してください [メディアポータルグループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

## メディアポータルパスワードの管理 {#handling-media-portal-passwords}

Media Portal ユーザ、寄稿者、寄稿者ユーザをサインアップしたときに、それらのユーザにパスワードが記載されたご案内の電子メールが送信されます。管理者は、Media Portal ユーザがこのパスワードを変更できるようにするかどうかを指定できます。

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL メディアポータルの設定]** > **[!UICONTROL 一般設定]**.
1. 全般設定ページで、**[!UICONTROL 「Media Portal ユーザによるパスワードの変更を許可」]**&#x200B;オプションを選択または選択解除します。
1. を選択 **[!UICONTROL 保存]**.

>[!NOTE]
>
>パスワード変更が許可されている Media Portal ユーザーは、次のオプションを選択してパスワードを変更できます。 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]** パスワードを変更する場合は、[ 個人設定 ] 画面で行います。

## Media Portal ユーザーの追加 {#adding-a-media-portal-user}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL ユーザー管理]**.
1. ユーザー管理ページで、次を選択します。 **追加**.
1. が含まれる **[!UICONTROL `Add User`]** ダイアログボックスのユーザー情報パネルで、ユーザーの名、姓およびメールアドレスを入力し、を選択します。 **[!UICONTROL 次]**.
1. 会社 / 役割パネルの会社ドロップダウンリストで、ユーザの会社を選択します。
1. 役割リストで、メディアポータルの役割を選択し、を選択します **[!UICONTROL 次]**.

   詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

1. アクセスグループパネルで、1 つまたは複数のグループを選択します。

   参照： [メディアポータルグループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups).

1. （オプション）を選択 **[!UICONTROL E メール設定]** 既定の設定とは異なる電子メール設定を選択します。

   [Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。

1. を選択 **[!UICONTROL ユーザーを追加]**.

ユーザを追加すると、追加を通知する電子メールメッセージが Media Portal からユーザに送信されます。メッセージには、一時パスワードと Media Portal の URL が含まれています。

## Media Portal ユーザリストのアップロード {#uploading-a-media-portal-user-list}

多数のユーザを追加する場合は、ユーザリストをアップロードできます。ユーザは、現在選択されているアカウントに自動的に追加されます。

ユーザリストは、ユーザ情報を含む CSV（カンマ区切り）ファイル形式で作成します。リストがアップロードされると、リスト内のユーザが自動的にアカウントに追加され、指定されているグループが割り当てられます。追加を通知する電子メールが各新規ユーザに送信されます。この電子メールには、Media Portal へのリンクと一時パスワードが含まれます。

### CSV ファイルの作成 {#create-the-csv-file}

次の形式とフィールドに従った CSV ファイル（filename.csv）を作成します。ファイルの最初の行には、次の表の列見出しを含める必要があります。列の順序は任意です。列はすべて必須です。

| 列名 | 説明 |
|--- |--- |
| 名 | 名前。 |
| 姓 | 姓。 |
| 電子メール | 有効な電子メールアドレス。 |
| パスワード | パスワード（大文字と小文字を区別）。 |
| ユーザの役割 | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| グループ | 各ユーザの 1 つまたは複数のアカウントグループ割り当てをカンマで区切ったリストです。アカウント名にプリフィックスを付け、スラッシュ（/）で区切ることで、グループを指定します。例えば、PortalCo/IT の場合、PortalCo はアカウント、IT は PortalCo アカウント内のグループです。 |

次のサンプルスプレッドシートで、CSV ファイルのレイアウト方法の例を示します。

| 名 | 姓 | 電子メール | パスワード | ユーザの役割 | グループ |
|--- |--- |--- |--- |--- |--- |
| プレーリー | カート | `prairiek@company.com` | welcome | MediaPortal 管理者 | PortalCo/IT, PortalCo/Admin |
| リック | ブロウ | `rickb@myco.com` | welcome | Media Portal ユーザ | PortalCo/MktgGroup, PortalCo/test |

### CSV ファイルのアップロード {#uploading-the-csv-file}

1. ユーザ管理設定画面を開きます。
1. を選択 **[!UICONTROL ユーザーリストをアップロード]**.
1. アップロードするファイルを選択ダイアログボックスで、CSV ファイルを選択してから選択します **[!UICONTROL 開く]**.

リスト内の各ユーザーは、指定したグループに自動的に追加されます。 追加を通知する電子メールメッセージが各ユーザに送信されます。

>[!NOTE]
>
>CSV ファイルが正しい形式でない場合は、次のエラーメッセージが表示されます。「アップロードされた CSV ファイルの処理中にエラーが発生しました。 ファイルの内容が有効なデータかどうかを確認します。」 また、CSV に既存の IP ユーザーまたは IPS ユーザーが含まれている場合、そのユーザーはユーザーリストに追加されません。

## 選択可能な Media Portal ユーザリストの生成 {#generating-a-selectable-list-of-media-portal-users}

Media Portal ユーザの名前と電子メールアドレスをポップアップウィンドウに表示できます。このリストは、ユーザ名とアドレスを Media Portal 以外で使用するためにカットおよびペーストする場合に便利です。

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL ユーザー管理]**.
1. が含まれる **[!UICONTROL ユーザーの役割別]** ドロップダウンリストで、メディアポータルユーザーの役割の名前を選択し、以下を選択します **[!UICONTROL 更新]** メディアポータルユーザーの 1 つのクラスの名前を表示します。
1. を選択 **[!UICONTROL ポップアップリスト]**. このリストをコピー&amp;ペーストします。

## Media Portal ユーザ向けのご案内の電子メールメッセージの設定 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

新規 Media Portal ユーザ、寄稿者、寄稿者ユーザを追加する際に、ご案内の電子メールを送信できます。このメールメッセージを設定するか、Adobe Dynamic Media Classicに送信しないように指定できます。

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 管理設定]** > **[!UICONTROL ユーザー管理]**.
1. ユーザー管理設定画面で、次の項目を選択します。 **[!UICONTROL E メール設定]**.
1. 電子メール設定ダイアログボックスで、次のいずれかの設定を指定します。

   * **[!UICONTROL メールを送信]**：新規ユーザーにサインアップしたことを電子メールで通知するには、このオプションの選択を解除します。

   * **[!UICONTROL デフォルトのパスワード]**：新規ユーザーの一時パスワードを入力するか、フィールドを空のままにして、Adobe Dynamic Media Classicでランダムパスワードを生成します。 ユーザーは、初めてログインしたときに、パスワードを変更するよう求められます。

   * **[!UICONTROL 置き換える URL]**：ユーザーが別の URL からAdobe Dynamic Media Classicにアクセスする場合は、デフォルトとは異なる URL を入力します。

## その他のユーザ管理タスク {#other-user-management-tasks}

ユーザ管理設定画面から、次のタスクも実行できます。

* **[!UICONTROL ユーザーリストのフィルタリングと並べ替え]**:Media Portal ユーザーのリストをフィルタリングして、ユーザーを見つけます。

* **[!UICONTROL ユーザーの削除]**：リストからユーザーを削除します。

* **[!UICONTROL ユーザーのアクティベートとアクティベート解除]**：フォルダーへのユーザーのアクセスを一時停止します。

* **[!UICONTROL ユーザー情報の編集]**：ユーザーに関する最新の情報を入力します。

* **[!UICONTROL ユーザー定義フィールドの作成]**：カスタムのユーザー定義メタデータフィールドを作成して、Adobe Dynamic Media Classicでのアセットの整理に役立てます。 このフィールドは必要に応じて、アクティブ化または非アクティブ化することができます。

[ユーザ定義フィールド](application-setup.md#user_defined_fields)を参照してください。
