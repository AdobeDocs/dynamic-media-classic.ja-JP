---
title: ごみ箱フォルダーを管理します。
description: ごみ箱フォルダーの管理方法を説明します。
uuid: 3992a5b8-1919-4924-b07d-7fb25565effd
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 553c95fc-0a41-4f06-af50-a62bc1438149
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: cffeec19-43fd-4a97-bdcc-df81af108ddd
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 33%

---

# ごみ箱フォルダーを管理します。{#managing-the-trash-folder}

Dynamic Media Classicから削除したAdobeは、ごみ箱フォルダーに移動されます。 削除されたデータは、復元または完全に削除されるまで、7日間このフォルダーに残ります。 アセットライブラリの下部にある&#x200B;**[!UICONTROL ごみ箱]**&#x200B;アイコンをクリックし、ごみ箱フォルダーページの項目を表示して、削除した項目を確認できます。

すべてのユーザは、ごみ箱フォルダ内の項目を元のフォルダに戻すことができます。また、すべてのユーザは、ごみ箱フォルダ内のすべてのコンテンツを空にすることができます。

ごみ箱フォルダーから項目を削除すると、AdobeDynamic Media Classicから項目が完全に削除されます。ごみ箱フォルダから削除されたアイテムは復元できなくなりました。 アセットがごみ箱から自動的に削除される前に会社の管理者に通知するように設定する方法について詳しくは、[アプリケーションの全般設定](application-setup.md#general_settings)を参照してください。

>[!NOTE]
>
>ごみ箱フォルダーに移動されたアセットは、引き続きAdobeDynamic Media Classicに登録されます。 削除したファイルと同じ名前のファイルをごみ箱フォルダーにアップロードしようとすると、AdobeDynamic Media Classicは、アップロードしたいアセットを重複アセットとして扱います。 このため、名前に番号が追加されます。

## ごみ箱フォルダについて {#about-the-trash-folder}

フォルダ内の項目を削除すると、項目がごみ箱フォルダに移動されます。削除され、ごみ箱フォルダに移動された項目は、次のような状態になります。

* 項目はAdobeのDynamic Media Classicフォルダーから削除されていますが、ごみ箱フォルダーに残っている間は、そのIDを別のアセットに割り当てることはできません。 ごみ箱フォルダー内のファイルと同じ名前のアセットをアップロードしようとすると、AdobeDynamic Media Classicによってアセット名に数字が追加されます。
* 項目を公開することはできません。削除したときに項目が公開用にマークされていても、項目は公開されません。
* 項目は、復元されるか、7日経過するか、または誰かが&#x200B;**[!UICONTROL ごみ箱を空にする]**&#x200B;コマンドを選択するまで、ごみ箱フォルダーに残ります。 7 日間経過した後に、自動クリーンアップ操作により項目が完全に削除されます。

## ごみ箱フォルダーからのアセットの復元 {#restoring-assets-from-the-trash-folder}

アセットを削除したユーザーがアセットを復元する必要はありません。誰でも、ごみ箱フォルダーからアセットを復元できます。 復元されたアセットは、削除時にアセットを格納していた元のフォルダに戻されます。これらのフォルダーが存在しなくなった場合は、AdobeDynamic Media Classicによって再作成され、復元されたアセットは再作成されたフォルダーに配置されます。

アセットをごみ箱フォルダーから削除元のフォルダーに復元するには、次の手順を実行します。

1. アセットライブラリパネルの下部で、**[!UICONTROL ごみ箱]**&#x200B;アイコンを選択して、ごみ箱フォルダーを開きます。
1. 復元する 1 つまたは複数のアセットを選択します。
1. **[!UICONTROL ファイル]** > **[!UICONTROL ごみ箱から復元]**&#x200B;に移動します。

## ごみ箱フォルダ内のアセットの完全な削除 {#permanently-deleting-assets-in-the-trash-folder}

ごみ箱フォルダ内のアセットを削除すると、アセットは完全に削除されます。また、7 日間が経過すると、自動的にごみ箱フォルダから削除されます。

ごみ箱フォルダーからアセットを完全に削除するには、**[!UICONTROL ごみ箱]**&#x200B;アイコンを選択します。 ごみ箱フォルダーページで、次のいずれかの操作を行います。

* **個々のアセットの削除**  — 完全に削除するアセットを選択し、ファイ **[!UICONTROL ル]** / **[!UICONTROL ごみ箱から空にする]**&#x200B;に移動します。

* **すべてのアセットの削除**  — ファ **[!UICONTROL イル]** / **[!UICONTROL 空のごみ箱]**&#x200B;に移動します。

>[!MORELIKETHIS]
>
>* [アセットの削除](moving-renaming-deleting-assets.md#delete_assets)

