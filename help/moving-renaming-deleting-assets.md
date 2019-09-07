---
title: アセットの移動、名前変更、削除
seo-title: アセットの移動、名前変更、削除
description: 'null'
seo-description: アセットの移動、名前の変更および削除方法について説明します。
uuid: deff6521-0ad0-4db9- b4e0- e3211ff97740
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/managing_ assets
discoiquuid: 1c9e29f0-3083-4d22- a439-2a01faf59683
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# アセットの移動、名前変更、削除{#moving-renaming-and-deleting-assets}

アセットは、参照パネルで移動、名前の変更および削除が可能です。また、テキストファイルを使用して複数のアセットを同時に削除することもできます。

## アセットの移動 {#move-assets}

参照パネルで、アセットを別のフォルダに移動できます。

1. 参照パネルで 1 つまたは複数のアセットを選択し、次のいずれかの操作を行います。

   * アセットライブラリでアセットの移動先フォルダを表示し、そのフォルダにアセットをドラッグします。
   * ファイル／移動を選択し、アセットの移動ウィンドウでフォルダを選択して、「移動」を選択します。

## アセット名の変更 {#rename-assets}

アセットの名前を変更するには、次の手順に従います。

1. 参照パネルでアセットを選択し、次のいずれかの操作を行います。

   * 名前を選択し、新しい名前を入力して、Enter キーを押すか、名前以外の箇所をクリックします。
   * ファイル／名前変更を選択します。アセットの名前がハイライトされます。新しい名前を入力して、Enter キーを押します。

既存の Scene7 Publishing System アセットの名前を入力しないようにしてください。

## アセットの削除 {#delete-assets}

参照パネルで選択したアセットを削除したり、フォルダ全体を削除することができます。削除したアセットとフォルダはごみ箱フォルダに移動され、7 日間経過した後に完全に削除されます。

アセットを削除すると、そのアセットから派生したすべてのアセットも削除されます。例えば、ズームターゲットを作成した画像を削除すると、画像とともにズームターゲットも削除されます。

>[!NOTE]
>
>派生元のアセットを削除すると、ズームターゲット、画像属性、およびヒストリーエントリが完全に削除されます。これらはアセットとともにごみ箱フォルダに移動されず、ごみ箱から元に戻すことはできません。

1. 次のいずれかの操作を行います。

   * 1 つまたは複数のアセットを削除するには、参照パネルでアセットを選択し、Delete キーを押すか、ファイル／削除を選択します。
   * To delete a folder, select the folder in the Asset Library, and click **Remove Folder**.

      フォルダを削除すると、フォルダ自体と、フォルダおよびサブフォルダ内のすべてのアセットが削除されます。

>[!NOTE]
>
>アセットファイルを削除する理由が同じ名前で別のアセットファイルに置き換える場合は、アセットファイルを削除する代わりに、アセットファイルを上書きすることをお勧めします。

## テキストファイルを使用した複数のアセットの削除 {#delete-multiple-assets-with-a-text-file}

To delete many assets at once throughout the Asset Library, you can list the assets you want to delete in a text file and submit the list to Dynamic Media Classic.

Scene7 Publishing System ID のリストを作成して、テキストファイル（.txt）として保存します。各 Scene7 Publishing System ID は、個別の行に記述され、末尾で改行されている必要があります。

リストを作成したら、次の手順に従ってアセットを削除します。

1. ファイル／アセットリストを削除
1. アセットリストを削除ダイアログボックスで、削除するアセットのリストが含まれたテキストファイルを参照して選択するか、テキストファイルへのパスを入力します。
1. 「削除」ボタンをクリックします。

テキストファイルを使用してアセットを削除すると、Scene7Publishing System IDがリストにない場合、Dynamic Media Classicが「リスト内のこれらのエントリを検証できません」というメッセージを表示することができます。」を入力します。

>[!MORELIKETHIS]
>
>* [参照パネルでのアセットの選択](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [アセットおよびフォルダのアップロードの準備](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [ごみ箱フォルダからのアセットの復元](trash-folder.md#restoring_assets_from_the_trash_folder)

