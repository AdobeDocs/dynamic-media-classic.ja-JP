---
title: 混在メディアセットの公開
description: Adobe Dynamic Media Classicから混在メディアセットを公開する方法を説明します。
uuid: 4172347c-7bb3-468d-bda2-fd1c26ccab85
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
discoiquuid: 4e8694f7-c1b5-4d45-a18b-2b9494db1757
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 1fca9640-d127-454a-b3aa-b2ac82136e62
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 31%

---

# 混在メディアセットの公開{#publishing-a-mixed-media-set}

Adobe Dynamic Media Classic Video Server および Image Server への公開用としてマークした混在メディアセットを公開する公開ジョブを作成します。 Adobe Dynamic Media Classicは、特定のサーバーに公開するための高度な公開オプションと、既に公開済みのアセットを再公開するためのオプションを提供します。

>[!NOTE]
>
>混在メディアセットは、**ビデオサーバー**&#x200B;にも **Image Server** にも公開する必要があります。**ビデオサーバー**&#x200B;を使用して、公開用にマークした実際のビデオを公開します。また、 **Image Server** ：ビデオサムネールなどの関連アセットを公開し、任意のアダプティブビデオセットの情報を設定します。

Adobe Dynamic Media Classicは、ジョブ画面で公開ジョブを追跡します。

詳しくは、[公開](publishing-files.md#publishing_files)を参照してください。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Updated the following steps as per Cynthia email, 11/9/2012, added 11/12/2012</p>

 -->

**混在メディアセットを公開するには:**

1. 次のいずれかの操作を行います。

   * 参照パネルで、「 **[!UICONTROL 公開用にマーク]** をクリックします。
   * アップロード画面で、「 」を選択します。 **[!UICONTROL 公開用にマーク]** をクリックします。

1. グローバルナビゲーションバーで、 **[!UICONTROL 公開]**.
1. 必要なスケジュールオプションを設定します。
1. （オプション）「**[!UICONTROL ジョブ名]**」フィールドに、公開ジョブの名前を入力します。
1. 「**[!UICONTROL 詳細]**」オプションの「**[!UICONTROL 公開先]**」ドロップダウンリストで、「**[!UICONTROL ビデオサーバー]**」を選択します。

   詳しくは、 [詳細公開オプション](publishing-files.md#advanced_publish_options) 他のオプションについては、を設定できます。

1. 選択 **[!UICONTROL 公開を送信]**.
1. 上記の手順 2～4 を繰り返します。
1. 「**[!UICONTROL 詳細]**」の「**[!UICONTROL 公開先]**」ドロップダウンリストで、「**[!UICONTROL Image Server]**」を選択します。

   詳しくは、 [詳細公開オプション](publishing-files.md#advanced_publish_options) 他のオプションについては、を設定できます。

1. 選択 **[!UICONTROL 公開を送信]**.
