---
title: ごみ箱フォルダーを管理
description: ごみ箱フォルダーの管理方法を説明します。
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 31%

---

# ごみ箱フォルダーを管理{#managing-the-trash-folder}

Adobe Dynamic Media Classicから削除した項目はごみ箱フォルダーに移動されます。 削除された項目は、復元または完全に削除されるまで、7 日間このフォルダに残ります。 削除した項目を確認するには、 **[!UICONTROL ごみ箱]** アセットライブラリの下部にあるアイコンをクリックし、ごみ箱フォルダページの項目を表示します。

すべてのユーザは、ごみ箱フォルダ内の項目を元のフォルダに戻すことができます。また、すべてのユーザは、ごみ箱フォルダ内のすべてのコンテンツを空にすることができます。

ごみ箱フォルダーから項目を削除すると、Adobe Dynamic Media Classicから項目が完全に削除されます。ごみ箱フォルダから削除された項目は復元できなくなりました。 アセットがごみ箱から自動的に削除される前に会社の管理者に通知するように設定する方法について詳しくは、[アプリケーションの全般設定](application-setup.md#general_settings)を参照してください。

>[!NOTE]
>
>ごみ箱フォルダーに移動されたアセットは、引き続きAdobe Dynamic Media Classicに登録されます。 ごみ箱フォルダー内の削除済みファイルと同じ名前のファイルをアップロードしようとすると、Adobe Dynamic Media Classicはアップロードしたいアセットを重複アセットとして扱います。 このため、名前に番号が追加されます。

## ごみ箱フォルダについて {#about-the-trash-folder}

フォルダ内の項目を削除すると、項目がごみ箱フォルダに移動されます。削除され、ごみ箱フォルダに移動された項目は、次のような状態になります。

* 項目はAdobe Dynamic Media Classicフォルダーから削除されていますが、ごみ箱フォルダー内に残っている間は、その ID を別のアセットに割り当てることはできません。 ごみ箱フォルダー内のファイルと同じ名前のアセットをアップロードしようとすると、Adobe Dynamic Media Classicによってアセット名に数字が追加されます。
* 項目を公開することはできません。削除したときに項目が公開用にマークされていても、項目は公開されません。
* 項目は、復元されるか、7 日が経過するか、誰かが **[!UICONTROL ごみ箱を空にする]** コマンドを使用します。 7 日間経過した後に、自動クリーンアップ操作により項目が完全に削除されます。

## ごみ箱フォルダーからアセットを復元 {#restoring-assets-from-the-trash-folder}

アセットを削除したユーザーがアセットを復元する必要はありません。ごみ箱フォルダーから誰でもアセットを復元できます。 復元されたアセットは、削除時にアセットを格納していた元のフォルダに戻されます。これらのフォルダーが存在しなくなった場合、Adobe Dynamic Media Classicはそれらを再作成し、復元されたアセットは再作成されたフォルダーに配置されます。

ごみ箱フォルダー内のアセットを削除元のフォルダーに復元するには、次の操作を行います。

1. アセットライブラリパネルの下部で、 **[!UICONTROL ごみ箱]** アイコンをクリックしてごみ箱フォルダーを開きます。
1. 復元する 1 つ以上のアセットを選択します。
1. に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL ごみ箱から復元]**.

## ごみ箱フォルダ内のアセットの完全な削除 {#permanently-deleting-assets-in-the-trash-folder}

ごみ箱フォルダ内のアセットを削除すると、アセットは完全に削除されます。また、7 日間が経過すると、自動的にごみ箱フォルダから削除されます。

ごみ箱フォルダーからアセットを完全に削除するには、 **[!UICONTROL ごみ箱]** アイコン ごみ箱フォルダーページで、次のいずれかの操作をおこないます。

* **個々のアセットの削除**  — 完全に削除するアセットを選択し、次に移動します： **[!UICONTROL ファイル]** > **[!UICONTROL ごみ箱から空にする]**.

* **すべてのアセットの削除**  — に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL ごみ箱を空にする]**.

>[!MORELIKETHIS]
>
>* [アセットの削除](moving-renaming-deleting-assets.md#delete_assets)
