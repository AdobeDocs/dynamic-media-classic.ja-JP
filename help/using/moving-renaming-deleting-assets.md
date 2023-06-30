---
title: アセットの移動、名前変更、削除
description: Adobe Dynamic Media Classicでアセットを移動、名前変更および削除する方法について説明します。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 31%

---

# アセットの移動、名前変更、削除{#moving-renaming-and-deleting-assets}

アセットは、参照パネルで移動、名前の変更および削除が可能です。また、テキストファイルを使用して複数のアセットを同時に削除することもできます。

## アセットの移動 {#move-assets}

参照パネルで、アセットを別のフォルダに移動できます。

**アセットを移動するには：**

1. 参照パネルで 1 つまたは複数のアセットを選択し、次のいずれかの操作を行います。

   * アセットライブラリ内のアセットの移動先のフォルダーを表示し、そのフォルダーにアセットをドラッグします。
   * に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 移動]**&#x200B;をクリックし、アセットを移動ウィンドウでフォルダーを選択し、「 **[!UICONTROL 移動]**.

## アセット名の変更 {#rename-assets}

1. 参照パネルでアセットを選択し、次のいずれかの操作を行います。

   * 名前を選択し、新しい名前を入力して、 **[!UICONTROL 入力]** または、名前から別の名前を選択します。
   * に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 名前を変更]**. アセットの名前がハイライトされます。新しい名前を入力し、 **[!UICONTROL 入力]**. 既存のAdobe Dynamic Media Classicアセットの名前を入力しないでください。

## アセットの削除 {#delete-assets}

参照パネルで選択したアセットを削除したり、フォルダー全体を削除したりできます。 削除したアセットとフォルダはごみ箱フォルダに移動され、7 日間経過した後に完全に削除されます。

アセットを削除すると、そのアセットから派生したすべてのアセットも削除されます。例えば、ズームターゲットを作成した画像を削除すると、画像とともにズームターゲットも削除されます。

派生元のアセットを削除すると、ズームターゲット、画像属性、およびヒストリーエントリが完全に削除されます。これらはアセットとともにごみ箱フォルダに移動されず、ごみ箱から元に戻すことはできません。

>[!IMPORTANT]
>
>一括削除は大量の操作です。 一括削除は、同時に大量の削除操作としてではなく、順番に実行してください。 Adobeでは、削除操作を、1 時間あたり 5000 個以下のアセット削除に制限することをお勧めします。 1 時間に 5000 を超える数を指定すると、レートが制限される場合があります。

**アセットを削除するには：**

1. 次のいずれかの操作を行います。

   * 1 つ以上のアセットを削除するには、参照パネルでアセットを選択し、 **[!UICONTROL 削除]** または **[!UICONTROL ファイル]** > **[!UICONTROL 削除]**.
   * フォルダーを削除するには、アセットライブラリでフォルダーを選択し、 **[!UICONTROL フォルダーを削除]**.

     フォルダーを削除すると、そのフォルダー、フォルダー内のすべてのアセット、およびサブフォルダー内のすべてのアセットが削除されます。

Adobe Dynamic Media Classicでは、アセットファイルを削除する理由で同じ名前の別のファイルに置き換える場合は、アセットファイルを削除するのではなく、上書きすることをお勧めします。

## テキストファイルを使用した複数のアセットの削除 {#delete-multiple-assets-with-a-text-file}

アセットライブラリ全体で多数のアセットを一度に削除するには、削除するアセットをテキストファイルにリストし、そのリストをAdobe Dynamic Media Classicに送信します。

Adobe Dynamic Media Classic ID のリストを作成し、テキスト (.txt) ファイルとして保存します。 各Adobe Dynamic Media Classic ID は、それぞれ別の行に記述し、その後にハードリターンを記述する必要があります。

リストを作成したら、次の手順に従ってアセットを削除します。

1. に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL アセットリストを削除]**.
1. アセットリストを削除ダイアログボックスで、削除するアセットのリストが含まれるテキストファイルのパスを参照または入力します。
1. 選択 **[!UICONTROL 削除]**.

テキストファイルを持つアセットを削除すると、Adobe Dynamic Media Classic ID がリストにない場合は、「リスト内のこれらのエントリを検証できません：」というメッセージが表示されます。 エントリのリストも表示されます。 ただし、Adobe Dynamic Media Classicはジョブページでエラーを生成しません。

>[!MORELIKETHIS]
>
>* [参照パネルでのアセットの選択](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [アップロード用のアセットおよびフォルダーの準備](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [ごみ箱フォルダーからアセットを復元](trash-folder.md#restoring_assets_from_the_trash_folder)
