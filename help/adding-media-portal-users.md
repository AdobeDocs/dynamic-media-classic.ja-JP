---
title: Media Portal のユーザの追加と管理
seo-title: Media Portal のユーザの追加と管理
description: 'null'
seo-description: Media Portalユーザを追加および管理する方法について説明します。
uuid: 96d4103c-6428-4ce1-b9e4-231599304f27
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 5e933045-ce1a-41b9-ba8b-2151c396b7a2
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 84%

---


# Media Portal のユーザの追加と管理{#adding-and-managing-media-portal-users}

管理者は、ユーザの追加と管理、ユーザによるパスワードの変更を許可するかどうかの指定、ユーザ情報の編集、ユーザリストのアップロードを実行できます。これらのタスクは、ユーザ管理画面で実行されます。この画面にアクセスするには、**設定**／**アプリケーション設定**&#x200B;をクリックし、**「管理設定」**&#x200B;で、**「ユーザ管理」**&#x200B;をクリックします。

>[!NOTE]
>
>ユーザを追加する前に、ユーザを管理するためのグループを設定します。Media Portal では、ユーザを 1 つまたは複数のグループに割り当てないと、ユーザを追加できません。詳しくは、[Media Portal グループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)を参照してください。

## Media Portal のパスワードの処理 {#handling-media-portal-passwords}

Media Portal ユーザ、寄稿者、寄稿者ユーザをサインアップしたときに、それらのユーザにパスワードが記載されたご案内の電子メールが送信されます。管理者は、Media Portal ユーザがこのパスワードを変更できるようにするかどうかを指定できます。

1. **設定**／**Media Portal 設定**／**全般設定**&#x200B;をクリックします。
1. 全般設定ページで、**「Media Portal ユーザによるパスワードの変更を許可」**&#x200B;オプションを選択または選択解除します。
1. **「保存」**&#x200B;をクリックします。

>[!NOTE]
>
>パスワードの変更が許可された Media Portal ユーザは、**設定**／**個人設定**&#x200B;を選択して、個人設定画面でパスワードを変更することができます。

## Media Portal ユーザの追加 {#adding-a-media-portal-user}

1. **設定**／**アプリケーション設定**／**管理設定**／**ユーザ管理**&#x200B;をクリックします。
1. ユーザ管理ページで、**「追加」**&#x200B;をクリックします。
1. ユーザを追加ダイアログボックスのユーザ情報パネルで、ユーザの名、姓、および電子メールアドレスを入力し、**「次へ」**&#x200B;をクリックします。
1. 会社 / 役割パネルの会社ドロップダウンリストで、ユーザの会社を選択します。
1. 役割リストで、Media Portal 役割を選択し、**次へ**&#x200B;をクリックします。

   詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

1. アクセスグループパネルで、1 つまたは複数のグループを選択します。

   詳しくは、[Media Portal グループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)を参照してください。

