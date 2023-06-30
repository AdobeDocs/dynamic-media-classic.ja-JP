---
title: 画像プリセットの設定
description: Adobe Dynamic Media Classicで画像プリセットを設定する方法について説明します。
uuid: 90530948-dee9-41bd-b39e-684140446abc
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 1ec39fe5-7b2a-4034-9570-6b5595f97052
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 50%

---

# 画像プリセットの設定{#setting-up-image-presets}

画像プリセットは、マクロのような定義済みのサイズおよび形式に関するコマンドの集まりであり、特定の名前が付けられて保存されています。画像プリセットの動作を理解するには、Web サイトで各製品画像を 2 つの異なるサイズで表示する必要があるとします。500 x 500 ピクセルおよび 150 x 150 ピクセル。 500 x 500 pixel で画像を表示する「Enlarge」という画像プリセットと、150 x 150 pixel で画像を表示する「Thumbnail」という画像プリセットを作成したとします。「拡大」および「サムネール」サイズの画像を配信するために、Dynamic Media Image Server では「拡大画像プリセット」と「サムネール画像プリセット」の定義を検索します。 サーバは、各画像プリセットのサイズおよび形式の指定に従って画像を動的に生成します。

Adobe Dynamic Media Classicには、使用するための「ベストプラクティス」画像プリセットがいくつか用意されています。 管理者は画像プリセットを作成することもできます。 画像プリセットは、新規作成することも、既存のプリセットを使用して別の名前で保存することもできます。

サーバから動的に配信されるときにサイズが縮小される画像は、シャープとディテールが損なわれることがあります。このため、各画像プリセットには、特定のサイズで配信されるときに画像を最適化するための形式制御機能が含まれています。これらの制御機能により、画像がシャープでクリアな状態で Web サイトやアプリケーションに配信されるようになります。

## 画像プリセットの作成 {#creating-an-image-preset}

会社の管理者は、独自の画像プリセットを作成できます。画像プリセットを作成することも、Adobe Dynamic Media Classicが提供するデフォルトの画像プリセットを使用して開始し、編集して、新しい名前で保存することもできます。

**画像プリセットを作成するには:**

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**.

   この画面で画像プリセット名を探して選択し、既存の画像プリセットをプレビューすることができます。画像プリセット名を選択すると、プレビューウィンドウ内のサンプル画像のサイズと外観が変わります。

1. 次のいずれかの操作を行います。

   * **画像プリセットの作成**  — 選択 **[!UICONTROL 追加]**.
   * **画像プリセットの編集**  — 作成したい画像プリセットに最も近い画像プリセットを参照し、「 」を選択します **[!UICONTROL 編集]**.

1. 画像プリセットの名前を入力します。
1. 高さおよび幅の値をピクセル単位で入力します。これらの値は、画像が配信されるサイズを決定します。
1. プリセットを追加画面またはプリセットを編集画面に必要な情報を入力します。詳しくは、[画像プリセットのオプション](application-setup.md#image_preset_options)を参照してください。

   Adobe Dynamic Media Classicは、次の「ベストプラクティス」オプションを推奨して開始します。

   * **[!UICONTROL 形式]** - 「JPEG」または要件を満たす他の形式を選択します。 すべての Web ブラウザが JPEG 画像形式をサポートしています。この形式では、小さいファイルサイズで優れた画質を得ることができます。ただし、JPEG 形式の画像は非可逆圧縮方式を使用するため、圧縮設定が低すぎると斑点が発生することがあります。そのため、Adobe Dynamic Media Classicでは（スライダーの）圧縮品質を 75 に設定することをお勧めします。 この設定により、小さいファイルサイズで優れた画質を得ることができます。

   * **[!UICONTROL シャープ]** - 「シャープ」は選択しないでください（このシャープフィルターでは、以下の制御ができません） **[!UICONTROL アンシャープマスク]** 設定 )。

   * **[!UICONTROL 再サンプルモード]**  — 選択 **[!UICONTROL バイキュービック法]**.

   * **[!UICONTROL アンシャープマスク]** (USM) — 次の設定を入力します。

   | プリセットの種類 | サイズ | 適用量 | 半径 | しきい値 |
   | --- | --- | --- | --- | --- |
   | Cross-Sell（ミニサムネール） | 75 x 75 | 1.5 | 0.8 | 5 |
   | Thumbnail | 150 × 150 | 1.1 | 1 | 5 |
   | Main | 350 x 350 | 1 | 1 | 6 |
   | Enlarge | 500 x 500 | 1.2 | 1.2 | 5 |

1. 選択 **[!UICONTROL 保存]**.

ここに示すAdobe Dynamic Media Classicの画像プリセットを作成するための「ベストプラクティス」オプションは、一般的な推奨事項です。シャープは非常に主観的です。 これらの「ベストプラクティス」設定は、2000 x 2000 のプライマリイメージに基づいていました。大きいファイルと小さいプライマリファイルの設定は異なる場合があります。 アンシャープマスク設定を調整する場合、Adobe Dynamic Media Classicでは次の範囲を推奨しています。

* **[!UICONTROL 金額]** - .8～1.5。

* **[!UICONTROL 半径]** - .6 ～ 2。

* **[!UICONTROL しきい値]** - 1 ～ 6。

画像プリセットを削除するには、画像プリセット画面で削除する画像プリセットを選択し、「 」を選択します **[!UICONTROL 削除]**.

>[!MORELIKETHIS]
>
>* [画像プリセットの作成と編集](application-setup.md#creating_and_editing_image_presets)
>* [画像プリセットのオプション](application-setup.md#image_preset_options)
>* [画像プリセットに基づいた画像アセットのプレビュー](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
