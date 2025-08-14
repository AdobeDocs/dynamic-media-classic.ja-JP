---
title: アップグレードへの対応
description: ' [!DNL Adobe Dynamic Media Classic]  から  [!DNL Dynamic Media]  に進みたい場合は、アップグレード準備チェッ  [!DNL Adobe Experience Manager] リストが表示されます。'
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 1%

---

# アップグレード準備チェックリスト

次のチェックリストは、[!DNL Dynamic Media Classic] から [!DNL Dynamic Media] へのアップグレードを理解し、準備するのに役立ちます。

|  | タスク | 説明 |
| :--- | :--- | --- |
| **フェーズ 1：ライセンス** | 契約の実行 | Adobe アカウントチームがトラフィックとストレージに基づいて [!DNL Dynamic Media Classic] ライセンスから移行し、[!DNL Dynamic Media] ライセンスで更新できるようにします。 |
| **フェーズ 2：準備** | 機能の使用状況の検証 | [!DNL Dynamic Media Classic] で使用されている機能が [!DNL Dynamic Media] で使用できることを確認します。 [ 機能の比較 ](/help/using/upgrade-feature-comparison.md) ページを参照してください。 [!DNL Dynamic Media] でまだ利用できない主な機能は次のとおりです。<br>・ ビジュアルコンフィギュレーター（画像作成者、画像レンダリング）。<br>・画像テンプレート（1:1 テンプレート）<br>・ eCatalog。<br> 上記の機能を使用している場合でも、これらの機能に [!DNL Dynamic Media Classic] 経由でアクセスできると仮定すると、アップグレードが行われます。 |
|   | アセットの識別 | アップグレードに使用するアセットとプリセットを検索して準備します。 |
| **フェーズ 3：環境** | アップグレード [!DNL Adobe Experience Manager] | [!DNL Adobe Experience Manager] のすべてのインスタンスを最新バージョンに更新する必要があります。 |
|   | 設定 [!DNL Dynamic Media] | Adobe Consultingまたはパートナーが、ユーザーの資格情報を使用して [!DNL Dynamic Media] を設定します。 |
| **フェーズ 4：アップグレード** | アセットをレプリケート | アップグレードプロセス中に、指定された [!DNL Dynamic Media Classic] アセットが Dynamic Media にレプリケートされます。 |
| **フェーズ 5：管理セットアップ** | ユーザーと権限の設定 | ユーザーを作成し、適切な権限を付与します。 |
|   | ビデオエンコーディングプロファイルの設定 | ビデオエンコーディングプロファイルを作成します。 |
|   | ビューアプリセットを設定 | ビューアプリセットを作成します。 |
|   | 画像プリセットの設定 | 画像プリセットを設定します。 |
| **フェーズ 6：検証** | 検証 | ユースケース、アセット、リンク、API を確認します。 |
