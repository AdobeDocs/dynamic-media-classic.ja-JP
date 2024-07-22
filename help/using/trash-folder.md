---
title: ごみ箱フォルダーの管理
description: ごみ箱フォルダーの管理方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 28%

---

# ごみ箱フォルダーの管理{#managing-the-trash-folder}

Adobe Dynamic Media Classicから削除した項目は、ごみ箱フォルダーに移動されます。 これらの削除されたアイテムは、復元されるか完全に削除されるまで、7 日間このフォルダーに残ります。 削除された項目を調べるには、アセットライブラリの下部にある **[!UICONTROL ごみ箱]** アイコンを選択し、ごみ箱フォルダーページで項目を表示します。

すべてのユーザは、ごみ箱フォルダ内の項目を元のフォルダに戻すことができます。また、すべてのユーザは、ごみ箱フォルダ内のすべてのコンテンツを空にすることができます。

ごみ箱フォルダーからアイテムを削除すると、Adobe Dynamic Media Classicからアイテムが完全に削除されます。ごみ箱フォルダーから削除されたアイテムは復元できなくなります。 アセットがごみ箱から自動的に削除される前に会社の管理者に通知するように設定する方法について詳しくは、[アプリケーションの全般設定](application-setup.md#general_settings)を参照してください。

>[!NOTE]
>
>ごみ箱フォルダーに移動されたAssetsは、引き続きAdobe Dynamic Media Classicに登録されます。 例えば、削除したファイルと同じ名前のファイルをごみ箱フォルダーにアップロードするとします。 Adobe Dynamic Media Classicはアップロードするアセットを重複したアセットとして扱います。 この場合は、名前に数字が付加されます。

## ごみ箱フォルダについて {#about-the-trash-folder}

フォルダ内の項目を削除すると、項目がごみ箱フォルダに移動されます。削除され、ごみ箱フォルダに移動された項目は、次のような状態になります。

* 項目はAdobe Dynamic Media Classic フォルダーから削除されますが、ごみ箱フォルダー内に残っている間は、その ID を別のアセットに割り当てることはできません。 ごみ箱フォルダー内のファイルと同じ名前のアセットをアップロードしようとすると、Adobe Dynamic Media Classicによってアセットの名前に数字が追加されます。
* 項目を公開することはできません。削除したときに項目が公開用にマークされていても、項目は公開されません。
* 項目は、復元されるか、7 日経過するか、誰かが **[!UICONTROL ごみ箱を空にする]** コマンドを選択するまで、ごみ箱フォルダーに残ります。 7 日間経過した後に、自動クリーンアップ操作により項目が完全に削除されます。

## ごみ箱フォルダーからのアセットの復元 {#restoring-assets-from-the-trash-folder}

アセットを削除したユーザーはアセットを復元する必要はありません。誰でもごみ箱フォルダーからアセットを復元できます。 復元されたアセットは、削除時にアセットを格納していた元のフォルダに戻されます。これらのフォルダーが存在しない場合、Adobe Dynamic Media Classicはフォルダーを再作成し、復元されたアセットは再作成されたフォルダーに配置されます。

ごみ箱フォルダーのアセットを削除済みフォルダーに復元するには、次の手順を実行します。

1. アセットライブラリパネルの下部にある **[!UICONTROL ごみ箱]** アイコンを選択して、ごみ箱フォルダーを開きます。
1. 復元するアセットを 1 つ以上選択します。
1. **[!UICONTROL ファイル]**/**[!UICONTROL ごみ箱から復元]** に移動します。

## ごみ箱フォルダ内のアセットの完全な削除 {#permanently-deleting-assets-in-the-trash-folder}

ごみ箱フォルダ内のアセットを削除すると、アセットは完全に削除されます。また、7 日間が経過すると、自動的にごみ箱フォルダから削除されます。

アセットをごみ箱フォルダーから完全に削除するには、「**[!UICONTROL ごみ箱]** アイコンを選択します。 ごみ箱フォルダーページで、次のいずれかの操作を行います。

* **個々のアセットの削除**：アセットを完全に削除できます。 必要なアセットを選択し、**[!UICONTROL ファイル]**/**[!UICONTROL ごみ箱から空にする]** をクリックします。

* **すべてのアセットを削除**: **[!UICONTROL ファイル]**/**[!UICONTROL ごみ箱を空にする]** に移動します。

>[!MORELIKETHIS]
>
>* [ アセットの削除 ](moving-renaming-deleting-assets.md#delete_assets)
