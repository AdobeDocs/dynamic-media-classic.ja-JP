---
title: Media Portal のユーザの追加と管理
description: Media Portalユーザーの追加方法と管理方法について説明します
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Administrator,Business Practitioner
exl-id: 9590c53c-fd38-4bf2-b723-cd7369702364
source-git-commit: 31ac96e6fd11c47284d58540f5ec0135f0e6223b
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 81%

---

# Media Portal のユーザの追加と管理{#adding-and-managing-media-portal-users}

管理者は、ユーザの追加と管理、ユーザによるパスワードの変更を許可するかどうかの指定、ユーザ情報の編集、ユーザリストのアップロードを実行できます。これらのタスクは、ユーザ管理画面で実行されます。この画面にアクセスするには、**[!UICONTROL 設定]**／**[!UICONTROL アプリケーション設定]**&#x200B;をクリックし、**[!UICONTROL 「管理設定」]**&#x200B;で、**[!UICONTROL 「ユーザ管理」]**&#x200B;をクリックします。

>[!NOTE]
>
>ユーザを追加する前に、ユーザを管理するためのグループを設定します。Media Portal では、ユーザを 1 つまたは複数のグループに割り当てないと、ユーザを追加できません。詳しくは、[Media Portal グループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)を参照してください。

## Media Portal のパスワードの処理 {#handling-media-portal-passwords}

Media Portal ユーザ、寄稿者、寄稿者ユーザをサインアップしたときに、それらのユーザにパスワードが記載されたご案内の電子メールが送信されます。管理者は、Media Portal ユーザがこのパスワードを変更できるようにするかどうかを指定できます。

1. **[!UICONTROL 設定]**／**[!UICONTROL Media Portal 設定]**／**[!UICONTROL 全般設定]**&#x200B;をクリックします。
1. 全般設定ページで、**[!UICONTROL 「Media Portal ユーザによるパスワードの変更を許可」]**&#x200B;オプションを選択または選択解除します。
1. **[!UICONTROL 「保存」]**&#x200B;をクリックします。

>[!NOTE]
>
>パスワードの変更が許可された Media Portal ユーザは、**[!UICONTROL 設定]**／**[!UICONTROL 個人設定]**&#x200B;を選択して、個人設定画面でパスワードを変更することができます。

## Media Portal ユーザの追加 {#adding-a-media-portal-user}

1. **[!UICONTROL 設定]**／**[!UICONTROL アプリケーション設定]**／**[!UICONTROL 管理設定]**／**[!UICONTROL ユーザ管理]**&#x200B;をクリックします。
1. ユーザ管理ページで、**「追加」**&#x200B;をクリックします。
1. ユーザを追加ダイアログボックスのユーザ情報パネルで、ユーザの名、姓、および電子メールアドレスを入力し、**[!UICONTROL 「次へ」]**&#x200B;をクリックします。
1. 会社 / 役割パネルの会社ドロップダウンリストで、ユーザの会社を選択します。
1. 役割リストで、Media Portal 役割を選択し、**[!UICONTROL 次へ]**&#x200B;をクリックします。

   詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

1. アクセスグループパネルで、1 つまたは複数のグループを選択します。

   詳しくは、[Media Portal グループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)を参照してください。

