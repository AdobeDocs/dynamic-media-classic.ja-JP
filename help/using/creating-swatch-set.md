---
title: スウォッチセットの作成
description: Adobe Dynamic Media Classicでスウォッチセットを作成する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/swatch_sets
feature: Dynamic Media Classic,Viewers
role: User
exl-id: 426b6e6b-daed-4ca6-b095-99bb06604b07
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '715'
ht-degree: 49%

---

# スウォッチセットの作成{#creating-a-swatch-set}

ユーザは、スウォッチセットを使用して、様々な色、パターン、仕上げでアイテムを表示することができます。カラースウォッチを使用してスウォッチセットを作成するには、表示する色、パターン、または仕上げごとに 1 枚ずつ画像が必要です。また、色、パターン、仕上げごとに、1 つの色、1 つのパターン、1 つの仕上げが必要です。

例えば、ひさしの色が異なる帽子が 3 種類あり、ひさしの色が、レッド、グリーン、ブルーの場合を考えてみましょう。この場合、同じ帽子の 3 種類のショット（ひさしがレッドの帽子のショットが 1 枚、グリーンが 1 枚、ブルーが 1 枚）が必要です。また、レッド、グリーン、およびブルーのカラースウォッチも必要です。カラースウォッチは、ユーザーがスウォッチセットビューアで選択して、赤のつばの帽子、緑のつばの帽子または青のつばの帽子を表示するためのサムネールとして機能します。

## スウォッチセットの作成 {#create}

セットを作成すると、次のようになります **保存後の公開** オプションは、次の方法でセットとセットのメンバーに影響します。

| **[!UICONTROL 保存後の公開]** 保存前にオプションを選択しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**スウォッチセットを作成するには：**

1. 次のいずれかの操作を行います。

   * **最初に画像を選択します**：参照パネルで画像を選択し、に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL スウォッチセット]**.

   * **スウォッチセット画面から開始します**：に移動します **[!UICONTROL ビルド]** > **[!UICONTROL スウォッチセット]**. アセットライブラリでフォルダーを選択し、画像をスウォッチセットページの「ビュー」セクションにドラッグします。

1. スウォッチセットページの「スウォッチ」プレースホルダーボックスにスウォッチの色、パターンまたは仕上げをドラッグします。

   各プレースホルダにドラッグした色、パターン、仕上げのスウォッチが、隣接する画像の色、パターンまたは仕上げに一致することを確認してください。

1. スウォッチセット内の画像の順序を変更するには、画像を新しい位置にドラッグします。
1. ページの右下隅付近に、次のことを確認します **[!UICONTROL 保存後の公開]** が選択されています（デフォルト）。
1. を選択 **[!UICONTROL 保存]**&#x200B;で、カラースウォッチスウォッチセットを保存するフォルダーを選択し、セットの名前を入力して選択します。 **[!UICONTROL Submit]**.
1. スウォッチセットビューアにスウォッチセットを表示するには、次のオプションを選択します。 **[!UICONTROL プレビュー]** スウォッチセット画面で、次の操作を行います。 スウォッチセットビューアでスウォッチサムネールを選択して、その動作を確認できます。

## スウォッチセットの編集 {#editing-a-swatch-set}

公開済みセットと非公開セットのどちらを編集した場合でも、 **[!UICONTROL 保存後の公開]** オプションは、次の方法でセットとセットのメンバーに影響します。

| セットが既に公開されているか？ | **[!UICONTROL 保存後の公開]** 編集を保存する前に「保存」オプションが選択されていますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- | --- | --- | --- |
| はい | はい | 公開 | 公開済み。 |
| はい | いいえ | 公開 | 既存のセットメンバーは、公開済みの状態を維持します。 編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開済み。 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**スウォッチセットを編集するには：**

1. グリッド表示で SwatchSet を参照し、画像の下で次を選択します。 **[!UICONTROL 編集]**.
1. 次のいずれかの操作を行います。

   * 画像（公開または非公開）を追加するには、アセットを追加のフォルダーからスウォッチセットにドラッグします **[!UICONTROL ビュー]** ページ。
   * 画像を削除するには、画像を選択してから選択します **[!UICONTROL 削除]** ツールバーで上書きできます。
   * 画像を並べ替えるには、画像を別の位置にドラッグします。

1. セットの編集が完了したら、ページの右下隅付近で次のことを確認します **[!UICONTROL 保存後の公開]** が選択されています（デフォルト）。
1. を選択 **[!UICONTROL 保存]**&#x200B;を選択し、ストレージフォルダーを選択して、セットの名前を入力してから、 **[!UICONTROL 保存]**.

## スウォッチセットの削除

セットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（または「子」）は影響を受けません。代わりに、それぞれのメンバーが既存の公開済み状態または未公開状態を保持します。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**スウォッチセットを削除するには：**

1. グリッド表示、リスト表示または詳細表示で、スウォッチセットを 1 つ以上選択します。
1. グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **[!UICONTROL 削除]**.