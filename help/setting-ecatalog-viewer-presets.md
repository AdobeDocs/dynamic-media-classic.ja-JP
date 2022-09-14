---
title: eCatalog ビューアプリセットの設定
description: Adobe Dynamic Media Classicで eCatalog ビューアプリセットを設定する方法について説明します。
uuid: aca66bc5-8491-4d81-9a06-1d3531860a14
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 6c123f85-3bc4-4392-a7fb-55618127c65e
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 33%

---

# eCatalog ビューアプリセットの設定{#setting-up-ecatalog-viewer-presets}

eCatalog ビューアプリセットによって、eCatalog ビューアのスタイル、動作、外観が決まります。Adobe Dynamic Media Classicには eCatalog ビューアプリセットが用意されています。管理者は、独自の eCatalog ビューアプリセットを作成することもできます。

プリセットを作成するには、最初から開始するか、Adobe Dynamic Media Classicが提供する eCatalog ビューアプリセットを使用して開始し、新しい名前で保存します。 製本する際に、会社の特性を表し、トーンを設定できるように独自の eCatalog ビューアプリセットを作成することができます。

eCatalog ビューアプリセットで設定できる内容は多数あり、ページ間の移動、ズーム、検索、スキンの選択などを設定することができます。これらのコントロールの外観とビューアの表示方法は、eCatalog ビューアプリセットの選択に応じて異なります。

eCatalog ビューアプリセットを作成できるようにするには、次の手順に従います（管理者である必要があります）。

1. グローバルナビゲーションバーで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.
1. ビューアプリセット画面で、最初から新規に作成するか、既存の eCatalog ビューアプリセットを編集して作成する方法で、eCatalog ビューアプリセットを作成します。

   * **eCatalog ビューアプリセットの作成**  — 選択 **[!UICONTROL 追加]**. ビューアプリセットを追加ダイアログボックスで、プラットフォームを選択し、「eCatalog ビューア」を選択して、「 **[!UICONTROL 追加]**.

   * **eCatalog ビューアプリセットの編集** - eCatalog ビューアプリセットを選択し、「 **[!UICONTROL 編集]**. 選択 **[!UICONTROL 名前を付けて保存]** プリセットの作成が完了したら、

1. ビューアを設定画面で、eCatalog ビューアプリセットの名前を入力します。
1. ビューア設定画面で、目的のオプションを設定します。

   を選択します。 **[!UICONTROL 情報ヒント]** 説明を読む場合は、オプションの横にあるアイコンをクリックします。

   設定を更新および変更すると、プレビューページにビューアが表示されます。

1. （オプション） **[!UICONTROL 情報パネルの設定]**、 **[!UICONTROL 情報サーバ URL]** オプションには、次の特殊なトークンを含めることができます。このトークンは、ビューアによって置き換えられます。

   | トークン | 置換後 | 説明 |
   | --- | --- | --- |
   | `$1$` | rollover_key 値 | からの項目識別子 `<area>` マップの要素。 |
   | `$2$` | frame | 画像セット内で現在表示されているフレームのシーケンス番号。 |
   | `$3$` | 画像ルート | 画像コマンドで指定された最初の項目の最初のパス要素（通常、画像セットを指定するカタログエントリの画像カタログ ID）。 |

1. （オプション） **[!UICONTROL 情報パネルの設定]**、 **[!UICONTROL 応答テンプレート]** ボックスに、画像マップの情報の取得でAdobe Dynamic Media Classicにエラーが発生した場合に表示するテキストを入力します。 例えば、システムで会社名と eCatalog 名は取得されるが、ロールオーバー識別子は取得されない場合に、このメッセージがユーザに表示されます。

>[!NOTE]
>
>eCatalog 自体で定義されたテンプレートの代わりにこの応答テンプレートを使用するには、 `fmt=1` を設定します。 例： `https://.../$3$/$4$/$1$/?FMT=1`.

1. 選択 **[!UICONTROL 保存]**.
1. 選択 **[!UICONTROL デフォルト]** 作成した eCatalog ビューアプリセットを、web ページ上で eCatalog を表示するために使用するものにする場合。

eCatalog ビューアプリセットを削除するには、ビューアプリセット画面で eCatalog ビューアプリセットを選択し、「 」を選択します **[!UICONTROL 削除]**.

>[!MORELIKETHIS]
>
>* [ビューアプリセット](application-setup.md#viewer_presets)

