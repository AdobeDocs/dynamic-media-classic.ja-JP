---
title: Adobe Dynamic Media ClassicのUGCについて
description: UGCの概要。
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:34:44.287Z'
TQID: 'https://experienceleague.adobe.com/SwNEO6U33qx45AECK79nff9f9kABWuOdq91d4X8SHd0'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 179
ht-degree: 33%

---

# Adobe Dynamic Media ClassicのUGCについて {#about-user-generated-content}

UGC （ユーザー生成コンテンツ）を利用するには、専用のAdobe Dynamic Media Classicストレージリポジトリにアセットをアップロードして、関連する操作を実行する必要があります。

UGCは、BMP、GIF、JPG、PNG、PSD、TIFFなどのラスター画像ファイル形式に対応しています。

>[!IMPORTANT]
>
>2023年5月1日（PT）以降、Dynamic MediaのUGC アセットは、アップロード日から最大60日間使用できるようになります。 60日後、アセットは削除されます。

<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!NOTE]
>
>Adobe Dynamic Media Classicでの新規または既存のUGC ベクター画像アセットのサポートは、2021年9月30日に終了しました。

アセットをアップロードする前に、共有秘密キーを取得します。 このキーは、アップロードトークンを取得するために使用します。 アセットをアップロードしたり、ほかのユーザ生成コンテンツのタスクを実行したりするときは、このアップロードトークンを送信します。

共有秘密キーとアップロードトークンを取得したら、以下のユーザ生成コンテンツ関連の操作を実行できます。

* アセットのアップロード：
* 画像のアセットメタデータの取得。
* アップロードしたアセットの削除。
* 会社のディスク容量の使用状況に関する情報を取得します。
