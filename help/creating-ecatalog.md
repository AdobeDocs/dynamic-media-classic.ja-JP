---
title: eCatalog の作成
seo-title: eCatalog の作成
description: 'null'
seo-description: eCatalogの作成方法について説明します。
uuid: 2ah05c2-7052-426c- b61d-7f9091f7ace8
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK_ PK/eCatalog/eCatalog
discoiquuid: 28889c60-596a-40d2-85d4- f48a4f86b932
translation-type: tm+mt
source-git-commit: 1941567db5c154620bb0dcd12e363d7eebc61b20

---


# eCatalog の作成{#creating-an-ecatalog}

eCatalog の作成には、ページの順序を決めたり、ページレイアウトを選択したり、画像マップを描画してページをリンクしたり、ロールオーバーとハイパーテキストリンクのデータを入力するといった作業があります。このほかに、ページ番号ではなくページ名を eCatalog ビューアで表示するように目次をカスタマイズすることもできます。

## eCatalog の作成 {#create}

eCatalog には、PDF ファイルだけでなく画像ファイルも含めることができます。

eCatalog を作成する際には、「**保存後に公開**」オプションがセットおよびセットメンバーに対して次のように影響します。

| 保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- |--- |--- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を作成するには**

1. 以下のいずれかの手順に従って、eCatalog を作成してください。

   **参照パネルでファイルを選択し、ファイルを選択して、ビルド/** eCatalogをクリックします。

   **eCatalog画面から、ビルド/eCatalogを** クリックします。アセットライブラリのフォルダーを選択し、そのフォルダーから eCatalog ページの「ページ順序」タブにファイルをドラッグします。

   ***note**: To view the items in the Asset Library by name instead of thumbnail, select the Name option for Default Asset Library View in Personal Setup. *

1. eCatalog の全体的なレイアウトを選択します。見開きページの表示単位を 1 ページにする場合は 1 アップボタン 、2 ページにする場合は 2 アップボタン 、3 ページ以上にする場合はカスタムボタン  をクリックします。eCatalog レイアウトを変更ダイアログボックスが表示されます。Select the All Spreads options and click **OK**.
1. 必要に応じて、ページまたは見開きページをクリックし、1 アップボタン、2 アップボタン、カスタムボタンを選択してページ単位または見開きページ単位でレイアウトを変更することができます。eCatalog レイアウトを変更ダイアログボックスが表示されます。Select the Selected Spreads options and click **OK**.
1. 必要に応じて、次の手順のいずれかに従いページの順番を変更します。

   **ドラッグ** ページまたは見開きページを新しい位置にドラッグします。ページの移動先になる部分に縦線が表示されます。

   **移動先ボタン** をクリックしてページまたは見開きページを選択し、「移動先」ボタンをクリックして、ページの前に表示するページを選択します。

   **シーケンス#** で、シーケンス#フィールドにページ番号を入力します。

1. 操作が完了したら、ページ右下付近にある「**保存後に公開**」が選択済み（初期設定）であることを確認します。
1. 「**保存**」をクリックします。
1. 保存ダイアログボックスで、eCatalog を保存するフォルダーを選択します。「ファイル名」フィールドに、スピンセット名を入力します。
1. 「**保存**」をクリックします。

   保存が終了すると、「**プレビュー**」をクリックして、eCatalog をプレビューできるようになります。

## eCatalog の編集 {#editing-an-ecatalog}

編集するセットが公開済みか非公開かに応じて、「**保存後に公開**」オプションがセットおよびセットメンバーに対して次のように影響します。

| セットが既に公開されているか？ | 編集内容の保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- |--- |--- |--- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーは公開状態を維持します。編集中に追加した新しいセットメンバーは、公開または非公開の状態を維持します。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を編集するには**

1. eCatalog のロールオーバー時に表示される「**編集**」ボタンをクリックします。
1. 必要に応じて変更を加えます。
1. 編集が完了したら、ページ右下付近にある「**保存後に公開**」が選択済み（初期設定）であることを確認します。
1. 「**保存**」をクリックし、保存するフォルダーを選択し、セットの名前を入力して、「**保存**」をクリックします。

## eCatalog の削除 {#deleting-an-ecatalog}

セットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（「子」）は影響を受けず、それらの既存の公開または非公開の状態が維持されます。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**eCatalog を削除するには**

1. グリッドビュー、リストビューまたは詳細ビューで、1 つ以上の eCatalog を選択します。
1. グローバルナビゲーションバーで、**ファイル**／**削除**／**削除**&#x200B;をクリックします。

## 目次のカスタマイズ {#customizing-the-table-of-contents-toc}

ダイナミックメディアClassicでは、eCatalog画面の「ページ順序」タブのeCatalogに初期設定のページ番号が表示されます。ページの名前を独自に定義する場合は、目次を構成するページラベルを変更します。表紙と裏表紙には名前を付けることをお勧めします。例えば、表紙ページで"Page0-1"の代わりに"Cover"という文字を読み取ることができます。

カスタマイズした eCatalog の目次は、手動で作成するか、CSV（Mac OS のみ）または XML ファイルからページ名を読み込んで作成できます。

>[!NOTE]
>
>初期設定のページタイトルに戻す場合は、「ページ順序」タブの TOC ラベルボタンをクリックし、「初期設定を復元 (すべて)」を選択します。

### ページ名の手動入力 {#manually-entering-page-names}

ページ名を一度に 1 つずつ手動で入力するには、eCatalog 画面の「ページ順序」タブに移動し、ページ番号フィールドをクリックして名前を入力します。名前を付ける各ページの名前を入力します。

### ページ名の読み込み {#importing-page-names}

ページ名の読み込みは、eCatalog のページ数が多い場合にお勧めします。ページ名は、タブ区切りファイルまたは XML ファイルから読み込めます。

目次ラベルは、画像のユーザデータフィールドに保存されます。このデータをリストとしてフォーマット `name=<value>`` pairs separated by two question marks “??” `します。例えば、tocENという名前のTOCフィールドに1つのラベルを設定するには、画像のユーザデータを次のように設定します。

tocEN=&lt;EN_page_label&gt;

tocEN と tocFR という 2 つの TOC フィールドに別々のラベルを設定するには、次のように設定します。

tocEN=&lt;EN_page_label&gt;??tocFR=&lt;FR_page_label&gt;

ユーザデータフィールドをタブ区切りファイルに読み込むには、次のように、フィールドユーザデータを含めます。

| IPSID | Userdata |
|--- |--- |
| `<image_IPS_ID>` | tocEN=&lt;EN_page_label&gt;??tocFR=&lt;FR_page_label&gt; |

ユーザデータフィールドを XML ファイルに読み込むには、次のように、属性`vc_userdata` を含めます。

```as3
<ips> 
<ghw_object vc_objectname="<image_IPS_ID>" … vc_userdata=" tocEN=<EN_page_label>??tocFR=<FR_page_label>" … /> 
</ips>
```

タブ区切りファイルまたは XML ファイルからページ名を読み込むには、TOC ラベルボタンを選択し、「読み込み」を選択します。メタデータをアップロードダイアログボックスが表示されます。「参照」ボタンをクリックし、各ページをページ名に関連付ける CSV ファイル（Mac OS のみ）または XML ファイルを読み込みます。