1. （オプション）**「電子メール設定」**&#x200B;をクリックして、初期設定とは異なる電子メール設定を選択します。

   [Media Portal ユーザ向けのご案内の電子メールメッセージの設定](adding-media-portal-users.md#setting_up_the_welcome_e_mail_message_for_media_portal_users)を参照してください。

1. **「ユーザを追加」**&#x200B;をクリックします。

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
| ユーザの役割 | Media PortalAdminMediaPortalUserMediaPortalContributorMediaPortalContributorContributorUser |
| グループ | 各ユーザの 1 つまたは複数のアカウントグループ割り当てをカンマで区切ったリストです。アカウント名にプリフィックスを付け、スラッシュ（/）で区切ることで、グループを指定します。例えば、PortalCo/IT の場合、PortalCo はアカウント、IT は PortalCo アカウント内のグループです。 |

次のサンプルスプレッドシートで、CSV ファイルのレイアウト方法の例を示します。

| 名 | 姓 | 電子メール | パスワード | ユーザの役割 | グループ |
|--- |--- |--- |--- |--- |--- |
| Peter | Peterson | `petep@company.com` | welcome | MediaPortal 管理者 | PortalCo/IT,PortalCo/Admin |
| Kevin | Marks | `kevinm@myco.com` | welcome | Media Portal ユーザ | PortalCo/MktgGroup, PortalCo/test |


### CSV ファイルのアップロード {#uploading-the-csv-file}

1. ユーザ管理設定画面を開きます。
1. **ユーザリストをアップロード**&#x200B;をクリックします。
1. アップロードするファイルを選択しますダイアログボックスで CSV ファイルを選択し、**「開く」**&#x200B;をクリックします。

リスト内の各ユーザが、指定されているグループに自動的に追加されます。追加を通知する電子メールメッセージが各ユーザに送信されます。

>[!NOTE]
CSV ファイルの形式が正しくなかった場合は、次のエラーメッセージが表示されます。「アップロードした CSV ファイルの処理中にエラーが発生しました。ファイルの内容を調べて、データが有効であることを確認してください。」また、CSV に既存の IP または IPS ユーザが含まれていた場合、そのユーザはユーザリストに追加されません。

## 選択可能な Media Portal ユーザリストの生成 {#generating-a-selectable-list-of-media-portal-users}

Media Portal ユーザの名前と電子メールアドレスをポップアップウィンドウに表示できます。このリストは、ユーザ名とアドレスを Media Portal 以外で使用するためにカットおよびペーストする場合に便利です。

1. **設定**／**アプリケーション設定**／**管理設定**／**ユーザ管理**&#x200B;をクリックします。
1. **「ユーザの役割が」**&#x200B;ドロップダウンリストで、Media Portal ユーザの役割名を選択し、**「更新」**&#x200B;をクリックして、Media Portal ユーザの 1 つのクラスの名前のみを表示します。
1. **「ポップアップリスト」**&#x200B;をクリックすると、ポップアップウィンドウが開きます。このリストをコピーしてペーストできます。

## Media Portal ユーザ向けのご案内の電子メールメッセージの設定 {#setting-up-the-welcome-e-mail-message-for-media-portal-users}

新規 Media Portal ユーザ、寄稿者、寄稿者ユーザを追加する際に、ご案内の電子メールを送信できます。この電子メールメッセージを設定するか、ClassicDynamic Mediaに送信しないように設定できます。

1. **設定**／**アプリケーション設定**／**管理設定**／**ユーザ管理**&#x200B;を選択します。
1. In the User Administration Setup screen, click **Email Settings**.
1. 電子メール設定ダイアログボックスで、次のいずれかの設定を指定します。

   **電子メールを送信** 新しいユーザーにサインアップが完了したことを電子メールで通知しない場合は、このオプションの選択を解除します。

   **デフォルトのパスワード** 新規ユーザーの一時パスワードを入力するか、フィールドを空のままにしてDynamic Mediaクラシックでランダムなパスワードを生成するようにします。 ユーザは、初めてログインしたときにパスワードを変更するように指示されます。

   **置換URL** ：ユーザーが別のURLを使用してDynamic MediaClassicにアクセスする場合、デフォルトとは異なるURLを入力します。

## その他のユーザ管理タスク {#other-user-management-tasks}

ユーザ管理設定画面から、次のタスクも実行できます。

**ユーザリストのフィルタリングと並べ替え** Media Portalユーザのリストをフィルタして、ユーザを探します。 詳しくは、ユーザリストのフィルタリングと並べ替えを参照してください。

**ユーザーの削除** リストからユーザーを削除します。 詳しくは、ユーザの削除を参照してください。

**ユーザーのアクティブ化と非アクティブ化** ：ユーザーによるフォルダーへのアクセスを停止します。 詳しくは、ユーザのアクティブ化と非アクティブ化を参照してください。

**ユーザー情報の編集** ：ユーザーに関する最新の情報を入力します。 詳しくは、ユーザ情報の編集を参照してください。

**ユーザ定義フィールドの作成** ClassicDynamic Media内のアセットを整理するのに役立つ、ユーザ定義のカスタムメタデータフィールドを作成します。 このフィールドは必要に応じて、アクティブ化または非アクティブ化することができます。

[ユーザ定義フィールド](application-setup.md#user_defined_fields)を参照してください。
