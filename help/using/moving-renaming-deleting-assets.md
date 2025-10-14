---
title: アセットの移動、名前変更、削除
description: Adobe Dynamic Media Classicでアセットを移動、名前変更、削除する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 391eb7ce-ed89-47a8-a6c6-5adb3e95bf78
topic: Content Management
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 17%

---

# アセットの移動、名前変更、削除{#moving-renaming-and-deleting-assets}

参照パネルからアセットの移動、名前変更、削除が可能です。 また、テキストファイルを使用して複数のアセットを同時に削除することもできます。

## アセットの移動 {#move-assets}

参照パネルで、アセットを別のフォルダーに移動できます。

**アセットを移動するには：**

1. 参照パネルで 1 つまたは複数のアセットを選択し、次のいずれかの操作を行います。

   * アセットライブラリでアセットの移動先のフォルダーを表示し、アセットをフォルダーにドラッグします。
   * **[!UICONTROL ファイル]**/**[!UICONTROL 移動]** に移動し、「Assetsを移動」ウィンドウでフォルダーを選択して、「**[!UICONTROL 移動]**」を選択します。

## アセット名の変更 {#rename-assets}

1. 参照パネルでアセットを選択し、次のいずれかの操作を行います。

   * 名前を選択し、新しい名前を入力して、**[!UICONTROL Enter]** キーを押すか、名前の外側を選択します。
   * **[!UICONTROL ファイル]**/**[!UICONTROL 名前を変更]** に移動します。 アセットの名前がハイライトされます。新しい名前を入力し、**[!UICONTROL Enter]** キーを押します。 既存のAdobe Dynamic Media Classic アセットの名前を入力しないでください。

## アセットの削除 {#delete-assets}

参照パネルで選択したアセットを削除したり、フォルダー全体を削除したりすることができます。 削除したアセットとフォルダはごみ箱フォルダに移動され、7 日間経過した後に完全に削除されます。

アセットを削除すると、そのアセットから派生したすべてのアセットも削除されます。 例えば、ズームターゲットを作成した画像を削除すると、画像と共にズームターゲットが削除されます。

派生元のアセットを削除すると、ズームターゲット、画像属性、およびヒストリーエントリが完全に削除されます。これらはアセットとともにごみ箱フォルダに移動されず、ごみ箱から元に戻すことはできません。

>[!IMPORTANT]
>
>一括削除は負荷の高い操作です。 一括削除は、同時に大量の削除操作を行うのではなく、順番に実行するようにしてください。 Adobeでは、削除操作を 1 時間あたり 5000 件以下に制限することをお勧めします。 1 時間あたり 5,000 より大きい数は、レート制限の原因となる可能性があります。

**アセットを削除するには：**

1. 次のいずれかの操作を行います。

   * 1 つ以上のアセットを削除するには、参照パネルでアセットを選択して **[!UICONTROL 削除]** を押すか、**[!UICONTROL ファイル]**/**[!UICONTROL 削除]** に移動します。
   * フォルダーを削除するには、アセットライブラリでフォルダーを選択して、「**[!UICONTROL フォルダーを削除]**」を選択します。

     フォルダーを削除すると、フォルダー、フォルダー内のすべてのアセットとそのサブフォルダー内のすべてのアセットが削除されます。

Adobe Dynamic Media Classicでは、アセットファイルを削除する理由が同じ名前の別のアセットファイルに置き換えることである場合は、アセットファイルを削除するのではなく、アセットファイルを上書きすることをお勧めします。

## テキストファイルを使用した複数のアセットの削除 {#delete-multiple-assets-with-a-text-file}

アセットライブラリ全体で一度に多くのアセットを削除するには、削除するアセットをテキストファイルでリストし、リストをAdobe Dynamic Media Classicに送信します。

Adobe Dynamic Media Classic ID のリストを作成し、テキスト（.txt）ファイルとして保存します。 各Adobe Dynamic Media Classic ID は、1 行にする必要があります（その後にハードリターンが続きます）。

リストを作成したら、次の手順に従ってアセットを削除します。

1. **[!UICONTROL ファイル]**/**[!UICONTROL アセットリストを削除]** に移動します。
1. **[!UICONTROL 削除済みアセットリスト]** ダイアログボックスで、削除するアセットのリストを含むテキストファイルへのパスを入力します。
1. 「**[!UICONTROL 削除]**」を選択します。

テキストファイルを使用してアセットを削除するときに、リストにAdobe Dynamic Media Classic ID が含まれていない場合は、「リスト内のこれらのエントリを検証できません：」というメッセージが表示されます。 エントリのリストも表示されます。 ただし、Adobe Dynamic Media Classicでは、ジョブ ページでエラーは生成されません。

>[!MORELIKETHIS]
>
>* [&#x200B; 参照パネルでのアセットの選択 &#x200B;](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [&#x200B; アップロード用のアセットとフォルダーの準備 &#x200B;](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [&#x200B; ごみ箱フォルダーからのアセットの復元 &#x200B;](trash-folder.md#restoring_assets_from_the_trash_folder)
