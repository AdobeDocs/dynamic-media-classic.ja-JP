---
title: ピアーとのリアルタイムでのアセット変更の共有
description: AdobeDynamic Media Classicで、ピアとリアルタイムでアセットの変更を共有する方法を説明します。
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
source-git-commit: e47c22508230adbb1ece323be0c1413a3f27ad89
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 44%

---

# ピアーとのリアルタイムでのアセット変更の共有{#sharing-asset-changes-with-peers-in-real-time}

同じ会社内の複数のAdobeでAdobeDynamic Media Classicを複数コピーする場合、任意のコンピューターDynamic Media Classicクライアントの次のアクションが、すべてのピアクライアントでリアルタイムに更新されます。

* アセットの編集（ビルダー、画像エディターなど）
* アセット名の変更
* アセットの削除
* アセットの移動
* 1 つ以上のアセットのアップロード（デスクトップおよび FTP とも）
* フォルダの作成、削除、名前の変更

元のクライアントで変更がおこなわれると、同じ会社にサインインしているすべてのピアクライアントが変更によって更新されます。 ピアで変更対象アセットをいずれかの画像エディタまたはビルダで編集している場合を除き、変更は通知なしにピアに反映されます。

サインインすると、ピアの更新を許可または拒否するように求められます。 選択は「記憶」できるので、この操作は一度限りです。選択をクリアするには、Global Settings の Peer Assisted Networking パネルで該当するサイトを削除します。

ピアによって変更されたアセットの編集中だった場合、ピアによる変更をビルダまたはエディタに取り込むよう求められます。「**[!UICONTROL はい]**」を選択した場合、ビルダーまたはエディターは、アセットに加えられた変更を破棄し、更新されたアセットを読み込みます。 「**[!UICONTROL いいえ]**」を選択した場合、ビルダーまたはエディターでアセットが変更されず、加えた変更がそのセッションに保持されます。

アセットを保存するとき、新しいバージョンが存在することが通知され、行った変更内容でそのアセットを上書きするかどうかの指定を求められます。
