---
title: 画像プリセットの設定
description: Adobe Dynamic Media Classicで画像プリセットを設定する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Image Presets
role: User
exl-id: 336802cc-b032-49b2-b2e6-d699bc997ee5
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:12:02.112Z'
TQID: 'https://experienceleague.adobe.com/a4ns4AjIZccBHisG5jIf7Wkm0iK5TNp2q4xSZit-RrQ'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 670
ht-degree: 32%

---

# 画像プリセットの設定{#setting-up-image-presets}

画像プリセットは、マクロのような定義済みのサイズおよび形式に関するコマンドの集まりであり、特定の名前が付けられて保存されています。 画像プリセットの仕組みを理解するには、Web サイトで各製品画像を500 × 500 ピクセルと150 × 150 ピクセルの2つの異なるサイズで表示する必要があるとします。 2つの画像プリセットを作成します。500 x 500 ピクセルの画像を表示する「拡大」と、150 × 150 ピクセルの画像を表示する「サムネール」と呼ばれます。 Dynamic Media画像サーバーは、「画像プリセットを拡大」および「サムネール」サイズで画像を配信するために、「画像プリセットを拡大」および「サムネール画像プリセット」の定義を検索します。 サーバは、各画像プリセットのサイズおよび形式の指定に従って画像を動的に生成します。

Adobe Dynamic Media Classicには、使用できるように既に設定されている「ベストプラクティス」画像プリセットがいくつか用意されています。 管理者は、画像プリセットも作成できます。 画像プリセットは、新規作成することも、既存のプリセットを使用して別の名前で保存することもできます。

サーバから動的に配信されるときにサイズが縮小される画像は、シャープとディテールが損なわれることがあります。 このため、各画像プリセットには、特定のサイズで配信されるときに画像を最適化するための形式制御機能が含まれています。 これらのコントロールにより、画像がWeb サイトまたはアプリケーションに配信される際に、シャープで明確に表示されます。

## 画像プリセットの作成 {#creating-an-image-preset}

会社管理者であれば、独自の画像プリセットを作成できます。 画像プリセットを作成するか、Adobe Dynamic Media Classicが提供するデフォルトの画像プリセットから開始して、編集し、新しい名前で保存できます。

**画像プリセットを作成するには：**

1. **[!UICONTROL 設定]** / **[!UICONTROL 画像プリセット]**&#x200B;に移動します。

   この画面で画像プリセット名を探して選択し、既存の画像プリセットをプレビューすることができます。 画像プリセット名を選択すると、プレビューウィンドウ内のサンプル画像のサイズと外観が変わります。

1. 次のいずれかの操作を行います。

   * **画像プリセットを作成**: **[!UICONTROL 追加]**&#x200B;を選択します。
   * **画像プリセットを編集**：作成する画像プリセットに最も近い画像プリセットを参照し、**[!UICONTROL 編集]**&#x200B;を選択します。

1. 画像プリセットの名前を入力します。
1. 高さおよび幅の値をピクセル単位で入力します。 これらの値は、画像が配信されるサイズを決定します。
1. プリセットを追加画面またはプリセットを編集画面に必要な情報を入力します。 詳しくは、[画像プリセットのオプション](application-setup.md#image_preset_options)を参照してください。

   Adobe Dynamic Media Classicでは、以下の「ベストプラクティス」オプションを推奨しています。

   * **[!UICONTROL フォーマット]**: JPEGまたは要件を満たす別のフォーマットを選択します。 すべてのWeb ブラウザーはJPEGの画像フォーマットをサポートしています。小さなファイルサイズと画質のバランスが良くなります。 ただし、JPEG画像では、非可逆圧縮方式が使用されており、圧縮設定が低すぎる場合に画像のアーティファクトが発生する可能性があります。 そのため、Adobe Dynamic Media Classicでは、圧縮画質（スライダー上）を75に設定することをお勧めします。 この設定により、小さいファイルサイズで優れた画質を得ることができます。

   * **[!UICONTROL シャープニング]**：シャープニングを選択しません（このシャープフィルターでは、**[!UICONTROL アンシャープマスク]**&#x200B;の設定よりも少ない制御が可能です）。

   * **[!UICONTROL 再サンプルモード]**: **[!UICONTROL Bi-Cubic]**&#x200B;を選択します。

   * **[!UICONTROL アンシャープマスク]** （USM）：次の設定を入力します。

   | プリセットの種類 | サイズ | 適用量 | 半径 | しきい値 |
   | --- | --- | --- | --- | --- |
   | Cross-Sell（ミニサムネール） | 75×75 | 1.5 | 0.8 | 5 |
   | Thumbnail | 150×150 | 1.1 | 1 | 5 |
   | Main | 350 × 350 | 1 | 1 | 6 |
   | Enlarge | 500 × 500 | 1.2 | 1.2 | 5 |

1. **[!UICONTROL 保存]**&#x200B;を選択します。

ここに記載されている画像プリセットを作成するためのAdobe Dynamic Media Classicの「ベストプラクティス」オプションは、一般的な推奨事項です。シャープ化は非常に主観的です。 これらの「ベストプラクティス」設定は、2000年×2000年のプライマリ画像に基づいています。大きいファイルと小さいファイルの設定は異なる場合があります。 アンシャープマスクの設定を調整する場合は、Adobe Dynamic Media Classicで次の範囲をお勧めします。

* **[!UICONTROL 金額]**: `.8` ～ `1.5`。

* **[!UICONTROL 半径]**: `.6` ～ `2`。

* **[!UICONTROL しきい値]**: `1`から`6`まで。

画像プリセットを削除するには、画像プリセット画面で選択し、**[!UICONTROL 削除]**&#x200B;を選択します。

>[!MORELIKETHIS]
>
>* [画像プリセットの作成と編集](application-setup.md#creating_and_editing_image_presets)
>* [画像プリセットオプション ](application-setup.md#image_preset_options)
>* [画像プリセットに基づく画像アセットのプレビュー](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)
