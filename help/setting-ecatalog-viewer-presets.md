---
title: eCatalog のビューアプリセットの設定
description: eCatalogビューアプリセットを設定する方法を説明します。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Mediaクラシック，ビューア，ビューアプリセット，eCatalog
role: Business Practitioner
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
translation-type: tm+mt
source-git-commit: 6f3801a71dd2a5f162acacf7d8199dbf8c3520f7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 41%

---

# eCatalog のビューアプリセットの設定{#setting-up-ecatalog-viewer-presets}

eCatalog ビューアプリセットによって、eCatalog ビューアのスタイル、動作、外観が決まります。eCatalogビューアプリセットはDynamic Mediaクラシックに用意されており、管理者は独自のeCatalogビューアプリセットを作成することもできます。

プリセットを作成するには、Dynamic Mediaクラシックが提供するeCatalogビューアプリセットを使用して、ゼロまたは開始から開始し、新しい名前で保存します。 製本する際に、会社の特性を表し、トーンを設定できるように独自の eCatalog ビューアプリセットを作成することができます。

eCatalog ビューアプリセットで設定できる内容は多数あり、ページ間の移動、ズーム、検索、スキンの選択などを設定することができます。eCatalogビューアプリセットの設定内容に応じて、これらのコントロールの外観とビューアの表示方法が変わります。

eCatalogビューアプリセットを作成するには、次の手順に従います（管理者のみ作成できます）。

1. グローバルナビゲーションバーで、**[!UICONTROL 設定]**/**[!UICONTROL ビューアプリセット]**&#x200B;をクリックします。
1. ビューアプリセット画面で、最初から新規に作成するか、既存の eCatalog ビューアプリセットを編集して作成する方法で、eCatalog ビューアプリセットを作成します。

   * **eCatalogビューアプリセットの作成**  — クリック **[!UICONTROL 追加]**。ビューアプ追加リセットダイアログボックスで、プラットフォームを選択し、「eCatalogビューア」を選択して、「**[!UICONTROL 追加]**」をクリックします。

   * **eCatalogビューアプリセットの編集** - eCatalogビューアプリセットを選択し、「編集」をクリックします。プリセットの作成が完了したら、「**[!UICONTROL 名前を付けて保存]**」をクリックします。

1. ビューアを設定画面で、eCatalog ビューアプリセットの名前を入力します。
1. ビューア設定画面で、目的のオプションを設定します。

   オプションの説明を読むには、オプションの横にある&#x200B;**[!UICONTROL 情報ヒント]**&#x200B;アイコンをクリックします。

   設定を更新および変更すると、プレビューページにビューアが表示されます。

1. （オプション）**[!UICONTROL 情報パネルの設定]**&#x200B;では、**[!UICONTROL 情報サーバのURL]**&#x200B;オプションに次の特殊なトークンを含めることができます。このトークンはビューアによって置き換えられます。

   | トークン | 置換後 | 説明 |
   |--- |--- |--- |
   | `$1$` | rollover_key 値 | マップの`<area>`要素の項目識別子。 |
   | `$2$` | frame | 画像セット内で現在表示されているフレームのシーケンス番号。 |
   | `$3$` | imageroot | 画像コマンドで指定された最初の項目の最初のパス要素（通常、画像セットを指定するカタログエントリの画像カタログ ID）。 |

1. （オプション）**[!UICONTROL 情報パネルの設定]**&#x200B;の「**[!UICONTROL 応答テンプレート]**」ボックスに、画像マップの情報を取得する際にエラーが発生した場合に表示するテキストを入力します。 例えば、システムで会社名と eCatalog 名は取得されるが、ロールオーバー識別子は取得されない場合に、このメッセージがユーザに表示されます。

>[!NOTE]
>
>eCatalogで定義されているテンプレートの代わりにこの応答テンプレートを使用するには、情報サーバのURLの末尾に`fmt=1`を追加します。 次に例を示します。`https://.../$3$/$4$/$1$/?FMT=1`.

1. 「**保存**」をクリックします。
1. 作成した eCatalog ビューアプリセットを Web ページ上で eCatalog の表示に使用する場合には、「初期設定」をクリックします。

eCatalogビューアプリセットを削除するには、ビューアプリセット画面でeCatalogビューアプリセットを選択し、「**[!UICONTROL 削除]**」をクリックします。

>[!MORELIKETHIS]
>
>* [ビューアプリセット](application-setup.md#viewer_presets)

