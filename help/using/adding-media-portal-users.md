---
title: Media Portal ユーザーの追加と管理
description: Adobe Dynamic Media ClassicでMedia Portal ユーザーを追加および管理する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
topic: Administration
level: Intermediate
autotag-review: '2026-05-13T17:37:47.692Z'
TQID: 'https://experienceleague.adobe.com/77PJd-uwpdL58aZssu7Ko0fMDpa17heQ1dUUEXRhdDM'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 1032
ht-degree: 51%

---

# Media Portal ユーザーの追加と管理{#adding-and-managing-media-portal-users}

管理者は、ユーザの追加と管理、ユーザによるパスワードの変更を許可するかどうかの指定、ユーザ情報の編集、ユーザリストのアップロードを実行できます。 これらのタスクは、ユーザ管理画面で実行されます。 この画面にアクセスするには、**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動します。

>[!NOTE]
>
>ユーザを追加する前に、ユーザを管理するためのグループを設定します。 Media Portalでは、ユーザーを1つ以上のグループに割り当てることで、ユーザーを追加できます。 詳しくは、[Media Portal グループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)を参照してください。

## Media Portal パスワードの管理 {#handling-media-portal-passwords}

Media Portal ユーザ、寄稿者、寄稿者ユーザをサインアップしたときに、それらのユーザにパスワードが記載されたご案内の電子メールが送信されます。 管理者は、Media Portal ユーザがこのパスワードを変更できるようにするかどうかを指定できます。

1. **[!UICONTROL 設定]** > **[!UICONTROL メディアポータル設定]** > **[!UICONTROL 一般設定]**&#x200B;に移動します。
1. 全般設定ページで、**[!UICONTROL 「Media Portal ユーザによるパスワードの変更を許可」]**&#x200B;オプションを選択または選択解除します。
1. **[!UICONTROL 保存]**&#x200B;を選択します。

