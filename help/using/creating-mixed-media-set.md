---
title: 混在メディアセットの作成
description: Adobe Dynamic Media Classicで混在メディアセットを作成する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 18669c65-a1c4-4012-8587-cd5095f4bd4e
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 56%

---

# 混在メディアセットの作成{#creating-a-mixed-media-set}

混在メディアセットは、複数のタイプのビューアを 1 つの表示に組み合わせる場合に作成します。混在メディアセットに追加するファイル、画像セット、スウォッチセットおよびスピンセットは、公開できる状態になっている必要があります。

![混在メディアセット](/help/using/assets/mm_mixed_media_set.png)

## 混在メディアセットの作成 {#create-a-mixed-media-set}

セットを作成すると、次のようになります **保存後の公開** オプションは、次の方法でセットとセットのメンバーに影響します。

| 保存前に「保存後に公開」オプションを選択しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**混在メディアセットを作成するには：:**

1. に移動 **[!UICONTROL ビルド]** > **[!UICONTROL 混在メディアセット]**.
1. ビデオ、画像セット、スピンセットおよびスウォッチを、アセットライブラリから混在メディアセット画面にドラッグします。

   >[!NOTE]
   >
   >混在メディアセットは、次のいずれかの文字を含むファイル名のアセットをサポートしていません。 `( ) { }`.

1. 次のいずれかの操作を行います。

   * サウンドトラックを追加するには、オーディオファイルをアセットライブラリから「サウンドトラック」ボックスにドラッグします。サウンドトラックは、画像が表示されている間、再生されます。ビデオの再生中に停止します。
   * セットの順序を変更するには、混在メディアセット画面でそのセットを新しい位置までドラッグします。画面上のセットの順序によって、混在メディアセットビューアで左から右に表示される順序が決まります。
   * （オプション）ビューアでビデオを表すカスタムサムネールを追加するには、アセットライブラリから「サムネール」プレースホルダボックスに画像ファイルをドラッグします。

1. ページの右下隅付近に、次のことを確認します **[!UICONTROL 保存後の公開]** が選択されています（デフォルト）。
1. を選択 **[!UICONTROL 保存]**.
1. 混在メディアセットを保存するフォルダーを選択し、セットの名前を入力します。
1. を選択 **[!UICONTROL 保存]**.

   画像セットビューアでコンボ画像セットがどのように表示されるかを確認するには、以下を選択します。 **[!UICONTROL プレビュー]**.

## 混在メディアセットの編集 {#edit-a-mixed-media-set}

混在メディアセットは編集することができます。混在メディアセット内のセットを編集するには、そのセットを別個に開き、編集して保存すると、編集内容は混在メディアセットに表示されます。

公開済みセットと非公開セットのどちらを編集した場合でも、 **[!UICONTROL 保存後の公開]** オプションは、次の方法でセットとセットのメンバーに影響します。

| セットが既に公開されているか？ | **[!UICONTROL 保存後の公開]** 編集を保存する前に選択したオプション | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- |--- |--- |--- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーは、公開済みの状態を維持します。 編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**混在メディアセットを編集するには：:**

1. 混在メディアセットのロールオーバーの選択 **[!UICONTROL 編集]** ボタン。
1. 次のいずれかの操作を行います。

   * 項目を削除するには、項目を選択して次を選択します **[!UICONTROL 削除]**.
   * 項目を並べ替えるには、項目を新しい位置にドラッグします。

1. セットの編集が完了したら、ページの右下隅付近で次のことを確認します **[!UICONTROL 保存後の公開]** が選択されています（デフォルト）。
1. を選択 **[!UICONTROL 保存]** または **[!UICONTROL 名前を付けて保存]**.

## 混在メディアセットの削除

セットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（または「子」）は影響を受けません。代わりに、それぞれのメンバーが既存の公開済み状態または未公開状態を保持します。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**混在メディアセットを削除するには：:**

1. グリッドビュー、リストビューまたは詳細ビューで、1 つ以上の混在メディアセットを選択します。
1. グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **[!UICONTROL 削除]**.
