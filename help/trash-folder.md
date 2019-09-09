---
title: ごみ箱フォルダの管理
seo-title: ごみ箱フォルダの管理
description: 'null'
seo-description: ごみ箱フォルダを管理する方法について説明します。
uuid: 3992a5b8-1919-4924- b07d-7fb25565efd
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/managing_ assets
discoiquuid: 553c95fc-0a41-4f06- af50- a62bc1438149
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# ごみ箱フォルダの管理{#managing-the-trash-folder}

Scene7 Publishing System から削除した項目は、ごみ箱フォルダへ移動されます。これらの項目は、復元されるか完全に削除されない限り、このフォルダに 7 日間残ります。アセットライブラリの下部にあるごみ箱アイコン  を選択し、ごみ箱フォルダ内の項目を参照して、削除した項目を確認できます。

すべてのユーザは、ごみ箱フォルダ内の項目を元のフォルダに戻すことができます。また、すべてのユーザは、ごみ箱フォルダ内のすべてのコンテンツを空にすることができます。

ごみ箱フォルダから項目を削除すると、項目が Scene7 Publishing System から完全に削除されます。ごみ箱フォルダから削除した項目を元に戻すことはできません。アセットがごみ箱から自動的に削除される前に会社の管理者に通知するように設定する方法について詳しくは、[アプリケーションの全般設定](application-setup.md#general_settings)を参照してください。

>[!NOTE]
>
>ごみ箱フォルダに移動されたアセットは、Scene7 Publishing System に登録されたままになります。ごみ箱フォルダ内の削除されたファイルと同じ名前のファイルをアップロードしようとすると、アップロードするアセットと同じアセットがDynamic Media Classicで処理されます。このため、名前に番号が追加されます。

## ごみ箱フォルダについて {#about-the-trash-folder}

フォルダ内の項目を削除すると、項目がごみ箱フォルダに移動されます。削除され、ごみ箱フォルダに移動された項目は、次のような状態になります。

* 項目は Scene7 Publishing System のフォルダから削除されますが、それがごみ箱フォルダに残っている間は、その ID を別のアセットに割り当てることはできません。ごみ箱フォルダ内のファイルと同じ名前のアセットをアップロードしようとすると、アセット名に数字が追加されます。
* 項目を公開することはできません。削除したときに項目が公開用にマークされていても、項目は公開されません。
* 項目は、復元するか、7 日間経過するかまたはいずれかのユーザがごみ箱を空にするコマンドを選択するまでごみ箱フォルダに残ります。7 日間経過した後に、自動クリーンアップ操作により項目が完全に削除されます。

## ごみ箱フォルダからのアセットの復元 {#restoring-assets-from-the-trash-folder}

アセットの復元は、アセットを削除したユーザが行う必要はありません。すべてのユーザがごみ箱フォルダからアセットを復元できます。復元されたアセットは、削除時にアセットを格納していた元のフォルダに戻されます。これらのフォルダが存在しなくなった場合は、Scene7 Publishing System はこれらを再作成し、復元されたアセットはこれらの再作成されたフォルダに配置されます。

アセットをごみ箱フォルダから、削除時にアセットを格納していたフォルダに戻すには、次の手順に従います。

1. ごみ箱アイコンをクリックしてごみ箱フォルダを開きます。
1. 復元する 1 つまたは複数のアセットを選択します。
1. ファイル／ごみ箱から復元を選択します。

## ごみ箱フォルダ内のアセットの完全な削除 {#permanently-deleting-assets-in-the-trash-folder}

ごみ箱フォルダ内のアセットを削除すると、アセットは完全に削除されます。また、7 日間が経過すると、自動的にごみ箱フォルダから削除されます。

ごみ箱フォルダからアセットを完全に削除するには、ごみ箱アイコン  を選択してごみ箱フォルダを開きます。次に、次の手順に従って、個別のアセットまたはフォルダ内のすべてのアセットを削除します。

**個別のアセット** を削除削除するアセットを選択し、ファイル/ごみ箱から空にするをクリックします。

**すべてのアセット** を削除するには、ファイル/ごみ箱を空にするをクリックします。

>[!MORELIKETHIS]
>
>* [アセットの削除](moving-renaming-deleting-assets.md#delete_assets)
