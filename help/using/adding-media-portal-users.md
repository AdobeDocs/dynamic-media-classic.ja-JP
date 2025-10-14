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

管理者は、ユーザの追加と管理、ユーザによるパスワードの変更を許可するかどうかの指定、ユーザ情報の編集、ユーザリストのアップロードを実行できます。これらのタスクは、ユーザ管理画面で実行されます。この画面にアクセスするには、**[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 管理設定]**/**[!UICONTROL ユーザー管理]** に移動します。

>[!NOTE]
>
>ユーザを追加する前に、ユーザを管理するためのグループを設定します。Media Portal では、ユーザーを 1 つ以上のグループに割り当てることでユーザーを追加できます。 詳しくは、[&#x200B; メディアポータルグループの作成と管理 &#x200B;](creating-media-portal-groups.md#creating_and_managing_media_portal_groups) を参照してください。

## メディアポータルパスワードの管理 {#handling-media-portal-passwords}

Media Portal ユーザ、寄稿者、寄稿者ユーザをサインアップしたときに、それらのユーザにパスワードが記載されたご案内の電子メールが送信されます。管理者は、Media Portal ユーザがこのパスワードを変更できるようにするかどうかを指定できます。

1. **[!UICONTROL 設定]**/**[!UICONTROL メディアポータル設定]**/**[!UICONTROL 一般設定]** に移動します。
1. 全般設定ページで、**[!UICONTROL 「Media Portal ユーザによるパスワードの変更を許可」]**&#x200B;オプションを選択または選択解除します。
1. **[!UICONTROL 保存]** を選択します。

>[!NOTE]
>
>Media Portal ユーザーはパスワードの変更が許可されている場合、「個人設定」画面で **[!UICONTROL 設定]**/**[!UICONTROL 個人設定]** を選択してパスワードを変更できます。

## Media Portal ユーザーの追加 {#adding-a-media-portal-user}

1. **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 管理設定]**/**[!UICONTROL ユーザー管理]** に移動します。
1. ユーザー管理ページで、「**追加**」を選択します。
1. **[!UICONTROL `Add User`]** ダイアログボックスのユーザー情報パネルで、ユーザーの名、姓、メールアドレスを入力し、「**[!UICONTROL 次へ]**」を選択します。
1. 会社 / 役割パネルの会社ドロップダウンリストで、ユーザの会社を選択します。
1. 役割リストで、メディアポータルの役割を選択し、「**[!UICONTROL 次へ]**」を選択します。

   詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

1. アクセスグループパネルで、1 つまたは複数のグループを選択します。

   [&#x200B; メディアポータルグループの作成と管理 &#x200B;](creating-media-portal-groups.md#creating_and_managing_media_portal_groups) を参照してください。

1. （オプション）デフォルトの設定とは異なるメール設定を選択するには、「**[!UICONTROL メール設定]**」を選択します。

   [Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。

1. 「**[!UICONTROL ユーザーを追加]**」を選択します。

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
1. **[!UICONTROL ユーザーリストをアップロード]** を選択します。
1. アップロードするファイルを選択ダイアログボックスで、CSV ファイルを選択して **[!UICONTROL 開く]** を選択します。

リスト内の各ユーザーは、指定したグループに自動的に追加されます。 追加を通知する電子メールメッセージが各ユーザに送信されます。

>[!NOTE]
>
>CSV ファイルが正しい形式でない場合は、次のエラーメッセージが表示されます。「アップロードされた CSV ファイルの処理中にエラーが発生しました。 ファイルの内容が有効なデータかどうかを確認します。」 また、CSV に既存の IP ユーザーまたは IPS ユーザーが含まれている場合、そのユーザーはユーザーリストに追加されません。

## 選択可能な Media Portal ユーザリストの生成 {#generating-a-selectable-list-of-media-portal-users}

Media Portal ユーザの名前と電子メールアドレスをポップアップウィンドウに表示できます。このリストは、ユーザ名とアドレスを Media Portal 以外で使用するためにカットおよびペーストする場合に便利です。

1. **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 管理設定]**/**[!UICONTROL ユーザー管理]** に移動します。
1. **[!UICONTROL ユーザーの役割別]** ドロップダウン・リストで、Media Portal ユーザーの役割の名前を選択し、**[!UICONTROL 更新]** を選択して、Media Portal ユーザーのクラスの名前を表示します。
1. **[!UICONTROL ポップアップ リスト]** を選択します。 このリストをコピー&amp;ペーストします。

## Media Portal ユーザ向けのご案内の電子メールメッセージの設定 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

新規 Media Portal ユーザ、寄稿者、寄稿者ユーザを追加する際に、ご案内の電子メールを送信できます。このメールメッセージを設定するか、Adobe Dynamic Media Classicに送信しないように指定できます。

1. **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 管理設定]**/**[!UICONTROL ユーザー管理]** に移動します。
1. ユーザー管理設定画面で、「**[!UICONTROL メール設定]**」を選択します。
1. 電子メール設定ダイアログボックスで、次のいずれかの設定を指定します。

   * **[!UICONTROL メールを送信]**：新規ユーザーにサインアップしたことをメールで通知する場合は、このオプションの選択を解除します。

   * **[!UICONTROL デフォルトパスワード]**：新規ユーザーの一時パスワードを入力します。Adobe Dynamic Media Classicでランダムパスワードを生成する場合は、フィールドを空のままにします。 ユーザーは、初めてログインしたときに、パスワードを変更するよう求められます。

   * **[!UICONTROL 置き換え URL]**：ユーザーが別の URL を使用してAdobe Dynamic Media Classicにアクセスする場合は、デフォルトの URL とは異なる URL を入力します。

## その他のユーザ管理タスク {#other-user-management-tasks}

ユーザ管理設定画面から、次のタスクも実行できます。

* **[!UICONTROL ユーザーリストのフィルタリングと並べ替え]**：ユーザーを見つけるために、Media Portal ユーザーのリストをフィルタリングします。

* **[!UICONTROL ユーザーを削除]**：リストからユーザーを削除します。

* **[!UICONTROL ユーザーのアクティベートとアクティベート解除]**：フォルダーへのユーザーのアクセスを一時停止します。

* **[!UICONTROL ユーザー情報の編集]**：ユーザーに関する最新の情報を入力します。

* **[!UICONTROL ユーザー定義フィールドの作成]**：カスタムのユーザー定義メタデータフィールドを作成して、Adobe Dynamic Media Classicでのアセットの整理に役立てます。 このフィールドは必要に応じて、アクティブ化または非アクティブ化することができます。

[ユーザ定義フィールド](application-setup.md#user_defined_fields)を参照してください。
