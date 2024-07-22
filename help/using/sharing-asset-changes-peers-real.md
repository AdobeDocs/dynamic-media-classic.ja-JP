---
title: アセットの変更をリアルタイムで仲間と共有
description: Adobe Dynamic Media Classicでアセットの変更内容をリアルタイムでピアと共有する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 26%

---

# アセットの変更をリアルタイムで仲間と共有{#sharing-asset-changes-with-peers-in-real-time}

同じ会社のコンピューター上で実行されているAdobe Dynamic Media Classicのコピーが複数あるとします。 このようなシナリオでは、任意のDynamic Media Classic クライアントからの次のアクションが、すべてのピアクライアントでリアルタイムに更新されます。

* アセットの編集（ビルダー、画像エディターなど）
* アセット名の変更
* アセットの削除
* アセットの移動
* 1 つ以上のアセットのアップロード（デスクトップおよび FTP とも）
* フォルダの作成、削除、名前の変更

元のクライアントで変更が行われると、同じ会社にサインインしているすべてのピア クライアントがその変更で更新されます。 ピアで変更対象アセットをいずれかの画像エディタまたはビルダで編集している場合を除き、変更は通知なしにピアに反映されます。

ログインすると、ピア更新を許可または拒否するように求められます。 選択は「記憶」できるので、この操作は一度限りです。選択をクリアするには、Global Settings の Peer Assisted Networking パネルで該当するサイトを削除します。

ピアによって変更されたアセットを編集している場合は、変更をビルダーまたはエディターに取り込むように求められます。 **[!UICONTROL はい]** を選択すると、ビルダーまたはエディターによってアセットに加えられた変更が破棄され、更新されたアセットが読み込まれます。 **[!UICONTROL いいえ]** を選択した場合、ビルダーまたはエディター内のアセットは変更されず、加えた変更はそのセッションで保持されます。

アセットを保存すると、新しいバージョンが存在することが通知され、変更をアセットに上書きするかどうかを尋ねられます。
