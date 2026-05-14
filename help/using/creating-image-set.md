---
title: 画像セットの作成
description: Adobe Dynamic Media Classicで画像セットを作成する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets,Spin Sets
role: User
exl-id: c18bb98c-b087-45d0-a4c9-44f58a3b514f
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:41:43.308Z'
TQID: 'https://experienceleague.adobe.com/W8HyE6-6ofFJRUWa37n9XnVAeXDkQ8ycBY-hna1ArAY'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 679
ht-degree: 39%

---

# 画像セットの作成{#creating-an-image-set}

複数ビューの画像セットを作成するには、1 つのアイテムを異なる視点から表示する画像または同じアイテムの異なる側面を表示する画像が必要です。 最終的な目標は、閲覧者がアイテムの外観や動作を十分に把握できるように、アイテムの画像を表示することです。

## 画像セットの作成 {#create}

セットを作成する場合、保存&#x200B;]**後に**[!UICONTROL &#x200B;公開オプションは、次の方法でセットとセットメンバーに影響を与えます。

| 保存する前に&#x200B;**[!UICONTROL `Publish after a save`]** オプションを選択しました？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

画像セットを作成する場合、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| 制限タイプ | ベストプラクティス | 制限が適用されました |
| --- | --- | --- |
| セットあたりの重複アセットの数 | 重複なし | 20‡ |
| 1 セットあたりの最大画像数 | 5～10枚/セット | 1000 |

‡ベストプラクティスは、セット内に重複するアセットを含めないことです。 1つのアセットに対する重複の数は20件までです。 セット内で、そのアセットに別の重複を追加した場合、リクエストはエラーを与えるか、重複を無視します。

[Dynamic Mediaの制限](/help/using/limitations.md)も参照してください。

**画像セットを作成するには：**

1. 次のいずれかの操作を行います。

   * **最初に画像を選択**：参照パネルで、画像セットに使用する画像を選択し、**[!UICONTROL ビルド]** > **[!UICONTROL 画像セット]**&#x200B;に移動します。

   * **画像セット画面から開始**: **[!UICONTROL ビルド]** > **[!UICONTROL 画像セット]**&#x200B;に移動します。 画像セット画面が開きます。 アセットライブラリでフォルダを選択し、画像セットに使用する画像を画像セット画面にドラッグします。

1. 画像の順序を変更するには、画像を別の場所にドラッグします。
1. ページの右下隅付近で、保存&#x200B;]**が選択された後に**[!UICONTROL &#x200B;公開することを確認します（デフォルト）。
1. **[!UICONTROL 保存]**&#x200B;を選択し、画像セットを保存するフォルダーを選択し、セットの名前を入力してから、**[!UICONTROL 保存]**&#x200B;を選択します。
1. 画像セットビューアで画像セットを表示するには、画像セット画面で「**[!UICONTROL プレビュー]**」を選択します。 画像セットビューアでスウォッチサムネールを選択して、その動作を確認できます。

## 画像セットの編集 {#editing-an-image-set}

公開済みセットと非公開セットのどちらを編集する場合でも、保存&#x200B;]**後に**[!UICONTROL &#x200B;公開オプションは、次の方法でセットとセットメンバーに影響を与えます。

| セットが既に公開されているか？ | 編集を保存する前に&#x200B;**[!UICONTROL `Publish after a save`]** オプションを選択しましたか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーの公開状態が維持される。 編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**画像セットを編集するには：**

1. グリッド表示でImageSetを参照し、画像の下にある「**[!UICONTROL 編集]**」を選択します。
1. 次のいずれかの操作を行います。

   * 画像を追加（公開または非公開）するには、Assetsを追加のフォルダーから画像セットの&#x200B;**[!UICONTROL ビュー]** ページに画像をドラッグします。
   * 画像を削除するには、画像を選択し、ツールバーの&#x200B;**[!UICONTROL 削除]**&#x200B;を選択します。
   * 画像を並べ替えるには、画像を別の位置にドラッグします。

1. セットの編集が完了したら、ページの右下隅付近で、保存&#x200B;]**が選択された後に**[!UICONTROL &#x200B;公開することを確認します（デフォルト）。
1. **[!UICONTROL 保存]**&#x200B;を選択し、セットのストレージフォルダーを選択し、セットの名前を入力してから、**[!UICONTROL 保存]**&#x200B;を選択します。

## 画像セットの削除

セットを削除すると、そのセット自体はごみ箱に移されます。 ただし、そのセット内のメンバー（または「子」）は影響を受けません。代わりに、それぞれが既存の公開済みまたは未公開状態を保持します。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**画像セットを削除するには：**

1. グリッド表示、リスト表示または詳細表示で、1つ以上の画像セットを選択します。
1. グローバルナビゲーションバーで、**[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **[!UICONTROL 削除]**&#x200B;に移動します。
