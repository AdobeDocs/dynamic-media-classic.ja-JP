---
title: 画像プリセットの作成と有効化
description: Dynamic Media Classicで画像プリセットを作成して有効にする方法について説明します。Adobe
uuid: 62cfc6fa-da91-4c42-a3ed-10956384d633
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 84257b2a-681c-4fe9-a6e5-3633c1d61d8c
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 78%

---

# 画像プリセットの作成と有効化{#creating-and-enabling-image-presets}

ユーザが Media Portal を使用して画像アセットを書き出すとき、選択したアセットを書き出しダイアログボックスで画像プリセットを選択できます。画像プリセットは、画像を書き出すときにサイズ、画質、形式、解像度およびその他の画像の外観を変更する、一連の定義済みの設定です。

Media Portal 管理者は画像プリセットを作成して、画像が書き出されるときの形式の変更方法を制御できます。画像プリセットは、ユーザーがDynamic Media Classicから画像を書き出す際に、Adobeの仕様に合わせて画像を再フォーマットします。 画像の形式を自動的に変更するのではなく、画像プリセットで定められた正確な指定に従って書き出します。

画像アセットを書き出す際、以下の制限が適用されます。

* 幅 x 高さは、画像あたり 100 MB 以下である必要があります。例えば、画像が 10K x 10K を超えたり、8K x 12K のような縦横比を超えてはいけません。
* 1つの書き出しジョブにつき、最大で1 GBのファイルサイズがあります。
* 書き出しジョブあたり、アセットの合計は最大で 500 個です。

>[!NOTE]
>
>これらの制限は、マスターファイルの書き出しではなく、派生した画像アセットの書き出しのみに適用されます。

画像プリセットを作成するには、[画像プリセット](application-setup.md#image_presets)を参照してください。

ユーザがファイルを書き出すときに画像プリセットを選択できるようにするには、[Media Portal ユーザが使用できる書き出しオプションの指定](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)を参照してください。

グループのメンバーが使用することができる画像プリセットを選択する方法については、[グループの画像プリセットへのアクセス権限の選択](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)を参照してください。
