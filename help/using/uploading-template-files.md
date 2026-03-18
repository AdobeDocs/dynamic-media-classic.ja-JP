---
title: テンプレートファイルのアップロード
description: Adobe Dynamic Media Classicにテンプレートファイルをアップロードする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
topic: Content Management
level: Experienced
source-git-commit: 9102019811713b953e016fc7c47dc9f7a0dfbcd9
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 32%

---

# テンプレートファイルのアップロード{#uploading-template-files}

テンプレートの構築を開始する前に、テンプレートに必要なファイルをAdobe Dynamic Media Classicにアップロードします。 テンプレートは、Adobe®Photoshop®PSDまたは画像ファイルから作成できます。 テンプレートには TIFF および PNG 画像を使用することをお勧めします。これは、これらの画像が透明化に対応しているためです。

>[!NOTE]
>
>Adobe Dynamic Media Classicでは、Web サイトに表示する正確なサイズのテンプレートに、透明なTIFF画像またはPSD画像を使用することをお勧めします。 また、テンプレートを公開するときには、これと同じサイズの画像プリセットで画像を呼び出します。 このようにサイズに注意することで、テンプレートは作成時のサイズが保たれ、サイズ変更（再サンプル）されなくなります。

テンプレートは、Adobe Photoshop PSD ファイルまたは画像ファイルから作成できます。

ファイルのアップロード手順について詳しくは、[ ファイルのアップロード ](uploading-files.md#uploading_files) を参照してください。 テンプレートファイルをアップロードするときは、以下の点に注意してください。

* PSD ファイルをアップロードする場合は、そこからテンプレートを作成できます。 Adobe Dynamic Media Classicは、PSDのレイヤーごとに個別の画像を作成します。 「アップロードジョブオプション」ダイアログボックスで、「**[!UICONTROL Photoshop オプション]**」を選択し、「**[!UICONTROL レイヤーを維持]**」および「**[!UICONTROL テンプレートを作成]**」を選択します。 次に、「**[!UICONTROL レイヤーの名前]**」ドロップダウンリストからオプションを選択して、Adobe Dynamic Media ClassicがPSDのレイヤーから作成する画像に名前を付けます。
詳しくは、[PSD アップロードオプション](psd-files.md#psd_upload_options)を参照してください。

<!--
THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). 
-->

>[!MORELIKETHIS]
>
>* [ ファイルをアップロードする ](uploading-files.md#uploading_your_files)
>* [PSD ファイルの操作 ](psd-files.md#working_with_psd_files)
