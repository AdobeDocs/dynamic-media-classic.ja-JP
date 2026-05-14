---
title: アセットの変更を他のユーザーとリアルタイムで共有
description: Adobe Dynamic Media Classicでアセットの変更をリアルタイムで他のユーザーと共有する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T20:12:54.992Z'
TQID: 'https://experienceleague.adobe.com/Yn5GsnQ4cM3Byk18iEB8Z4uGsTt9FjEZOBP17Yt-K8M'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 281
ht-degree: 26%

---

# アセットの変更を他のユーザーとリアルタイムで共有{#sharing-asset-changes-with-peers-in-real-time}

例えば、同じ会社のコンピューター上でAdobe Dynamic Media Classicの複数のコピーが実行されているとします。 このような場合、Dynamic Media Classic クライアントからの次のアクションは、すべてのピアクライアントでリアルタイムに更新されます。

* アセットの編集（ビルダー、画像エディターなど）
* アセット名の変更
* アセットの削除
* アセットの移動
* 1 つ以上のアセットのアップロード（デスクトップおよび FTP とも）
* フォルダの作成、削除、名前の変更

元のクライアントで変更が行われた後、同じ会社にサインインしたすべてのピアクライアントが変更で更新されます。 ピアで変更対象アセットをいずれかの画像エディタまたはビルダで編集している場合を除き、変更は通知なしにピアに反映されます。

ログインすると、ピア更新を許可または拒否するように求められます。 選択は「記憶」できるので、この操作は一度限りです。 選択をクリアするには、Global Settings の Peer Assisted Networking パネルで該当するサイトを削除します。

ピアによって変更されたアセットを編集する場合は、ビルダーまたはエディターに変更を取り込むよう求められます。 **[!UICONTROL はい]**&#x200B;を選択すると、ビルダーまたはエディターはアセットに加えられた変更を破棄し、更新されたアセットを読み込みます。 **[!UICONTROL No]**&#x200B;を選択した場合、アセットはビルダーまたはエディターで変更されず、行った変更はそのセッションに保持されます。

アセットを保存すると、新しいバージョンが存在することを通知され、変更を加えてアセットを上書きするかどうかを尋ねられます。
