---
title: アップグレードへの対応
description: 次の状態から進む場合は、アップグレード準備チェックリストです。 [!DNL Adobe Dynamic Media Classic] 対象： [!DNL Dynamic Media] 日付： [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 1%

---

# アップグレード準備チェックリスト

次のチェックリストを使用して、のアップグレードの理解と準備に役立ててください [!DNL Dynamic Media Classic] 対象： [!DNL Dynamic Media].

|  | タスク | 説明 |
| :--- | :--- | --- |
| **フェーズ 1: ライセンス** | 契約の実行 | トラフィックとストレージに基づいて、Adobeアカウントチームはお客様と協力して、 [!DNL Dynamic Media Classic] の更新ライセンス [!DNL Dynamic Media] ライセンス。 |
| **フェーズ 2：準備** | 機能の使用状況の検証 | で使用されている機能の確認 [!DNL Dynamic Media Classic] はで利用できます。 [!DNL Dynamic Media]. を参照してください。 [機能の比較](/help/using/upgrade-feature-comparison.md) ページ。 主な機能はではまだ利用できません [!DNL Dynamic Media] 以下を含めます。<br>・ Visual Configurator （イメージ作成、イメージ レンダリング）<br>・画像テンプレート（1:1 テンプレート）。<br>・ eCatalog。<br>上記の機能を使用している場合でも、の経由でこれらの機能にアクセスできることを前提として、アップグレードが行われます。 [!DNL Dynamic Media Classic]. |
|   | アセットの識別 | アップグレードに使用するアセットとプリセットを検索して準備します。 |
| **フェーズ 3：環境** | アップグレード [!DNL Adobe Experience Manager] | のすべてのインスタンス [!DNL Adobe Experience Manager] を最新バージョンに更新する必要があります。 |
|   | 設定 [!DNL Dynamic Media] | Adobeのコンサルティングまたはパートナーによる構成 [!DNL Dynamic Media] の資格情報を使用します。 |
| **フェーズ 4：アップグレード** | アセットをレプリケート | アップグレードプロセス中、以下を指定 [!DNL Dynamic Media Classic] アセットはDynamic Mediaにレプリケートされます。 |
| **フェーズ 5：管理セットアップ** | ユーザーと権限の設定 | ユーザーを作成し、適切な権限を付与します。 |
|   | ビデオエンコーディングプロファイルの設定 | ビデオエンコーディングプロファイルを作成します。 |
|   | ビューアプリセットを設定 | ビューアプリセットを作成します。 |
|   | 画像プリセットの設定 | 画像プリセットを設定します。 |
| **フェーズ 6：検証** | 検証 | ユースケース、アセット、リンク、API を確認します。 |
