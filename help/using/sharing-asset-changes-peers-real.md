---
title: アセットの変更をピアとリアルタイムで共有
description: アセットの変更を同業者とリアルタイムでAdobe Dynamic Media Classicで共有する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management,Collaboration
role: Admin,User
exl-id: d74b4966-fe43-4349-bbe1-3a379c49bf1f
topic: Administration, Collaboration
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 26%

---

# アセットの変更をピアとリアルタイムで共有{#sharing-asset-changes-with-peers-in-real-time}

同じ会社内の複数のコンピューターで実行されているAdobe Dynamic Media Classicの複数のコピーを使用すると、任意のAdobe Dynamic Media Classicクライアントからの次の操作が、すべてのピアクライアントでリアルタイムに更新されます。

* アセットの編集（ビルダー、画像エディターなど）
* アセット名の変更
* アセットの削除
* アセットの移動
* 1 つ以上のアセットのアップロード（デスクトップおよび FTP とも）
* フォルダの作成、削除、名前の変更

元のクライアントで変更が行われると、同じ会社にサインインしているすべてのピアクライアントが、変更に応じて更新されます。 ピアで変更対象アセットをいずれかの画像エディタまたはビルダで編集している場合を除き、変更は通知なしにピアに反映されます。

サインインすると、ピアの更新を許可または拒否するように求められました。 選択は「記憶」できるので、この操作は一度限りです。選択をクリアするには、Global Settings の Peer Assisted Networking パネルで該当するサイトを削除します。

ピアによって変更されたアセットを編集している場合は、変更をビルダーまたはエディターに取り込むように求めるプロンプトが表示されます。 次を選択した場合： **[!UICONTROL はい]**&#x200B;その後、ビルダーまたはエディターは、アセットに加えられた変更を破棄し、更新されたアセットを読み込みます。 次を選択した場合： **[!UICONTROL いいえ]**&#x200B;の場合、アセットはビルダーまたはエディターで変更されず、加えた変更はそのセッションで保持されます。

アセットを保存すると、新しいバージョンが存在することが通知され、アセットを変更内容で上書きするかどうかを尋ねられました。
