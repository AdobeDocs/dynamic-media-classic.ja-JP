---
title: eCatalog の作成
description: Adobe Dynamic Media Classicで eCatalog を作成する方法を説明します。
uuid: 2aff05c2-7052-426c-b61d-7f9091f7ace8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: 28889c60-596a-40d2-85d4-f48a4f86b932
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 51d411b2-b4bc-4cf6-afca-dd0ed0d219a1
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 56%

---

# eCatalog の作成 {#creating-an-ecatalog}

eCatalog の作成には、ページの順序を決めたり、ページレイアウトを選択したり、画像マップを描画してページをリンクしたり、ロールオーバーとハイパーテキストリンクのデータを入力するといった作業があります。このほかに、ページ番号ではなくページ名を eCatalog ビューアで表示するように目次をカスタマイズすることもできます。

## eCatalog の作成 {#create}

eCatalog には、画像ファイルとPDFファイルを含めることができます。

eCatalog を作成する際には、「**[!UICONTROL 保存後に公開]**」オプションがセットおよびセットメンバーに対して次のように影響します。

| 保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を作成するには:**

1. 以下のいずれかの手順に従って、eCatalog を作成してください。

   * **最初にファイルを選択**  — 参照パネルで、ファイルを選択し、に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL eCatalogs]**.

   * **eCatalog 画面から開始**  — に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL eCatalogs]**. アセットライブラリのフォルダーを選択し、そのフォルダーから eCatalog ページの「ページ順序」タブにファイルをドラッグします。

      >[!NOTE]
      >
      >アセットライブラリ内の項目をサムネールではなく名前で表示するには、個人設定の「初期設定のアセットライブラリビュー」で「名前」オプションを選択します。

1. eCatalog の全体的なレイアウトを選択します。選択 **[!UICONTROL 1 アップ]** （単一ページの場合） **[!UICONTROL 2 アップ]** 見開き 2 ページ、または **[!UICONTROL カスタム]** 2 ページを超えるページスプレッド用。 内 **[!UICONTROL eCatalog レイアウトの変更]** ダイアログボックスで、 **[!UICONTROL すべてのスプレッド]** オプションと選択 **[!UICONTROL OK]**.
1. 必要に応じて、個々のページまたはページスプレッドを選択し、次に **[!UICONTROL 1 アップ]**, **[!UICONTROL 2 アップ]**&#x200B;または **[!UICONTROL カスタム]** 」ボタンをクリックします。 内 **[!UICONTROL eCatalog レイアウトの変更]** ダイアログボックスで、 **[!UICONTROL 選択したスプレッド]** オプションと選択 **[!UICONTROL OK]**.
1. 必要に応じて、次の手順のいずれかに従いページの順番を変更します。

   * **ドラッグ中**  — ページまたは見開きページを新しい場所にドラッグします。 ページの移動先になる部分に縦線が表示されます。

   * **移動先ボタン**  — ページまたはページ見開きを選択し、 **[!UICONTROL 移動先]**&#x200B;をクリックし、前にページを表示するメニューのページを選択します。

   * **シーケンス#**  — リスト表示で、「シーケンス番号」フィールドにページ番号を入力します。

1. 操作が完了したら、ページ右下付近にある「**[!UICONTROL 保存後に公開]**」が選択済み（初期設定）であることを確認します。
1. 選択 **[!UICONTROL 保存]**.
1. 保存ダイアログボックスで、eCatalog を保存するフォルダーを選択します。「ファイル名」フィールドに、スピンセット名を入力します。
1. 選択 **[!UICONTROL 保存]**.

   eCatalog を保存した後で、「 」を選択して、eCatalog をプレビューできます。 **[!UICONTROL プレビュー]**.

## eCatalog を編集 {#editing-an-ecatalog}

公開済みセットと非公開セットのどちらを編集する場合でも、 **[!UICONTROL 保存後に公開]** このオプションは、次の方法でセットおよびセットメンバーに影響します。

| セットが既に公開されているか？ | 編集内容の保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーの公開状態が維持される。編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を編集するには:**

1. eCatalog のロールオーバーを選択 **[!UICONTROL 編集]** 」ボタンをクリックします。
1. 必要に応じて変更を加えます。
1. 編集が完了したら、ページ右下付近にある「**[!UICONTROL 保存後に公開]**」が選択済み（初期設定）であることを確認します。
1. 選択 **[!UICONTROL 保存]**、ストレージフォルダーを選択し、セットの名前を入力して、「 」を選択します。 **[!UICONTROL 保存]**.

## eCatalog の削除 {#deleting-an-ecatalog}

セットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（「子」）は影響を受けず、それらの既存の公開または非公開の状態が維持されます。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を削除するには:**

1. グリッドビュー、リストビューまたは詳細ビューで、1 つ以上の eCatalog を選択します。
1. グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **[!UICONTROL 削除]**.

## 目次のカスタマイズ (TOC) {#customizing-the-table-of-contents-toc}

Adobe Dynamic Media Classicは、eCatalog 画面の「ページを並べ替え」タブにある eCatalog にデフォルトのページ番号を提供します。 ページの名前を独自に定義する場合は、目次を構成するページラベルを変更します。表紙と裏表紙には名前を付けることをお勧めします。例えば、表紙には、「0-1 ページ」ではなく「表紙」を読み取ることができます。

カスタマイズした eCatalog の目次は、手動で作成するか、CSV（Mac OS のみ）または XML ファイルからページ名を読み込んで作成できます。

>[!NOTE]
>
>ページのタイトルをデフォルトに戻すには、 **[!UICONTROL ページを並べ替え]** タブ、選択 **[!UICONTROL TOC ラベル]**&#x200B;を選択し、 **[!UICONTROL デフォルトに戻す（すべて）]**.

### ページ名の手動入力 {#manually-entering-page-names}

ページ名を一度に 1 つずつ手動で入力するには、eCatalog 画面の「ページ順序」タブに移動し、次に、「ページ番号」フィールドに、名前を付ける各ページの名前を入力します。

### ページ名を読み込む {#importing-page-names}

ページ名の読み込みは、eCatalog のページ数が多い場合にお勧めします。ページ名は、タブ区切りファイルまたは XML ファイルから読み込めます。

TOC ラベルは、画像の「ユーザーデータ」フィールドに格納されます。このデータをのリストとしてフォーマット `name=<value>` ` pairs separated by two question marks “??” `. 例えば、`tocEN` という名前の TOC フィールドに 1 つのラベルを設定するには、画像のユーザデータを次のように設定します。

`tocEN=&lt;EN_page_label>`

TOC フィールドに別々のラベルを設定するには `tocEN` および `tocFR`:

`tocEN=&lt;EN_page_label>??tocFR=&lt;FR_page_label>`

「ユーザーデータ」フィールドをタブ区切りファイルにインポートするには、次のようにフィールドユーザーデータを含めます。

| IPSID | ユーザーデータ |
| --- | --- |
| `<image_IPS_ID>` | `tocEN=<EN_page_label>??tocFR=<FR_page_label>` |

ユーザデータフィールドを XML ファイルに読み込むには、次のように、属性`vc_userdata` を含めます。

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

タブ区切りファイルまたは XML ファイルからページ名を読み込むには、 **[!UICONTROL TOC ラベル]** ボタンと選択 **[!UICONTROL インポート]**. メタデータをアップロードダイアログボックスで、「 **[!UICONTROL 参照]**&#x200B;をクリックし、各ページをページ名に関連付ける CSV ファイル (Macのみ ) または XML ファイルを読み込みます。