1. （オプション）**[!UICONTROL 「電子メール設定」]**&#x200B;をクリックして、初期設定とは異なる電子メール設定を選択します。

   [Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。

1. **[!UICONTROL 「ユーザを追加」]**&#x200B;をクリックします。

ユーザを追加すると、追加を通知する電子メールメッセージが Media Portal からユーザに送信されます。メッセージには、一時パスワードと Media Portal の URL が含まれています。

## Media Portal ユーザリストのアップロード {#uploading-a-media-portal-user-list}

多数のユーザを追加する場合は、ユーザリストをアップロードできます。ユーザは、現在選択されているアカウントに自動的に追加されます。

ユーザリストは、ユーザ情報を含む CSV（カンマ区切り）ファイル形式で作成します。リストがアップロードされると、リスト内のユーザが自動的にアカウントに追加され、指定されているグループが割り当てられます。追加を通知する電子メールが各新規ユーザに送信されます。この電子メールには、Media Portal へのリンクと一時パスワードが含まれます。

### CSV ファイルの作成 {#creating-the-csv-file}

次の形式とフィールドに従った CSV ファイル（filename.csv）を作成します。ファイルの最初の行には、次の表の列見出しを含める必要があります。列の順序は任意です。列はすべて必須です。

| 列名 | 説明 |
|--- |--- |
| 名 | 名前。 |
| 姓 | 姓。 |
| 電子メール | 有効な電子メールアドレス。 |
| パスワード | パスワード（大文字と小文字を区別）。 |
| ユーザの役割 | MediaPortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorContributorUser |
| グループ | 各ユーザの 1 つまたは複数のアカウントグループ割り当てをカンマで区切ったリストです。アカウント名にプリフィックスを付け、スラッシュ（/）で区切ることで、グループを指定します。例えば、PortalCo/IT の場合、PortalCo はアカウント、IT は PortalCo アカウント内のグループです。 |

次のサンプルスプレッドシートで、CSV ファイルのレイアウト方法の例を示します。

| 名 | 姓 | 電子メール | パスワード | ユーザの役割 | グループ |
|--- |--- |--- |--- |--- |--- |
| プレイリー | カト | `prairiek@company.com` | welcome | MediaPortal 管理者 | PortalCo/IT,PortalCo/Admin |
| Rick | ブルー | `rickb@myco.com` | ようこそ | Media Portal ユーザ | PortalCo/MktgGroup, PortalCo/test |


### CSV ファイルのアップロード {#uploading-the-csv-file}

1. ユーザ管理設定画面を開きます。
1. **[!UICONTROL ユーザリストをアップロード]**&#x200B;をクリックします。
1. アップロードするファイルを選択しますダイアログボックスで CSV ファイルを選択し、**[!UICONTROL 「開く」]**&#x200B;をクリックします。

リスト内の各ユーザが、指定されているグループに自動的に追加されます。追加を通知する電子メールメッセージが各ユーザに送信されます。

>[!NOTE]
>
>CSV ファイルの形式が正しくなかった場合は、次のエラーメッセージが表示されます。「アップロードした CSV ファイルの処理中にエラーが発生しました。ファイルの内容を調べて、データが有効であることを確認してください。」また、CSV に既存の IP または IPS ユーザが含まれていた場合、そのユーザはユーザリストに追加されません。

## 選択可能な Media Portal ユーザリストの生成 {#generating-a-selectable-list-of-media-portal-users}

Media Portal ユーザの名前と電子メールアドレスをポップアップウィンドウに表示できます。このリストは、ユーザ名とアドレスを Media Portal 以外で使用するためにカットおよびペーストする場合に便利です。

1. **[!UICONTROL 設定]**／**[!UICONTROL アプリケーション設定]**／**[!UICONTROL 管理設定]**／**[!UICONTROL ユーザ管理]**&#x200B;をクリックします。
1. **[!UICONTROL 「ユーザの役割が」]**&#x200B;ドロップダウンリストで、Media Portal ユーザの役割名を選択し、**[!UICONTROL 「更新」]**&#x200B;をクリックして、Media Portal ユーザの 1 つのクラスの名前のみを表示します。
1. **[!UICONTROL 「ポップアップリスト」]**&#x200B;をクリックすると、ポップアップウィンドウが開きます。このリストをコピーして貼り付けます。

## Media Portal ユーザ向けのご案内の電子メールメッセージの設定 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

新規 Media Portal ユーザ、寄稿者、寄稿者ユーザを追加する際に、ご案内の電子メールを送信できます。この電子メールメッセージを設定するか、Dynamic Media Classicに送信しないように伝えることができます。

1. **[!UICONTROL 設定]**／**[!UICONTROL アプリケーション設定]**／**[!UICONTROL 管理設定]**／**[!UICONTROL ユーザ管理]**&#x200B;を選択します。
1. ユーザー管理の設定画面で、「**[!UICONTROL 電子メールの設定]**」をクリックします。
1. 電子メール設定ダイアログボックスで、次のいずれかの設定を指定します。

   * **[!UICONTROL 電子メールを送信]**  — 新しいユーザーにサインアップしたことを電子メールで通知しない場合は、このオプションの選択を解除します。

   * **[!UICONTROL デフォルトのパスワード]**  — 新規ユーザーの一時パスワードを入力します。Dynamic Media Classicでランダムなパスワードを生成する場合は、このフィールドを空のままにします。ユーザーは、初めてログインしたときにパスワードを変更するように求められます。

   * **[!UICONTROL 置換URL]**  — ユーザーが別のURLを使用してDynamic Media Classicにアクセスする場合は、デフォルトとは異なるURLを入力します。

## その他のユーザ管理タスク {#other-user-management-tasks}

ユーザ管理設定画面から、次のタスクも実行できます。

* **[!UICONTROL ユーザーリストのフィルターと並べ替え]**  - Media Portalユーザーのリストをフィルターして、ユーザーを見つけます。

* **[!UICONTROL ユーザーの削除]**  — リストからユーザーを削除します。

* **[!UICONTROL ユーザーのアクティベートとアクティベート解除]**  — フォルダーへのアクセスを停止します。

* **[!UICONTROL ユーザー情報の編集]**  — ユーザーに関する最新の情報を入力します。

* **[!UICONTROL ユーザー定義フィールドの作成]**  - Dynamic Media Classicでのアセットの整理に役立つ、カスタムのユーザー定義メタデータフィールドを作成します。このフィールドは必要に応じて、アクティブ化または非アクティブ化することができます。

[ユーザ定義フィールド](application-setup.md#user_defined_fields)を参照してください。
