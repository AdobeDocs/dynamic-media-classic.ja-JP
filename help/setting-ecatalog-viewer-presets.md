---
title: eCatalog のビューアプリセットの設定
seo-title: eCatalog のビューアプリセットの設定
description: 'null'
seo-description: eCatalogビューアプリセットを設定する方法について説明します。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
discoiquuid: 6c123f85-3bc4-4392- a7fb-55618127c65e
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# eCatalog のビューアプリセットの設定{#setting-up-ecatalog-viewer-presets}

eCatalog ビューアプリセットによって、eCatalog ビューアのスタイル、動作、外観が決まります。Dynamic Media ClassicにはeCatalogビューアプリセットがあり、管理者が独自のeCatalogビューアプリセットを作成することもできます。

新しいプリセットを作成するには、最初から最初から開始するか、Dynamic Media Classicに付属のeCatalogビューアプリセットを使用して、新しい名前で保存します。製本する際に、会社の特性を表し、トーンを設定できるように独自の eCatalog ビューアプリセットを作成することができます。

eCatalog ビューアプリセットで設定できる内容は多数あり、ページ間の移動、ズーム、検索、スキンの選択などを設定することができます。eCatalog ビューアプリセットの設定内容によって、これらのコントロールの外観と、ビューア自体の外観が決まります。

eCatalog ビューアプリセットを作成するには、以下の手順に従います（管理者のみ作成可能）。

1. **設定**／**ビューアプリセット**&#x200B;をクリックします。
1. ビューアプリセット画面で、最初から新規に作成するか、既存の eCatalog ビューアプリセットを編集して作成する方法で、eCatalog ビューアプリセットを作成します。

   **eCatalogビューアプリセットの作成「追加** 」をクリックします。In the Add Viewer Preset dialog box, choose a platform, choose eCatalog Viewer, then click **Add**.

   **eCatalogビューアプリセット** の編集eCatalogビューアプリセットを選択し、「編集」をクリックします。Click **Save As** after you finish creating the preset.

1. ビューアを設定画面で、eCatalog ビューアプリセットの名前を入力します。
1. ビューア設定画面で、目的のオプションを設定します。

   オプションの説明を表示するには、オプションに隣接する情報ヒントアイコン  をクリックします。

   設定を更新または変更すると、プレビュー画面にビューアが表示されます。

1. （オプション）情報パネルの設定では、「情報サーバの URL」オプションに次の特殊なトークンを含めることができます。このトークンはビューアによって置き換えられます。

   | トークン | 置換後 | 説明 |
   |--- |--- |--- |
   | `$1$` | rollover_key 値 | The item identifier from the `<area>` element of the map. |
   | `$2$` | frame | 画像セット内で現在表示されているフレームのシーケンス番号。 |
   | `$3$` | imageroot | 画像コマンドで指定された最初の項目の最初のパス要素（通常、画像セットを指定するカタログエントリの画像カタログ ID）。 |

1. （オプション）情報パネルの設定の「応答テンプレート」ボックスに、画像マップの情報を取得する際にエラーが発生した場合に表示するテキストを入力します。例えば、システムで会社名と eCatalog 名は取得されるが、ロールオーバー識別子は取得されない場合に、このメッセージがユーザに表示されます。

>[!NOTE]
>
>eCatalog で定義されているテンプレートの代わりにこの応答テンプレートを使用するには、「情報サーバの URL」の末尾に「fmt=1」と追加します。For example: `https://.../$3$/$4$/$1$/?FMT=1`.

1. 「**保存**」をクリックします。
1. 作成した eCatalog ビューアプリセットを Web ページ上で eCatalog の表示に使用する場合には、「初期設定」をクリックします。

To delete an eCatalog Viewer Preset, select it on the Viewer Presets screen and click **Delete**.

>[!MORELIKETHIS]
>
>* [ビューアプリセット](application-setup.md#viewer_presets)

