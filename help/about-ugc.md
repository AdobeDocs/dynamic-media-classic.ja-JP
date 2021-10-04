---
title: Dynamic Media Classic のユーザー生成コンテンツについて
description: ユーザー生成コンテンツの紹介です。
uuid: ba867a6a-84a4-4968-9a77-712f3ce5dad5
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
discoiquuid: c1594abf-8cc2-46dd-88bf-af93db7db607
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
source-git-commit: f92109182283f3bf046604b1b6910180f858d73e
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 48%

---

# Dynamic Media Classic のユーザー生成コンテンツについて {#about-user-generated-content}

UGC（ユーザー生成コンテンツ）を使用する場合は、専用のAdobeDynamic Media Classic ストレージリポジトリにアセットをアップロードし、関連する操作を実行します。

UGC は、ラスター画像ファイル形式 (BMP、GIF、JPG、PNG、PSD、TIFF) をサポートしています。
<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!IMPORTANT]
>
>AdobeDynamic Media Classic での新規または既存の UGC ベクトル画像アセットのサポートは、2021 年 9 月 30 日に終了しました。

アセットをアップロードする前に、共有秘密キーを取得します。このキーは、アップロードトークンを取得するために使用します。アセットをアップロードしたり、ほかのユーザ生成コンテンツのタスクを実行したりするときは、このアップロードトークンを送信します。

共有秘密キーとアップロードトークンを取得したら、以下のユーザ生成コンテンツ関連の操作を実行できます。

* アセットのアップロード。
* 画像のアセットメタデータの取得。
* アップロードしたアセットの削除。
* 会社のディスク使用状況に関する情報の取得。
