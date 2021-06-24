---
title: テンプレートファイルのアップロード
description: テンプレートファイルのアップロード方法を説明します。
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
feature: Dynamic Media Classic
role: Business Practitioner
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 48%

---

# テンプレートファイルのアップロード{#uploading-template-files}

テンプレートの作成を開始する前に、テンプレートに必要なファイルをDynamic Media Classicにアップロードします。 Adobe® Photoshop® PSD·ファイルまたは画像ファイルからテンプレートを作成できます。テンプレートには TIFF および PNG 画像を使用することをお勧めします。これは、これらの画像が透明化に対応しているためです。

>[!NOTE]
>
>Dynamic Media Classicでは、Webサイトに表示するのと同じサイズで、透明なTIFFまたはPSD画像をテンプレートに使用することをお勧めします。 また、テンプレートを公開するときには、これと同じサイズの画像プリセットで画像を呼び出します。このようにサイズに注意することで、テンプレートは作成時のサイズが保たれ、サイズ変更（再サンプル）されなくなります。

テンプレートは、Adobe Photoshop PSD ファイルまたは画像ファイルから作成できます。

ファイルのアップロードについて詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。テンプレートファイルをアップロードするときは、以下の点に注意してください。

* PSDファイルをアップロードする場合は、そのファイルからテンプレートを作成できます。 Dynamic Media Classicは、PSD内の各レイヤーに個別の画像を作成します。 アップロードオプションを設定ダイアログボックスで、「**[!UICONTROL Photoshopオプション]**」をクリックし、「**[!UICONTROL レイヤーを維持]**」と「**[!UICONTROL テンプレートを作成]**」を選択します。 次に、「**[!UICONTROL レイヤーの命名]**」ドロップダウンリストからオプションを選択し、Dynamic Media ClassicがPSDのレイヤーから作成する画像に名前を付けます。
詳しくは、[PSD アップロードオプション](psd-files.md#psd_upload_options)を参照してください。

<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [ファイルのアップロード](uploading-files.md#uploading_your_files)
* [PSD ファイルの操作 ](psd-files.md#working_with_psd_files)

