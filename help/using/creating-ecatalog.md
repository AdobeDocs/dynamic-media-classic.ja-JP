---
title: eCatalog の作成
description: Adobe Dynamic Media Classicで e カタログを作成する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 30%

---

# eCatalog の作成 {#creating-an-ecatalog}

eCatalog の作成には、ページの順序付け、ページ レイアウトの選択、およびイメージ マップの描画によるページのリンクが必要です。 また、ロールオーバーとハイパーテキストのリンクデータを入力する必要があります。 このほかに、ページ番号ではなくページ名を eCatalog ビューアで表示するように目次をカスタマイズすることもできます。

## eCatalog の作成 {#create}

eCatalog には、画像ファイルとPDFファイルを含めることができます。

eCatalog を作成すると、 **[!UICONTROL 保存後の公開]** オプションは、次の方法でセットとセットのメンバーに影響します。

| 保存前に「保存後に公開」オプションを選択しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を作成するには：**

1. 以下のいずれかの手順に従って、eCatalog を作成してください。

   * **最初にファイルを選択します**：参照パネルで、「ファイル」を選択してから「」に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL eCatalog]**.

   * **eCatalog 画面から開始**：に移動します **[!UICONTROL ビルド]** > **[!UICONTROL eCatalog]**. アセットライブラリでフォルダーを選択します。 フォルダーから eCatalog ページの「ページを並べ替え」タブにファイルをドラッグします。

     >[!NOTE]
     >
     >アセットライブラリ内の項目をサムネールではなく名前で表示するには、個人設定の「初期設定のアセットライブラリビュー」で「名前」オプションを選択します。

1. eCatalog の全体的なレイアウトを選択します。を選択 **[!UICONTROL 1 つ上]** 単一ページの場合、 **[!UICONTROL 2 つ上]** ダブルページスプレッドの場合、または **[!UICONTROL カスタム]** （2 ページ以上のページスプレッドの場合）。 が含まれる **[!UICONTROL eCatalog レイアウトの変更]** ダイアログボックスで、 **[!UICONTROL すべてのスプレッド]** オプションと選択 **[!UICONTROL OK]**.
1. 必要に応じて、個々のページまたはページスプレッドを選択して選択し、レイアウトを変更します **[!UICONTROL 1 つ上]**, **[!UICONTROL 2 つ上]**、または **[!UICONTROL カスタム]** ボタン。 が含まれる **[!UICONTROL eCatalog レイアウトの変更]** ダイアログボックスで、 **[!UICONTROL 選択したスプレッド]** オプションと選択 **[!UICONTROL OK]**.
1. 必要に応じて、次の手順のいずれかに従いページの順番を変更します。

   * **ドラッグ**：ページまたはページスプレッドを新しい場所にドラッグします。 ページの移動先になる部分に縦線が表示されます。

   * **「移動先」ボタン**：ページまたはスプレッドを選択し、選択します **[!UICONTROL を次へ移動]**&#x200B;を選択し、ページを表示するメニュー上のページを選択します。

   * **シーケンス #**: リスト表示で、シーケンス #のフィールドにページ番号を入力します。

1. 作業が完了したら、ページの右下隅付近で、次のことを確認してください **[!UICONTROL 保存後の公開]** が選択されています（デフォルト）。
1. を選択 **[!UICONTROL 保存]**.
1. 保存ダイアログボックスで、eCatalog を保存するフォルダーを選択します。「ファイル名」フィールドに、スピンセット名を入力します。
1. を選択 **[!UICONTROL 保存]**.

   eCatalog は、保存後に次のオプションを選択してプレビューできます。 **[!UICONTROL プレビュー]**.

## eCatalog の編集 {#editing-an-ecatalog}

公開済みセットと非公開セットのどちらを編集した場合でも、 **[!UICONTROL 保存後の公開]** オプションは、次の方法でセットとセットのメンバーに影響します。

| セットが既に公開されているか？ | 編集を保存する前に「保存後に公開」オプションを選択しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーは、公開済みの状態を維持します。 編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を編集するには：**

1. eCatalog のロールオーバーの選択 **[!UICONTROL 編集]** ボタン。
1. 必要に応じて変更を加えます。
1. 編集が完了したら、ページの右下隅付近で、次のことを確認します **[!UICONTROL 保存後の公開]** が選択されています（デフォルト）。
1. を選択 **[!UICONTROL 保存]**&#x200B;を選択し、ストレージフォルダーを選択して、セットの名前を入力してから、 **[!UICONTROL 保存]**.

## eCatalog の削除

セットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（または「子」）は影響を受けません。代わりに、それぞれのメンバーが既存の公開済み状態または未公開状態を保持します。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を削除するには：**

1. グリッドビュー、リストビューまたは詳細ビューで、1 つ以上の eCatalog を選択します。
1. グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **[!UICONTROL 削除]**.

## 目次（TOC）のカスタマイズ {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classicは、eCatalog 画面の「ページを注文」タブで、eCatalog にデフォルトのページ番号を表示します。 ページの名前を独自に定義する場合は、目次を構成するページラベルを変更します。表紙と裏表紙には名前を付けることをお勧めします。例えば、表紙は「0-1 ページ」ではなく「表紙」と読むことができます。

eCatalog 用にカスタマイズされた目次（TOC）を手動で作成できます。 または、CSV （Macのみ）または XML ファイルからページ名を読み込むこともできます。

>[!NOTE]
>
>既定のページ タイトルを復元するには、 **[!UICONTROL ページを注文]** タブ、選択 **[!UICONTROL 目次ラベル]**&#x200B;を選択してから、 **[!UICONTROL デフォルトに戻す（すべて）]**.

### ページ名の手動入力 {#manually-entering-page-names}

eCatalog 画面の「ページを注文」タブに移動して、ページ名を 1 つずつ手動で入力します。 次に、「ページ番号」フィールドに、名前を付けるページごとに名前を入力します。

### ページ名の読み込み {#importing-page-names}

ページ名の読み込みは、eCatalog のページ数が多い場合にお勧めします。ページ名は、タブ区切りファイルまたは XML ファイルから読み込めます。

目次ラベルは、画像のユーザーデータフィールドに保存されます。このデータを次のリストとしてフォーマットします。 `name=<value>` ` pairs separated by two question marks "??" `. 例えば、という名前の目次フィールドに 1 つのラベルを設定する場合 `tocEN`画像のユーザーデータを次のように設定します。

`tocEN=&lt;EN_page_label>`

という名前の目次フィールドに別々のラベルを設定するには `tocEN` および `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

ユーザーデータフィールドをタブ区切りファイルに読み込むには、ユーザーデータのフィールドを含めます。

| IPSID | ユーザーデータ |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

ユーザーデータフィールドを XML ファイルにインポートするには、属性を含めます `vc_userdata`:

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

ページ名をタブ区切り形式または XML ファイルからインポートするには、 **[!UICONTROL 目次ラベル]** ボタンと選択 **[!UICONTROL インポート]**. メタデータをアップロードダイアログボックスで、を選択します。 **[!UICONTROL 参照]**&#x200B;を選択してから、各ページをページ名に関連付ける CSV ファイル（Macのみ）または XML ファイルを読み込みます。
