---
title: アセットの移動、名前変更、削除
description: アセットの移動、名前の変更および削除の方法について説明します。
uuid: deff6521-0ad0-4db9-b4e0-e3211ff97740
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: 1c9e29f0-3083-4d22-a439-2a01faf59683
feature: Dynamic Mediaクラシック，アセット管理
role: Business Practitioner
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
translation-type: tm+mt
source-git-commit: 38d09bb78834c6b3614bf2b96fd6aee5661e0a5a
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 44%

---

# アセットの移動、名前変更、削除{#moving-renaming-and-deleting-assets}

アセットは、参照パネルで移動、名前の変更および削除が可能です。また、テキストファイルを使用して複数のアセットを同時に削除することもできます。

## アセットの移動 {#move-assets}

参照パネルで、アセットを別のフォルダに移動できます。

1. 参照パネルで 1 つまたは複数のアセットを選択し、次のいずれかの操作を行います。

   * アセットライブラリでアセットの移動先フォルダを表示し、そのフォルダにアセットをドラッグします。
   * **[!UICONTROL ファイル]**/**[!UICONTROL 移動]**&#x200B;をクリックし、アセットの移動ウィンドウでフォルダーを選択して、**[!UICONTROL 移動]**&#x200B;を選択します。

## アセット名の変更 {#rename-assets}

1. 参照パネルでアセットを選択し、次のいずれかの操作を行います。

   * 名前を選択し、新しい名前を入力して、**[!UICONTROL Enter]**&#x200B;キーを押すか、名前以外の場所をクリックします。
   * **[!UICONTROL ファイル]**/**[!UICONTROL 名前の変更]**&#x200B;をクリックします。 アセットの名前がハイライトされます。新しい名前を入力し、**[!UICONTROL Enter]**&#x200B;を押します。

既存のDynamic Mediaクラシックアセットの名前は入力しないでください。

## アセットの削除 {#delete-assets}

参照パネルで選択したアセットを削除したり、フォルダ全体を削除したりできます。 削除したアセットとフォルダはごみ箱フォルダに移動され、7 日間経過した後に完全に削除されます。

アセットを削除すると、そのアセットから派生したすべてのアセットも削除されます。例えば、ズームターゲットを作成した画像を削除すると、画像とともにズームターゲットも削除されます。

>[!NOTE]
>
>派生元のアセットを削除すると、ズームターゲット、画像属性、およびヒストリーエントリが完全に削除されます。これらはアセットとともにごみ箱フォルダに移動されず、ごみ箱から元に戻すことはできません。

1. 次のいずれかの操作を行います。

   * 1つ以上のアセットを削除するには、参照パネルでアセットを選択し、**[!UICONTROL 削除]**&#x200B;を押すか、**[!UICONTROL ファイル]**/**[!UICONTROL 削除]**&#x200B;をクリックします。
   * フォルダを削除するには、アセットライブラリでフォルダを選択し、**[!UICONTROL フォルダを削除]**&#x200B;をクリックします。

      フォルダを削除すると、フォルダ、フォルダ内のすべてのアセット、サブフォルダ内のすべてのアセットが削除されます。

>[!NOTE]
>
>アセットファイルを同じ名前の別のアセットファイルで置き換える場合、Dynamic Mediaクラシックでは、アセットファイルを削除するのではなく、上書きすることをお勧めします。

## テキストファイルを使用した複数のアセットの削除 {#delete-multiple-assets-with-a-text-file}

アセットライブラリ内の複数のアセットを一度に削除するには、削除するアセットをテキストファイルでリストし、そのリストをDynamic Mediaクラシックに送信します。

Dynamic MediaクラシックIDのリストを作成し、テキストファイル(.txt)として保存します。 各Dynamic MediaクラシックIDは、それぞれ独自の行に記述され、末尾で改行されている必要があります。

リストを作成したら、次の手順に従ってアセットを削除します。

1. **[!UICONTROL ファイル]**/**[!UICONTROL アセットリストを削除]**&#x200B;をクリックします。
1. アセットリストを削除ダイアログボックスで、削除するアセットのリストが含まれているテキストファイルを参照または入力します。
1. **[!UICONTROL 「削除」]**&#x200B;をクリックします。

テキストファイルを含むアセットを削除すると、リストにDynamic MediaクラシックIDがない場合は、「リストー内の次のエントリを検証できません：」というメッセージが表示され、エントリのリストが示されます。 ただし、Dynamic Mediaクラシックではジョブページでエラーは発生しません。

>[!MORELIKETHIS]
>
>* [参照パネルでのアセットの選択](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [アセットおよびフォルダのアップロードの準備](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [ごみ箱フォルダからのアセットの復元](trash-folder.md#restoring_assets_from_the_trash_folder)

