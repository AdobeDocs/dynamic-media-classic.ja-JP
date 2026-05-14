---
title: eCatalogの作成
description: Adobe Dynamic Media Classicでe カタログを作成する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T17:43:46.184Z'
TQID: 'https://experienceleague.adobe.com/wNCmgUez4XtC2sJFmMQvlsczy2r-TxFsDXzrzACGNXc'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 990
ht-degree: 31%

---

# eCatalog の作成 {#creating-an-ecatalog}

eCatalogを作成するには、ページの順序、ページレイアウトの選択、画像マップを描画してページをリンクさせる必要があります。 また、ロールオーバーとハイパーテキストリンクのデータを入力する必要があります。 このほかに、ページ番号ではなくページ名を eCatalog ビューアで表示するように目次をカスタマイズすることもできます。

## eCatalogの作成 {#create}

eCatalogには、画像ファイルとPDF ファイルを含めることができます。

eCatalogを作成する場合、保存&#x200B;**後に**&#x200B;公開オプションは、次の方法でセットおよびセットメンバーに影響を与えます。

| 保存前に「保存後に公開」オプションを選択した場合 | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalogを作成するには：**

1. 以下のいずれかの手順に従って、eCatalog を作成してください。

   * **最初にファイルを選択**：参照パネルでファイルを選択し、**[!UICONTROL ビルド]**/**[!UICONTROL eCatalogs]**&#x200B;に移動します。

   * **eCatalog画面から開始**: **[!UICONTROL ビルド]** > **[!UICONTROL eCatalogs]**&#x200B;に移動します。 アセットライブラリでフォルダーを選択します。 フォルダーからeCatalog ページの「注文ページ」タブにファイルをドラッグします。

     >[!NOTE]
     >
     >アセットライブラリ内の項目をサムネールではなく名前で表示するには、個人設定の「初期設定のアセットライブラリビュー」で「名前」オプションを選択します。

1. eCatalog の全体的なレイアウトを選択します。 単一ページの場合は&#x200B;**[!UICONTROL 1 Up]**、二重ページのスプレッドの場合は&#x200B;**[!UICONTROL 2 Up]**、2 ページを超えるページのスプレッドの場合は&#x200B;**[!UICONTROL Custom]**&#x200B;を選択します。 **[!UICONTROL eCatalog レイアウトの変更]** ダイアログボックスで、**[!UICONTROL すべてのスプレッド]** オプションを選択し、**[!UICONTROL OK]**&#x200B;を選択します。
1. 必要に応じて、個々のページまたはページスプレッドのレイアウトを変更するには、ページを選択し、「**[!UICONTROL 1 Up]**」、「**[!UICONTROL 2 Up]**」、「**[!UICONTROL Custom]**」ボタンを選択します。 **[!UICONTROL eCatalog レイアウトの変更]** ダイアログボックスで、**[!UICONTROL 選択したスプレッド]** オプションを選択し、**[!UICONTROL OK]**&#x200B;を選択します。
1. 必要に応じて、次の手順のいずれかに従いページの順番を変更します。

   * **ドラッグ**: ページまたはページのスプレッドを新しい場所にドラッグします。 ページの移動先になる部分に縦線が表示されます。

   * **移動先ボタン**: ページまたはページスプレッドを選択し、**[!UICONTROL 移動先]**&#x200B;を選択して、ページを表示するメニューのページを選択します。

   * **シーケンス#**: リスト表示で、シーケンス#のフィールドにページ番号を入力します。

1. 完了したら、ページの右下隅付近で、保存&#x200B;**が選択された後に**&#x200B;公開することを確認します（デフォルト）。
1. **[!UICONTROL 保存]**&#x200B;を選択します。
1. 保存ダイアログボックスで、eCatalog を保存するフォルダーを選択します。 「ファイル名」フィールドに、スピンセット名を入力します。
1. **[!UICONTROL 保存]**&#x200B;を選択します。

   eCatalogを保存した後、「**[!UICONTROL プレビュー]**」を選択してプレビューできます。

## eCatalogの編集 {#editing-an-ecatalog}

公開済みセットを編集する場合でも、非公開セットを編集する場合でも、**[!UICONTROL 保存した後に公開]** オプションは、次の方法でセットとセットメンバーに影響します。

| セットが既に公開されているか？ | 編集内容を保存する前に「保存後に公開」オプションを選択していますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーの公開状態が維持される。 編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalogを編集するには：**

1. eCatalogのロールオーバー&#x200B;**[!UICONTROL 編集]** ボタンを選択します。
1. 必要に応じて変更を加えます。
1. 編集が完了したら、ページの右下隅付近で、保存&#x200B;**が選択された後に**&#x200B;公開することを確認します（デフォルト）。
1. **[!UICONTROL 保存]**&#x200B;を選択し、ストレージフォルダーを選択し、セットの名前を入力してから、**[!UICONTROL 保存]**&#x200B;を選択します。

## eCatalogの削除

セットを削除すると、そのセット自体はごみ箱に移されます。 ただし、そのセット内のメンバー（または「子」）は影響を受けません。代わりに、それぞれが既存の公開済みまたは未公開状態を保持します。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalogを削除するには：**

1. グリッドビュー、リストビューまたは詳細ビューで、1 つ以上の eCatalog を選択します。
1. グローバルナビゲーションバーで、**[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **[!UICONTROL 削除]**&#x200B;に移動します。

## 目次のカスタマイズ {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classicでは、eCatalog画面の「注文ページ」タブに、eCatalogのデフォルトのページ番号が表示されます。 ページの名前を独自に定義する場合は、目次を構成するページラベルを変更します。 表紙と裏表紙には名前を付けることをお勧めします。 例えば、表紙のページでは、「Page 0-1」ではなく「Cover」を読み取ることができます。

eCatalog用にカスタマイズされた目次（TOC）を手動で作成できます。 または、CSV （Macのみ）またはXML ファイルからページ名を読み込むことができます。

>[!NOTE]
>
>デフォルトのページタイトルを復元するには、「**[!UICONTROL 注文ページ]**」タブで「**[!UICONTROL 目次ラベル]**」を選択し、「**[!UICONTROL デフォルトの復元（すべて）]**」を選択します。

### ページ名の手動入力 {#manually-entering-page-names}

eCatalog画面の「注文ページ」タブに移動して、ページ名を手動で1つずつ入力します。 次に、「ページ番号」フィールドに、名前を付ける各ページの名前を入力します。

### ページ名の読み込み {#importing-page-names}

ページ名の読み込みは、eCatalog のページ数が多い場合にお勧めします。 ページ名は、タブ区切りファイルまたは XML ファイルから読み込めます。

目次ラベルは、画像のユーザーデータフィールドに保存されます。このデータは`name=<value>` ` pairs separated by two question marks "??" `のリストとして書式設定されます。 例えば、`tocEN`という名前の目次フィールドに1つのラベルを設定するには、画像のユーザーデータを次のように設定します。

`tocEN=&lt;EN_page_label>`

`tocEN`および`tocFR`という名前の目次フィールドに個別のラベルを設定するには：

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

タブ区切りファイルにユーザーデータフィールドを読み込むには、フィールドユーザーデータを含めます。

| IPSID | ユーザーデータ |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

XML ファイルにユーザーデータ フィールドを読み込むには、属性`vc_userdata`を含めます。

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

タブ区切りまたはXML ファイルからページ名を読み込むには、**[!UICONTROL 目次ラベル]** ボタンを選択し、**[!UICONTROL 読み込み]**&#x200B;を選択します。 メタデータをアップロードダイアログボックスで、**[!UICONTROL 参照]**&#x200B;を選択し、各ページをページ名に関連付けるCSV ファイル（Macのみ）またはXML ファイルを読み込みます。
