---
title: アセットの移動、名前変更、削除
seo-title: アセットの移動、名前変更、削除
description: 'null'
seo-description: アセットの移動、名前の変更および削除の方法について説明します。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 66%

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

既存のダイナミックメディアクラシックアセットの名前は入力しないでください。

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
>アセットファイルを同じ名前の別のファイルで置き換える場合、アセットファイルを削除するのではなく、上書きすることをお勧めします。

## テキストファイルを使用した複数のアセットの削除 {#delete-multiple-assets-with-a-text-file}

アセットライブラリ全体で一度に複数のアセットを削除するには、削除するアセットをテキストファイルでリストし、そのリストをDynamic Media Classicに送信します。

Dynamic Media Classic IDのリストを作成し、テキスト(.txt)ファイルとして保存します。 各Dynamic Media Classic IDは、それぞれ独自の行に記述し、末尾で改行する必要があります。

リストを作成したら、次の手順に従ってアセットを削除します。

1. ファイル／アセットリストを削除
1. アセットリストを削除ダイアログボックスで、削除するアセットのリストが含まれたテキストファイルを参照して選択するか、テキストファイルへのパスを入力します。
1. 「削除」ボタンをクリックします。

テキストファイルを含むアセットを削除する際に、Dynamic Media Classic IDがリストにない場合は、Dynamic Media Classicが「リストー内の次のエントリを検証できません：」であることと、エントリのリストを示すメッセージが表示されます。 ただし、Dynamic Media Classicはジョブ画面でエラーを生成しません。

>[!MORELIKETHIS]
>
>* [参照パネルでのアセットの選択](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [アセットおよびフォルダのアップロードの準備](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [ごみ箱フォルダからのアセットの復元](trash-folder.md#restoring_assets_from_the_trash_folder)