>[!NOTE]
>
>パスワードの変更が許可されているMedia Portal ユーザーは、**[!UICONTROL 設定]**/**[!UICONTROL 個人設定]**&#x200B;を選択し、個人設定画面でパスワードを変更することで、パスワードを変更できます。

## Media Portal ユーザーの追加 {#adding-a-media-portal-user}

1. **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動します。
1. ユーザー管理ページで、**追加**&#x200B;を選択します。
1. **[!UICONTROL `Add User`]** ダイアログボックスのユーザー情報パネルで、ユーザーの名、姓、電子メールアドレスを入力し、**[!UICONTROL 次へ]**&#x200B;を選択します。
1. 会社 / 役割パネルの会社ドロップダウンリストで、ユーザの会社を選択します。
1. 役割リストで、Media Portalの役割を選択し、**[!UICONTROL 次へ]**&#x200B;を選択します。

   詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

1. アクセスグループパネルで、1 つまたは複数のグループを選択します。

   [Media Portal グループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)を参照してください。

1. （オプション）「**[!UICONTROL メール設定]**」を選択して、デフォルト設定とは異なるメール設定を選択します。

   [Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。

1. 「**[!UICONTROL ユーザーを追加]**」を選択します。

ユーザを追加すると、追加を通知する電子メールメッセージが Media Portal からユーザに送信されます。 メッセージには、一時パスワードと Media Portal の URL が含まれています。

## Media Portal ユーザリストのアップロード {#uploading-a-media-portal-user-list}

多数のユーザを追加する場合は、ユーザリストをアップロードできます。 ユーザは、現在選択されているアカウントに自動的に追加されます。

ユーザリストは、ユーザ情報を含む CSV（カンマ区切り）ファイル形式で作成します。 リストがアップロードされると、リスト内のユーザが自動的にアカウントに追加され、指定されているグループが割り当てられます。 追加を通知する電子メールが各新規ユーザに送信されます。この電子メールには、Media Portal へのリンクと一時パスワードが含まれます。

### CSV ファイルの作成 {#create-the-csv-file}

次の形式とフィールドに従った CSV ファイル（filename.csv）を作成します。 ファイルの最初の行には、次の表の列見出しを含める必要があります。列の順序は任意です。 列はすべて必須です。

| 列名 | 説明 |
|--- |--- |
| 名 | 名前。 |
| 姓 | 姓。 |
| 電子メール | 有効な電子メールアドレス。 |
| パスワード | パスワード（大文字と小文字を区別）。 |
| ユーザの役割 | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorUser |
| グループ | 各ユーザの 1 つまたは複数のアカウントグループ割り当てをカンマで区切ったリストです。 アカウント名にプリフィックスを付け、スラッシュ（/）で区切ることで、グループを指定します。 例えば、PortalCo/IT の場合、PortalCo はアカウント、IT は PortalCo アカウント内のグループです。 |

次のサンプルスプレッドシートで、CSV ファイルのレイアウト方法の例を示します。

| 名 | 姓 | 電子メール | パスワード | ユーザの役割 | グループ |
|--- |--- |--- |--- |--- |--- |
| プレーリー | Kat | `prairiek@company.com` | welcome | MediaPortal 管理者 | PortalCo/IT、PortalCo/Admin |
| リック | Brough | `rickb@myco.com` | welcome | Media Portal ユーザ | PortalCo/MktgGroup, PortalCo/test |

### CSV ファイルのアップロード {#uploading-the-csv-file}

1. ユーザ管理設定画面を開きます。
1. 「**[!UICONTROL ユーザーリストをアップロード]**」を選択します。
1. アップロードするファイルを選択ダイアログボックスで、CSV ファイルを選択し、**[!UICONTROL 開く]**&#x200B;を選択します。

リスト内の各ユーザーは、指定したグループに自動的に追加されます。 追加を通知する電子メールメッセージが各ユーザに送信されます。

>[!NOTE]
>
>CSV ファイルが正しくフォーマットされていない場合は、次のエラーメッセージが表示されます。「アップロードされたCSV ファイルの処理中にエラーが発生しました。 有効なデータのファイル内容を確認してください。」 また、CSVに既存のIPまたはIPS ユーザーが含まれている場合、そのユーザーはユーザーリストに追加されません。

## 選択可能な Media Portal ユーザリストの生成 {#generating-a-selectable-list-of-media-portal-users}

Media Portal ユーザの名前と電子メールアドレスをポップアップウィンドウに表示できます。 このリストは、ユーザ名とアドレスを Media Portal 以外で使用するためにカットおよびペーストする場合に便利です。

1. **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動します。
1. **[!UICONTROL ユーザーの役割]** ドロップダウンリストで、Media Portal ユーザーの役割の名前を選択し、**[!UICONTROL 更新]**&#x200B;を選択して、Media Portal ユーザーの1つのクラスの名前を表示します。
1. **[!UICONTROL ポップアップリスト]**&#x200B;を選択します。 このリストをコピー&amp;ペーストします。

## Media Portal ユーザ向けのご案内の電子メールメッセージの設定 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

新規 Media Portal ユーザ、寄稿者、寄稿者ユーザを追加する際に、ご案内の電子メールを送信できます。 この電子メールメッセージを設定するか、Adobe Dynamic Media Classicに送信しないように指示できます。

1. **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Administration Setup]** > **[!UICONTROL User Administration]**&#x200B;に移動します。
1. ユーザー管理の設定画面で、**[!UICONTROL メール設定]**&#x200B;を選択します。
1. 電子メール設定ダイアログボックスで、次のいずれかの設定を指定します。

   * **[!UICONTROL 電子メールを送信]**：このオプションの選択を解除すると、新規登録者に電子メールで通知されます。

   * **[!UICONTROL デフォルトのパスワード]**：新規ユーザーの一時パスワードを入力するか、フィールドを空のままにして、Adobe Dynamic Media Classicでランダムなパスワードを生成します。 ユーザーは、初めてログインしたときにパスワードを変更するように求められます。

   * **[!UICONTROL 置き換えURL]**：ユーザーが別のURLを使用してAdobe Dynamic Media Classicにアクセスする場合は、デフォルトとは異なるURLを入力します。

## その他のユーザ管理タスク {#other-user-management-tasks}

ユーザ管理設定画面から、次のタスクも実行できます。

* **[!UICONTROL ユーザーリストをフィルタリングして並べ替え]**: Media Portal ユーザーのリストをフィルタリングしてユーザーを検索します。

* **[!UICONTROL ユーザーを削除]**: リストからユーザーを削除します。

* **[!UICONTROL ユーザーをアクティブ化および非アクティブ化]**: ユーザーのフォルダーへのアクセスを停止します。

* **[!UICONTROL ユーザー情報を編集]**: ユーザーに関する最新情報を入力します。

* **[!UICONTROL ユーザー定義フィールドを作成]**: ユーザー定義のカスタムメタデータフィールドを作成して、Adobe Dynamic Media Classicでのアセットの整理に役立てることができます。 このフィールドは必要に応じて、アクティブ化または非アクティブ化することができます。

[ユーザ定義フィールド](application-setup.md#user_defined_fields)を参照してください。
