---
title: テンプレートファイルのアップロード
description: Adobe Dynamic Media Classicでテンプレートファイルをアップロードする方法を説明します。
uuid: e19979b5-3f41-49c5-99aa-107ede3be98c
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 75658717-5c39-473e-9d32-718d00706310
feature: Dynamic Media Classic
role: User
exl-id: a105c18a-7e06-43cb-938c-a3bcdc3e9d22
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 38%

---

# テンプレートファイルのアップロード{#uploading-template-files}

テンプレートの作成を開始する前に、テンプレートに必要なファイルをAdobe Dynamic Media Classicにアップロードします。 Adobe® Photoshop® PSD·ファイルまたは画像ファイルからテンプレートを作成できます。テンプレートには TIFF および PNG 画像を使用することをお勧めします。これは、これらの画像が透明化に対応しているためです。

>[!NOTE]
>
>Adobe Dynamic Media Classicでは、透明なTIFFまたはPSD画像を、Web サイトに表示するサイズと同じサイズでテンプレートに使用することをお勧めします。 また、テンプレートを公開するときには、これと同じサイズの画像プリセットで画像を呼び出します。このようにサイズに注意することで、テンプレートは作成時のサイズが保たれ、サイズ変更（再サンプル）されなくなります。

テンプレートは、Adobe Photoshop PSD ファイルまたは画像ファイルから作成できます。

ファイルのアップロードについて詳しくは、 [ファイルをアップロード](uploading-files.md#uploading_files). テンプレートファイルをアップロードするときは、以下の点に注意してください。

* テンプレートファイルをアップロードする場合は、PSDファイルからテンプレートを作成できます。 Adobe Dynamic Media Classicは、PSD内の各レイヤーに対して個別のイメージを作成します。 アップロードオプションを設定ダイアログボックスで、 **[!UICONTROL Photoshop Options]**&#x200B;を選択し、 **[!UICONTROL レイヤーを維持]** および **[!UICONTROL テンプレートを作成]**. 次に、 **[!UICONTROL レイヤーの命名]** Adobe Dynamic Media ClassicがPSDのレイヤーから作成する画像に名前を付けるためのドロップダウンリスト。
詳しくは、[PSD アップロードオプション](psd-files.md#psd_upload_options)を参照してください。

<!-- THERE IS NO LONGER AN IMAGE EDITING OPTIONS MENU * If you are uploading images, you can create a mask from its clipping path. This option applies to images created with image-editing applications in which a clipping path was created. In the Upload Job Options dialog box, select Image Editing Options and select the Create Mask From Clipping Path option. 
See [Image editing options at upload](image-editing-options-upload.md#image-editing-options-at-upload). -->

>[!MORELIKETHIS]
>
>* [ファイルをアップロード](uploading-files.md#uploading_your_files)
>* [PSDファイルの操作](psd-files.md#working_with_psd_files)

