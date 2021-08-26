---
title: アセットの移動、名前変更、削除
description: AdobeDynamic Media Classicでアセットを移動、名前変更および削除する方法について説明します。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 37%

---

# アセットの移動、名前変更、削除{#moving-renaming-and-deleting-assets}

アセットは、参照パネルで移動、名前の変更および削除が可能です。また、テキストファイルを使用して複数のアセットを同時に削除することもできます。

## アセットの移動 {#move-assets}

参照パネルで、アセットを別のフォルダに移動できます。

1. 参照パネルで 1 つまたは複数のアセットを選択し、次のいずれかの操作を行います。

   * アセットライブラリでアセットの移動先フォルダを表示し、そのフォルダにアセットをドラッグします。
   * **[!UICONTROL ファイル]** > **[!UICONTROL 移動]**&#x200B;に移動し、アセットを移動ウィンドウでフォルダーを選択して、「**[!UICONTROL 移動]**」を選択します。

## アセット名の変更 {#rename-assets}

1. 参照パネルでアセットを選択し、次のいずれかの操作を行います。

   * 名前を選択し、新しい名前を入力して、**[!UICONTROL Enter]**&#x200B;キーを押すか、名前から別の場所を選択します。
   * **[!UICONTROL ファイル]** > **[!UICONTROL 名前を変更]**&#x200B;に移動します。 アセットの名前がハイライトされます。新しい名前を入力し、**[!UICONTROL Enter]**&#x200B;キーを押します。

既存のDynamic Media Classicアセットの名前は入力しないでください。

## アセットの削除 {#delete-assets}

参照パネルで選択したアセットを削除したり、フォルダー全体を削除したりできます。 削除したアセットとフォルダはごみ箱フォルダに移動され、7 日間経過した後に完全に削除されます。

アセットを削除すると、そのアセットから派生したすべてのアセットも削除されます。例えば、ズームターゲットを作成した画像を削除すると、画像とともにズームターゲットも削除されます。

>[!NOTE]
>
>派生元のアセットを削除すると、ズームターゲット、画像属性、およびヒストリーエントリが完全に削除されます。これらはアセットとともにごみ箱フォルダに移動されず、ごみ箱から元に戻すことはできません。

1. 次のいずれかの操作を行います。

   * 1つ以上のアセットを削除するには、参照パネルでアセットを選択し、**[!UICONTROL 削除]**&#x200B;キーを押すか、**[!UICONTROL ファイル]**/**[!UICONTROL 削除]**&#x200B;に移動します。
   * フォルダーを削除するには、アセットライブラリ内のフォルダーを選択し、「**[!UICONTROL フォルダーを削除]**」を選択します。

      フォルダーを削除すると、そのフォルダー、フォルダー内のすべてのアセット、およびそのサブフォルダー内のすべてのアセットが削除されます。

>[!NOTE]
>
>AdobeDynamic Media Classicでは、アセットファイルを削除する理由で同じ名前の別のファイルに置き換える場合は、アセットファイルを削除するのではなく、上書きすることをお勧めします。

## テキストファイルを使用した複数のアセットの削除 {#delete-multiple-assets-with-a-text-file}

アセットライブラリ全体で多数のアセットを一度に削除するには、削除するアセットをテキストファイルにリストし、そのリストをAdobeDynamic Media Classicに送信します。

Dynamic Media Classic IDのAdobeのリストを作成し、テキスト(.txt)ファイルとして保存します。 各AdobeDynamic Media Classic IDは、それぞれ別の行に記述し、その後にハードリターンを記述する必要があります。

リストを作成したら、次の手順に従ってアセットを削除します。

1. **[!UICONTROL File]** > **[!UICONTROL Delete Asset List]**&#x200B;に移動します。
1. アセットリストを削除ダイアログボックスで、削除するアセットのリストが含まれているテキストファイルのパスを参照または入力します。
1. 「**[!UICONTROL 削除]**」を選択します。

テキストファイルを含むAdobeを削除すると、Dynamic Media Classic IDがリストにない場合、「リスト内のこれらのエントリを検証できません：」というメッセージとエントリのリストが表示されます。 ただし、AdobeDynamic Media Classicはジョブページでエラーを生成しません。

>[!MORELIKETHIS]
>
>* [参照パネルでのアセットの選択](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [アップロード用のアセットおよびフォルダーの準備](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [ごみ箱フォルダーからのアセットの復元](trash-folder.md#restoring_assets_from_the_trash_folder)

