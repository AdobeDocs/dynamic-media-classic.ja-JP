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
autotag-review: '2026-05-13T20:15:24.015Z'
TQID: 'https://experienceleague.adobe.com/5XOu6T0n7zssUzXgQXushja4DJBSHs8-0-2h2Ao1L20'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 563
ht-degree: 28%

---

# ごみ箱フォルダーの管理{#managing-the-trash-folder}

Adobe Dynamic Media Classicから削除したアイテムは、ごみ箱フォルダーに移動されます。 これらの削除されたアイテムは、復元または完全に削除されるまで、このフォルダーに7日間残ります。 アセットライブラリの下部にある「**[!UICONTROL ゴミ箱]**」アイコンを選択し、ごみ箱フォルダーページでアイテムを表示することで、削除されたアイテムを調べることができます。

すべてのユーザは、ごみ箱フォルダ内の項目を元のフォルダに戻すことができます。 また、すべてのユーザは、ごみ箱フォルダ内のすべてのコンテンツを空にすることができます。

ごみ箱フォルダーからアイテムを削除すると、Adobe Dynamic Media Classicからアイテムが完全に削除されます。ごみ箱フォルダーから削除されたアイテムは復元できなくなります。 アセットがごみ箱から自動的に削除される前に会社の管理者に通知するように設定する方法について詳しくは、[アプリケーションの全般設定](application-setup.md#general_settings)を参照してください。

>[!NOTE]
>
>ごみ箱フォルダーに移動されたAssetsは、Adobe Dynamic Media Classicに登録されたままです。 例えば、削除したファイルと同じ名前のファイルをごみ箱フォルダーにアップロードするとします。 Adobe Dynamic Media Classicは、アップロードするアセットを重複アセットとして扱います。 この場合は、名前に数字が付加されます。

## ごみ箱フォルダについて {#about-the-trash-folder}

フォルダ内の項目を削除すると、項目がごみ箱フォルダに移動されます。 削除され、ごみ箱フォルダに移動された項目は、次のような状態になります。

* アイテムはAdobe Dynamic Media Classic フォルダーから削除されますが、ごみ箱フォルダーに残っている間はIDを別のアセットに割り当てることはできません。 ゴミ箱フォルダー内のファイルと同じ名前のアセットをアップロードしようとすると、Adobe Dynamic Media Classicはアセット名に数字を追加します。
* 項目を公開することはできません。 削除したときに項目が公開用にマークされていても、項目は公開されません。
* アイテムが復元されるか、7日が経過するか、誰かが&#x200B;**[!UICONTROL ごみ箱]** コマンドを空にするまで、アイテムはゴミ箱フォルダーに残ります。 7 日間経過した後に、自動クリーンアップ操作により項目が完全に削除されます。

## ごみ箱フォルダーからのアセットの復元 {#restoring-assets-from-the-trash-folder}

アセットを削除したユーザーがアセットを復元する必要はありません。誰でもゴミ箱フォルダーからアセットを復元できます。 復元されたアセットは、削除時にアセットを格納していた元のフォルダに戻されます。 これらのフォルダーが存在しなくなった場合、Adobe Dynamic Media Classicはフォルダーを再作成し、復元されたアセットは再作成されたフォルダーに配置されます。

アセットをゴミ箱フォルダーから削除されたフォルダーに復元するには、次の操作を行います。

1. アセットライブラリパネルの下部にある「**[!UICONTROL ごみ箱]**」アイコンを選択して、ごみ箱フォルダーを開きます。
1. 復元するアセットを選択します。
1. **[!UICONTROL ファイル]** > **[!UICONTROL ごみ箱からの復元]**&#x200B;に移動します。

## ごみ箱フォルダ内のアセットの完全な削除 {#permanently-deleting-assets-in-the-trash-folder}

ごみ箱フォルダ内のアセットを削除すると、アセットは完全に削除されます。 また、7 日間が経過すると、自動的にごみ箱フォルダから削除されます。

**[!UICONTROL ごみ箱]** アイコンを選択すると、ごみ箱フォルダーからアセットを完全に削除できます。 ごみ箱フォルダーページで、次のいずれかの操作を行います。

* **個々のアセットを削除しています**: アセットを完全に削除できます。 必要なアセットを選択し、**[!UICONTROL ファイル]**/**[!UICONTROL ゴミ箱から空にする]**&#x200B;をクリックします。

* **すべてのアセットを削除**: **[!UICONTROL ファイル]** > **[!UICONTROL 空のゴミ箱]**&#x200B;に移動します。

>[!MORELIKETHIS]
>
>* [ アセットの削除](moving-renaming-deleting-assets.md#delete_assets)
