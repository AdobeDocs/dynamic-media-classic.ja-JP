---
title: 画像プリセットの作成と有効化
description: Adobe Dynamic Media Classicで画像プリセットを作成し、有効にする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:41:19.856Z'
TQID: 'https://experienceleague.adobe.com/AlYkBI41GganXzy28kbNN9DXU1Pd4mVCwJKCdwmnN4M'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 265
ht-degree: 47%

---

# 画像プリセットの作成と有効化{#creating-and-enabling-image-presets}

ユーザが Media Portal を使用して画像アセットを書き出すとき、選択したアセットを書き出しダイアログボックスで画像プリセットを選択できます。 画像プリセットは、定義済みの設定のコレクションです。 これらの設定により、書き出し時の画像のサイズ、画質、形式、解像度などの外観を変更できます。

Media Portal 管理者は画像プリセットを作成して、画像が書き出されるときの形式の変更方法を制御できます。 画像プリセットは、ユーザーがAdobe Dynamic Media Classicから画像を書き出す際に、会社の仕様に合わせて画像を再フォーマットします。 画像の形式を自動的に変更するのではなく、画像プリセットで定められた正確な指定に従って書き出します。

画像アセットを書き出す際、以下の制限が適用されます。

* 幅×高さは、画像ごとに100 MB以下にする必要があります。 例えば、画像のアスペクト比が10 K×10 Kを超えること、または8 K×12 Kなどのアスペクト比を超えることはできません。
* 書き出しジョブごとに最大1 GBの合計ファイルサイズがあります。
* 書き出しジョブあたり合計 500 個のアセットまで許容されています。

>[!NOTE]
>
>これらの制限は、派生画像アセットの書き出しにのみ適用され、プライマリファイルの書き出しには適用されません。

画像プリセットを作成するには、[画像プリセット](application-setup.md#image_presets)を参照してください。

ユーザがファイルを書き出すときに画像プリセットを選択できるようにするには、[Media Portal ユーザが使用できる書き出しオプションの指定](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)を参照してください。

グループのメンバーが使用することができる画像プリセットを選択する方法については、[グループの画像プリセットへのアクセス権限の選択](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)を参照してください。
