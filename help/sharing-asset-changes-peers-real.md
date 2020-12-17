---
title: アセット変更内容のピアとのリアルタイム共有
seo-title: アセット変更内容のピアとのリアルタイム共有
description: 'null'
seo-description: アセットの変更をピアとリアルタイムで共有する方法を説明します。
uuid: 13fa4f6e-66bf-4682-96a9-0e7040706f53
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: ca7c8a7f-76f4-4a25-8c36-617a029e55be
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 83%

---


# アセット変更内容のピアとのリアルタイム共有{#sharing-asset-changes-with-peers-in-real-time}

同じ会社内の1台以上のコンピュータで複数のDynamic Mediaクラシックを実行すると、任意のDynamic Mediaクラシッククライアントからの次の操作がすべてのピアクライアントとリアルタイムで更新されます。

* アセットの編集（ビルダ、画像エディタなど）
* アセット名の変更
* アセットの削除
* アセットの移動
* 1 つ以上のアセットのアップロード（デスクトップおよび FTP とも）
* フォルダの作成、削除、名前の変更

元のクライアントで変更されると、同じ会社にログインしているすべてのピアクライアントに変更内容が更新されます。ピアで変更対象アセットをいずれかの画像エディタまたはビルダで編集している場合を除き、変更は通知なしにピアに反映されます。

ログインすると、Flash Player によりピアの更新を許可または拒否するよう求められます。選択は「記憶」できるので、この操作は一度限りです。選択をクリアするには、Global Settings の Peer Assisted Networking パネルで該当するサイトを削除します。

ピアによって変更されたアセットの編集中だった場合、ピアによる変更をビルダまたはエディタに取り込むよう求められます。「はい」を選択すると、ビルダまたはエディタはアセットに対して行われていた変更を破棄し、更新されたアセットを読み込みます。「いいえ」を選択すると、ビルダまたはエディタでアセットは変更されず、行われていた変更内容がそのセッション内に保持されます。

アセットを保存するとき、新しいバージョンが存在することが通知され、行った変更内容でそのアセットを上書きするかどうかの指定を求められます。
