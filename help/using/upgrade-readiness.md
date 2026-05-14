---
title: アップグレードの準備状況
description: ' [!DNL Adobe Dynamic Media Classic] から [!DNL Dynamic Media] まで [!DNL Adobe Experience Manager]に進む場合は、アップグレードの準備状況チェックリストを使用します。'
feature: Dynamic Media Classic
role: Admin,User
exl-id: 86537998-b7e9-449c-83eb-6fd04533a00f
topic: Administration, Migration
level: Intermediate
autotag-review: '2026-05-13T20:16:07.073Z'
TQID: 'https://experienceleague.adobe.com/3Kcp3UwvJV8Mkzk6RBRgOJQ7JKF3Ldek-SiOeqS5EKE'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 221
ht-degree: 1%

---

# アップグレードの準備状況チェックリスト

次のチェックリストを使用して、[!DNL Dynamic Media Classic]から[!DNL Dynamic Media]へのアップグレードについて理解し、準備します。

|  | タスク | 説明 |
| :--- | :--- | --- |
| **フェーズ 1: ライセンス** | 契約の実行 | トラフィックとストレージに基づいて、Adobe アカウントチームはユーザーと協力して、[!DNL Dynamic Media Classic] ライセンスから[!DNL Dynamic Media] ライセンスの更新に移行します。 |
| **フェーズ 2：準備** | 機能の利用状況を検証 | [!DNL Dynamic Media Classic]で使用されている機能が[!DNL Dynamic Media]で利用できることを確認してください。 [機能比較](/help/using/upgrade-feature-comparison.md) ページを参照してください。 [!DNL Dynamic Media]で利用できない主な機能には、次のようなものがあります。<br>・ Visual Configurator （Image Author, Image Render）。<br>・ Image Templates （1:1 Template）。<br>・ eCatalogs.<br>上記の機能が使用されている場合でも、[!DNL Dynamic Media Classic]経由でこれらの機能にアクセスできるという前提でアップグレードを実行できます。 |
|   | アセットの特定 | アップグレードに使用するアセットとプリセットを検索して準備を整えます。 |
| **フェーズ 3：環境** | [!DNL Adobe Experience Manager]をアップグレード | [!DNL Adobe Experience Manager]のすべてのインスタンスを最新バージョンに更新する必要があります。 |
|   | [!DNL Dynamic Media]を設定 | Adobe Consultingまたはパートナーは、お客様の資格情報を使用して[!DNL Dynamic Media]を設定します。 |
| **フェーズ 4: アップグレード** | アセットのレプリケート | アップグレードプロセス中、指定された[!DNL Dynamic Media Classic] アセットがDynamic Mediaにレプリケートされます。 |
| **フェーズ 5：管理設定** | ユーザーと権限の設定 | ユーザーを作成し、適切な権限を付与します。 |
|   | ビデオエンコーディングプロファイルの設定 | 動画エンコーディングプロファイルの作成。 |
|   | ビューアプリセットの設定 | ビューアプリセットの作成。 |
|   | 画像プリセットの設定 | 画像プリセットを設定します。 |
| **フェーズ 6：検証** | 検証 | ユースケース、アセット、リンク、APIを検証する。 |
