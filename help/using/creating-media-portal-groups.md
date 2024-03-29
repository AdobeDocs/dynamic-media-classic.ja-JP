---
title: Media Portal グループの作成と管理
description: Adobe Dynamic Media Classicで Media Portal グループを作成および管理する方法について説明します。
uuid: 23f360e1-ddcb-491b-ab9f-428f3ac9c316
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 91524d36-b77a-4dc4-acba-a7bd85297e98
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: 0deb7133-b895-4c3f-8e5e-8604a6f2d16b
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 54%

---

# Media Portal グループの作成と管理{#creating-and-managing-media-portal-groups}

*グループ*&#x200B;を使用して、Media Portal ユーザを管理することができます。ユーザがアセットにアクセスするには、そのアセットへのアクセス権限を持つ少なくとも 1 つのグループに属している必要があります。ユーザを追加する際、ユーザに 1 つまたは複数のグループを割り当てます。その際には、グループが割り当てられているフォルダーへのアクセス権をユーザーに付与します。 また、グループが使用することができる画像プリセットを選択することもできます。

## グループを使用して、フォルダー、アセットおよび画像プリセットへのアクセスを制限する {#using-groups-to-restrict-access-to-folders-assets-and-image-presets}

異なるレベルにアクセス権限を割り当てるには、グループを作成します。各グループに、様々なフォルダやフォルダ内のアセットに対する読み取り、書き込みおよび削除権限を割り当てます。また、グループが使用することができる画像プリセットも指定します。次に、ユーザをグループに割り当てます。ユーザは、複数のグループに属すことができます。グループの概念によって、全コンテンツの一部のみにアクセスを制限する柔軟性が得られます。

特にアセットまたはフォルダーにグループ権限を付与しない場合、そのアセットまたはフォルダーは、親フォルダー（フォルダー階層内でその上にあるフォルダー）に割り当てた権限を継承します。 親フォルダに権限を付与すると、すべての子フォルダに同じ権限が継承されます。

>[!NOTE]
>
>ユーザは、複数のグループに属すことができます。ユーザが、フォルダへのアクセス権限が異なる 2 つのグループに属している場合、ユーザは最も高いアクセス権が付与されます。

## グループの追加 {#adding-a-group}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal の設定]** > **[!UICONTROL グループ]**.
1. 選択 **[!UICONTROL 追加]**.
1. [ グループの追加 ] ダイアログボックスで、[ グループ名 ] ボックスにグループの名前を入力し、[ **[!UICONTROL グループを追加]**.
1. 必要に応じて、ユーザの名前の横のボックスを選択して、ユーザを新しいグループに追加できます。
1. 今すぐアクセス権限を指定する場合は、 **[!UICONTROL アセットのアクセス権限]** 」タブをクリックし、必要なオプションを指定します。

   詳しくは、[グループのアセットのアクセス権限の設定](creating-media-portal-groups.md#establishing_asset_access_permissions_for_a_group)を参照してください。

1. グループで使用可能な画像プリセットを選択する場合は、「 **[!UICONTROL 画像プリセットのアクセス権限]** 」タブをクリックし、グループが使用できる画像プリセットを選択します。

   詳しくは、[グループの画像プリセットへのアクセス権限の選択](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)を参照してください。

1. 選択 **[!UICONTROL 閉じる]**.

## グループのアセットへのアクセス権限の設定 {#establishing-asset-access-permissions-for-a-group}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal の設定]** > **[!UICONTROL グループ]**.
1. 「グループリスト」ページで、次のいずれかの操作を行います。

   * グループを追加して権限を指定するには、 **[!UICONTROL 追加]**. グループを追加ダイアログボックスで、グループの名前を入力し、「 」を選択します。 **[!UICONTROL グループを追加]**&#x200B;をクリックし、ユーザーをグループに追加します。
   * グループの権限を編集するには、グループを選択し、 **[!UICONTROL 編集]**.

1. グループを追加またはグループを編集ダイアログボックスで、 **[!UICONTROL アセットのアクセス権限]** タブをクリックします。 タブの右側には、フォルダとアセットの読み取り、書き込みおよび削除の権限を設定するためのボックスがあります。左側のパネルでフォルダやサブフォルダを展開したり、折りたたんだりすることができます。
1. フォルダや個々のアセットへの権限を割り当てるには、左側のパネルでフォルダを選択します。フォルダの内容が右側のパネルに表示されます。次に、右側のパネルで、ファイルやフォルダに対応するボックスを選択することで、グループの権限を割り当てます。

   次の表に、各種タスクと、読み取り、書き込み、削除権限との対応を示しています。

   | タスク | 読み取り | 書き込み | 削除 |
   | --- | --- | --- | --- |
   | フォルダとファイルの参照 | X | | |
   | ファイルの編集（切り抜き、シャープ、調整） | | X | |
   | ファイル名の選択変更 | | X | |
   | 別のフォルダへのファイルの移動 | | X | |
   | ファイル名の変更 | | X | |
   | ファイルの削除 | | | X |

1. 選択 **[!UICONTROL 閉じる]**.

>[!NOTE]
>
>ボックスを選択すると、アクセス権限が設定されます。フォルダにアクセス権を割り当てると、そのサブフォルダとその中のすべてのファイルに、親フォルダと同じアクセス権が付与されます。ただし、サブフォルダやアセットファイルごとに異なるアクセス権を指定することもできます。

## グループの画像プリセットへのアクセス権限の選択 {#choosing-image-preset-access-permissions-for-a-group}

グループメンバーが Media Portal でアセットを書き出す際に使用することができる画像プリセットを指定する場合は、グループの画像プリセットのアクセス権限を選択します。

関連トピック [Media Portal ユーザーが使用できる書き出しオプションを指定します](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

**グループの画像プリセットのアクセス権限を選択するには：**

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal の設定]** > **[!UICONTROL グループ]**.
1. 「グループリスト」ページで、次のいずれかの操作を行います。

   * グループを追加し、使用可能な画像プリセットを指定するには、「 **[!UICONTROL 追加]**. グループを追加ダイアログボックスで、グループの名前を入力し、「 」を選択します。 **[!UICONTROL グループを追加]**&#x200B;をクリックし、ユーザーをグループに追加します。
   * グループの画像プリセットオプションを編集するには、グループを選択し、 **[!UICONTROL 編集]**.

1. グループを追加またはグループを編集ダイアログボックスで、 **[!UICONTROL 画像プリセットのアクセス権限]** タブをクリックします。
1. Media Portal ユーザーがアセットの書き出し時に使用できるプリセットを指定するには、「画像プリセット」を選択または選択解除します。
1. 選択 **[!UICONTROL 閉じる]**.

## グループの編集および削除 {#edit-and-delete-groups}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL Media Portal の設定]** > **[!UICONTROL グループ]**.
1. 「グループリスト」ページで、グループを選択し、編集または削除します。

   **グループの編集**  — 選択 **[!UICONTROL 編集]**&#x200B;をクリックし、グループを編集ダイアログボックスでオプションを選択します。

   **グループの削除**  — 選択 **[!UICONTROL 削除]**.
