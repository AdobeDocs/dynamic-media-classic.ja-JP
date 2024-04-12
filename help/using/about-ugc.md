---
title: Adobe Dynamic Media Classicのユーザー生成コンテンツについて
description: ユーザー作成コンテンツの概要です。
contentOwner: rbrough
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/user_generated_content
feature: Dynamic Media Classic
role: Admin,User
exl-id: 14729192-7b9d-4f42-99da-6564a3f35959
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 33%

---

# Adobe Dynamic Media Classicのユーザー生成コンテンツについて {#about-user-generated-content}

UGC （ユーザー生成コンテンツ）を使用するには、専用のAdobe Dynamic Media Classic ストレージリポジトリーにアセットをアップロードし、関連する操作を実行します。

UGC は、ラスターイメージファイル形式 BMP、GIF、JPG、PNG、PSD、TIFFをサポートしています。

>[!IMPORTANT]
>
>2023 年 5 月 1 日（PT）以降、Dynamic Mediaの UGC アセットは、アップロード日から最大 60 日間使用できます。 60 日後にアセットが削除されます。

<!-- * Vector: AI, EPS (EPS files from Adobe Illustrator 2018 are not supported), PDF (only when the PDF file is previously opened and saved in Adobe Illustrator CS6) -->

>[!NOTE]
>
>Adobe Dynamic Media Classicでの新規または既存の UGC ベクター画像アセットのサポートは、2021 年 9 月 30 日（PT）に終了しました。

アセットをアップロードする前に、共有秘密キーを取得します。このキーは、アップロードトークンを取得するために使用します。アセットをアップロードしたり、ほかのユーザ生成コンテンツのタスクを実行したりするときは、このアップロードトークンを送信します。

共有秘密キーとアップロードトークンを取得したら、以下のユーザ生成コンテンツ関連の操作を実行できます。

* アセットをアップロードします。
* 画像のアセットメタデータの取得。
* アップロードしたアセットの削除。
* 会社のディスク容量の使用状況に関する情報を取得します。
