---
title: 画像プリセットを作成して有効にする
description: Adobe Dynamic Media Classicで画像プリセットを作成して有効にする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Image Presets,Asset Management
role: Admin,User
exl-id: 94c6c388-226b-4172-a6c7-a8dcf9c0f0cf
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 49%

---

# 画像プリセットを作成して有効にする{#creating-and-enabling-image-presets}

ユーザが Media Portal を使用して画像アセットを書き出すとき、選択したアセットを書き出しダイアログボックスで画像プリセットを選択できます。画像プリセットは、書き出し時の画像のサイズ、画質、形式、解像度、その他の外観を変更する事前定義済みの設定のコレクションです。

Media Portal 管理者は画像プリセットを作成して、画像が書き出されるときの形式の変更方法を制御できます。ユーザーがAdobe Dynamic Media Classicから画像を書き出すと、画像プリセットによって、画像が会社の仕様に合わせて再フォーマットされます。 画像の形式を自動的に変更するのではなく、画像プリセットで定められた正確な指定に従って書き出します。

画像アセットを書き出す際、以下の制限が適用されます。

* 幅×高さは、1 つの画像につき 100 MB 以下である必要があります。 例えば、画像のサイズは 10 K × 10 K 以下にしたり、縦横比のバリエーション（8 K × 12 K など）を超えたりすることはできません。
* エクスポートジョブあたりの合計ファイルサイズは最大 1 GB です。
* 書き出しジョブあたり合計 500 個のアセットまで許容されています。

>[!NOTE]
>
>これらの制限は、派生画像アセットの書き出しにのみ適用され、プライマリファイルの書き出しには適用されません。

画像プリセットを作成するには、[画像プリセット](application-setup.md#image_presets)を参照してください。

ユーザがファイルを書き出すときに画像プリセットを選択できるようにするには、[Media Portal ユーザが使用できる書き出しオプションの指定](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)を参照してください。

グループのメンバーが使用することができる画像プリセットを選択する方法については、[グループの画像プリセットへのアクセス権限の選択](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)を参照してください。
