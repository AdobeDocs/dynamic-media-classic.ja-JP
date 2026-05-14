---
title: プロジェクトを使用した作業の整理
description: Adobe Dynamic Media Classicでプロジェクトを使用して作業を整理する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 69aabf4a-21bc-4bd8-8aad-33c2cfb9cf57
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:06:21.685Z'
TQID: 'https://experienceleague.adobe.com/5qHEB75XuruG3SWp5zXaM3nadbtkW9M7xRvPA0mxo4M'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 483
ht-degree: 21%

---

# プロジェクトを使用した作業の整理{#organizing-your-work-with-projects}

プロジェクトを使用すると、アセットが保存されているフォルダとは独立してアセットを編成することができます。 アセットは、1 つのフォルダにのみ配置できますが、アセット編成のために複数のプロジェクトフォルダにコピーすることができます。

プロジェクトフォルダを作成して、そこにアセットを配置することができます。 プロジェクト内のAssetsは、実際にはアセットが保存されているAsset Library フォルダーへのポインターです。 アセットは、複数のプロジェクトに配置することができます。 例えば、ブラウスの画像を「ブラウス」と「フォールコレクション」の両方のプロジェクトフォルダーに配置できます。

プロジェクトは、ファイルをアップロードしたときに作成できます。アセットライブラリパネルで作成することも可能です。

>[!NOTE]
>
>Adobe Dynamic Media Classicでは、プロジェクトではなくメタデータを使用してアセットを整理することをお勧めします。 [&#x200B; メタデータの表示、追加、エクスポート &#x200B;](viewing-adding-exporting-metadata.md)を参照してください。

>[!NOTE]
>
>一般ユーザがプロジェクト内のアセットを編成するには、管理者によって、それが可能なように設定されている必要があります。 Assets ライブラリの下部に「プロジェクト」フォルダーのセクションが表示されない場合、このアセットの整理方法は使用できません。 詳しくは、[アプリケーションの全般設定](application-setup.md#general-settings)を参照してください。

## プロジェクトフォルダーの作成 {#creating-a-project-folder}

Assets ライブラリから始まるプロジェクトフォルダーを作成するか、ファイルをAdobe Dynamic Media Classicにアップロードするときに作成できます。

* **アセットライブラリ**: アセットライブラリの一番下にある「プロジェクト」セクションまでスクロールし、「**[!UICONTROL プロジェクトを追加]**」を選択します。 プロジェクトの名前を入力します。

* **ファイルをアップロードする場合**: アップロード画面で、**[!UICONTROL プロジェクトに追加]** > **[!UICONTROL プロジェクトを作成]**&#x200B;に移動します。 プロジェクトの名前を入力します。

>[!NOTE]
>
>アセットライブラリの「プロジェクト」エリアは、単一レベルのフォルダーリストです。サブフォルダーは許可されません。

## プロジェクトフォルダーの操作 {#working-with-project-folders}

プロジェクトフォルダーを表示、削除、名前を変更するには、次のいずれかの操作を行います。

* **コンテンツを参照**: アセットライブラリでフォルダーの名前を選択します。 アセットが参照パネルに表示されます。

* **プロジェクトフォルダーを削除**: プロジェクトフォルダーを選択し、**[!UICONTROL プロジェクトを削除]**&#x200B;を選択します。 プロジェクトフォルダーからアセットを削除しても、Adobe Dynamic Media Classicからアセットが削除されることはありません。アセットは、保存されている元のフォルダーに残ります。

* **プロジェクトフォルダーの名前を変更**: アセットパネルでフォルダーの名前をダブルクリックし、新しい名前を入力します。

## プロジェクトフォルダーへのアセットの追加 {#adding-assets-to-a-project-folder}

参照パネルから始まるプロジェクトフォルダーに、またはAdobe Dynamic Media Classicにファイルをアップロードする際に、画像を追加できます。

* **参照パネル**&#x200B;からアセットを選択し、プロジェクト フォルダーにドラッグします。 **[!UICONTROL ファイル]**/**[!UICONTROL プロジェクトに追加]**&#x200B;することもできます。 プロジェクトを選択ダイアログボックスでプロジェクトフォルダー名を選択し、**[!UICONTROL 送信]**&#x200B;を選択します。

* **ファイルをアップロードする場合**: アップロードページで、**[!UICONTROL ジョブオプション]**&#x200B;を選択します。 アップロードジョブオプションダイアログボックスで、「**[!UICONTROL プロジェクト]**」を選択し、プロジェクト名を選択します。
