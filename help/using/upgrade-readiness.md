---
title: アップグレード準備
description: 次の段階から進む場合のアップグレード準備チェックリスト [!DNL Adobe Dynamic Media Classic] から [!DNL Dynamic Media] オン [!DNL Adobe Experience Manager].
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 1%

---

# アップグレード準備チェックリスト

次のチェックリストを使用して、からのアップグレードの理解と準備に役立ちます。 [!DNL Dynamic Media Classic] から [!DNL Dynamic Media].

|  | タスク | 説明 |
| :--- | :--- | --- |
| **フェーズ 1：ライセンス** | 契約を実行 | トラフィックとストレージに基づき、Adobeアカウントチームがお客様と連携して [!DNL Dynamic Media Classic] ～で更新するライセンス [!DNL Dynamic Media] ライセンス。 |
| **フェーズ 2：準備** | 機能の使用状況を検証 | で使用されている機能を確認します。 [!DNL Dynamic Media Classic] は、 [!DNL Dynamic Media]. 詳しくは、 [機能の比較](/help/using/upgrade-feature-comparison.md) ページに貼り付けます。 まだで使用できない主な機能 [!DNL Dynamic Media] 以下が含まれます。<br>・ビジュアルコンフィギュレータ（画像作成者、画像レンダリング）。<br>・画像テンプレート（1:1 テンプレート）。<br>・ eCatalogs<br>上記の機能を使用している場合でも、アップグレードは、これらの機能が [!DNL Dynamic Media Classic]. |
|   | アセットの特定 | アップグレードに使用するアセットやプリセットを検索し、準備を整えます。 |
| **フェーズ 3：環境** | アップグレード [!DNL Adobe Experience Manager] | のすべてのインスタンス [!DNL Adobe Experience Manager] を最新バージョンに更新する必要があります。 |
|   | 設定 [!DNL Dynamic Media] | Adobeコンサルティングまたはパートナーが構成 [!DNL Dynamic Media] 認証情報を使用して、 |
| **フェーズ 4：アップグレード** | アセットのレプリケート | アップグレードプロセス中に、指定された [!DNL Dynamic Media Classic] アセットがDynamic Mediaにレプリケートされます。 |
| **フェーズ 5：管理の設定** | ユーザーと権限の設定 | ユーザーを作成し、適切な権限を付与します。 |
|   | ビデオエンコーディングプロファイルの設定 | ビデオエンコーディングプロファイルを作成します。 |
|   | ビューアプリセットを設定 | ビューアプリセットを作成します。 |
|   | 画像プリセットの設定 | 画像プリセットを設定します。 |
| **フェーズ 6：検証** | 検証 | 使用例、アセット、リンク、API を確認します。 |
