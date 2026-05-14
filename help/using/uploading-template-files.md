---
title: テンプレートファイルのアップロード
description: Adobe Dynamic Media Classicでテンプレートファイルをアップロードする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
topic: Content Management
level: Experienced
autotag-review: '2026-05-13T19:58:21.817Z'
TQID: 'https://experienceleague.adobe.com/pwmEOjYzNJNV-yxeBfOz3xQBT3rJ9u9imU6cdNgQLDA'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 245
ht-degree: 32%

---

# テンプレートファイルのアップロード{#uploading-template-files}

テンプレートの作成を開始する前に、テンプレートに必要なファイルをAdobe Dynamic Media Classicにアップロードします。 Adobe、Photoshop®PSD®または画像ファイルからテンプレートを作成できます。 テンプレートには TIFF および PNG 画像を使用することをお勧めします。これは、これらの画像が透明化に対応しているためです。

>[!NOTE]
>
>Adobe Dynamic Media Classicでは、Web サイトに表示する正確なサイズのTIFFまたはPSDの透明な画像をテンプレートに使用することをお勧めします。 また、テンプレートを公開するときには、これと同じサイズの画像プリセットで画像を呼び出します。 このようにサイズに注意することで、テンプレートは作成時のサイズが保たれ、サイズ変更（再サンプル）されなくなります。

テンプレートは、Adobe Photoshop PSD ファイルまたは画像ファイルから作成できます。

ファイルのアップロードについて詳しくは、[ ファイルのアップロード ](uploading-files.md#uploading_files)を参照してください。 テンプレートファイルをアップロードするときは、以下の点に注意してください。

* PSD ファイルをアップロードする場合は、そのファイルからテンプレートを作成できます。 Adobe Dynamic Media Classicでは、PSDの各レイヤーに対して個別の画像が作成されます。 アップロードジョブオプションダイアログボックスで、**[!UICONTROL Photoshopオプション]**&#x200B;を選択し、**[!UICONTROL レイヤーの維持]**&#x200B;と&#x200B;**[!UICONTROL テンプレートの作成]**&#x200B;を選択します。 次に、**[!UICONTROL レイヤー名]** ドロップダウンリストから、PSDのレイヤーからAdobe Dynamic Media Classicが作成する画像に名前を付けるオプションを選択します。
詳しくは、[PSD アップロードオプション](psd-files.md#psd_upload_options)を参照してください。

<!--
THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). 
-->

>[!MORELIKETHIS]
>
>* [ ファイルをアップロード ](uploading-files.md#uploading_your_files)
>* [PSD ファイルの操作](psd-files.md#working_with_psd_files)
