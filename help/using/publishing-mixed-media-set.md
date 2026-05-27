---
title: 混在メディアセットの公開
description: Adobe Dynamic Media Classicから混在メディアセットを公開する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 1fca9640-d127-454a-b3aa-b2ac82136e62
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:08:57.110Z'
TQID: 'https://experienceleague.adobe.com/ZDf5ovDIKfCJ5p-6-Qz-isp77LnCQDKJo5hQA1HBN0w'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 264
ht-degree: 12%

---

# 混在メディアセットの公開{#publishing-a-mixed-media-set}

公開用にマークした混在メディアセットをAdobe Dynamic Media Classic Video ServerおよびImage Serverに公開するには、公開ジョブを作成します。 Adobe Dynamic Media Classicでは、特定のサーバーに公開するための高度な公開オプションと、既に公開されているアセットを再公開するためのオプションを提供しています。

>[!NOTE]
>
>混在メディアセットは、**ビデオサーバー**&#x200B;にも **Image Server** にも公開する必要があります。 **Video Server**&#x200B;を使用して、公開用にマークした実際のビデオを公開します。 また、**Image Server**&#x200B;を使用して、ビデオサムネールなどの関連アセットを公開し、アダプティブビデオセットの情報を設定します。

Adobe Dynamic Media Classicは、ジョブ画面で公開ジョブを追跡します。

詳しくは、[公開](publishing-files.md#publishing_files)を参照してください。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Updated the following steps as per Cynthia email, 11/9/2012, added 11/12/2012</p>

 -->

**混在メディアセットを公開するには：**

1. 次のいずれかの操作を行います。

   * 参照パネルで、公開する各ファイル名の横にある「**[!UICONTROL 公開用にマーク]**」を選択します。
   * アップロード画面で、公開する各ファイル名の横にある&#x200B;**[!UICONTROL 公開用にマーク]**&#x200B;を選択します。

1. グローバルナビゲーションバーで、**[!UICONTROL 公開]**&#x200B;を選択します。
1. 必要なスケジュール・オプションを設定します。
1. （オプション）「**[!UICONTROL ジョブ名]**」フィールドに、公開ジョブの名前を入力します。
1. **[!UICONTROL 詳細]** オプションで、**[!UICONTROL 公開先]** ドロップダウンリストから「**[!UICONTROL ビデオサーバー]**」を選択します。

   設定できる詳細なオプションについては、[高度な公開オプション ](publishing-files.md#advanced_publish_options)を参照してください。

1. 「**[!UICONTROL 公開を送信]**」を選択します。
1. 上記の手順2～4を繰り返します。
1. 「**[!UICONTROL 詳細]**」の「**[!UICONTROL 公開先]**」ドロップダウンリストで、「**[!UICONTROL Image Server]**」を選択します。

   設定できる詳細なオプションについては、[高度な公開オプション ](publishing-files.md#advanced_publish_options)を参照してください。

1. 「**[!UICONTROL 公開を送信]**」を選択します。
