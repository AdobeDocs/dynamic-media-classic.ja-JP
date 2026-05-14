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
autotag-review: '2026-05-13T20:04:38.888Z'
TQID: 'https://experienceleague.adobe.com/PhoMSxegLPSABPovcBA94eiSksqAcIMhQV93BcAWh-s'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 613
ht-degree: 17%

---

# アセットの移動、名前変更、削除{#moving-renaming-and-deleting-assets}

参照パネルからアセットを移動、名前変更、削除できます。 また、テキストファイルを使用して複数のアセットを同時に削除することもできます。

## アセットの移動 {#move-assets}

参照パネルでアセットを別のフォルダーに移動できます。

**アセットを移動するには：**

1. 参照パネルでアセットを選択し、次のいずれかの操作を行います。

   * アセットを移動するフォルダーをアセットライブラリに表示し、アセットをフォルダーにドラッグします。
   * **[!UICONTROL ファイル]** > **`Move`**&#x200B;に移動し、`Move Assets` ウィンドウでフォルダーを選択し、**`Move`**&#x200B;を選択します。

## アセット名の変更 {#rename-assets}

1. 参照パネルでアセットを選択し、次のいずれかの操作を行います。

   * 名前を選択し、新しい名前を入力して、**[!UICONTROL Enter]**&#x200B;を押すか、名前から離れて選択します。
   * **[!UICONTROL ファイル]** > **[!UICONTROL 名前を変更]**&#x200B;に移動します。 アセットの名前がハイライトされます。 新しい名前を入力し、**[!UICONTROL Enter]**&#x200B;を押します。 既存のAdobe Dynamic Media Classic アセットの名前を入力しないでください。

## アセットの削除 {#delete-assets}

参照パネルで選択したアセットを削除したり、フォルダー全体を削除したりできます。 削除したアセットとフォルダはごみ箱フォルダに移動され、7 日間経過した後に完全に削除されます。

アセットを削除すると、そのアセットから派生したすべてのアセットも削除されます。 例えば、ズームターゲットを作成した画像を削除すると、その画像と共にズームターゲットが削除されます。

派生元のアセットを削除すると、ズームターゲット、画像属性、およびヒストリーエントリが完全に削除されます。 これらはアセットとともにごみ箱フォルダに移動されず、ごみ箱から元に戻すことはできません。

>[!IMPORTANT]
>
>一括削除は集中的な操作です。 同時に大量の削除操作を実行するのではなく、一括削除を順次実行してください。 Adobeでは、1時間あたりのアセット削除数を5000以下に制限することをお勧めします。 1時間あたり5000を超える数値を指定すると、レート制限が発生する可能性があります。

**アセットを削除するには：**

1. 次のいずれかの操作を行います。

   * 1つ以上のアセットを削除するには、参照パネルでアセットを選択し、**[!UICONTROL 削除]**&#x200B;を押すか、**[!UICONTROL ファイル]**/**[!UICONTROL 削除]**&#x200B;に移動します。
   * フォルダーを削除するには、アセットライブラリでフォルダーを選択し、**[!UICONTROL フォルダーの削除]**&#x200B;を選択します。

     フォルダーを削除すると、フォルダー、フォルダー内のすべてのアセット、およびそのサブフォルダー内のすべてのアセットが削除されます。

Adobe Dynamic Media Classicでは、アセットファイルを削除する理由が同じ名前で別のファイルに置き換える場合は、アセットファイルを削除せずに上書きすることをお勧めします。

## テキストファイルを使用した複数のアセットの削除 {#delete-multiple-assets-with-a-text-file}

アセットライブラリ全体で一度に多くのアセットを削除するには、削除するアセットをテキストファイルに一覧表示し、リストをAdobe Dynamic Media Classicに送信します。

Adobe Dynamic Media Classic IDのリストを作成し、テキスト（.txt）ファイルとして保存します。 各Adobe Dynamic Media Classic IDは、独自の行（その後にハードリターン）にする必要があります。

リストを作成したら、次の手順に従ってアセットを削除します。

1. **[!UICONTROL ファイル]**/**[!UICONTROL アセットリストの削除]**&#x200B;に移動します。
1. **[!UICONTROL 削除済みアセットリスト]** ダイアログボックスで、削除するアセットのリストを含むテキストファイルへのパスを入力します。
1. **[!UICONTROL 削除]**&#x200B;を選択します。

テキストファイルを含むアセットを削除すると、リストにAdobe Dynamic Media Classic IDがない場合は、「これらのエントリをリストで検証できません：」というメッセージが表示されます。 エントリのリストも表示されます。 ただし、Adobe Dynamic Media Classicではジョブページにエラーは発生しません。

>[!MORELIKETHIS]
>
>* [参照パネルでアセットを選択](selecting-assets-browse-panel.md#selecting_assets_in_the_browse_panel)
>* [&#x200B; アセットとフォルダーをアップロード用に準備する](uploading-files.md#preparing_your_assets_and_folders_for_uploading)
>* [ごみ箱フォルダーからアセットを復元](trash-folder.md#restoring_assets_from_the_trash_folder)
