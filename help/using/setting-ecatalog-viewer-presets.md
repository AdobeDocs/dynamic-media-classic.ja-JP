---
title: eCatalog ビューアプリセットの設定
description: Adobe Dynamic Media Classicで eCatalog ビューアプリセットを設定する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 25%

---

# eCatalog ビューアプリセットの設定{#setting-up-ecatalog-viewer-presets}

eCatalog ビューアプリセットによって、eCatalog ビューアのスタイル、動作、外観が決まります。Adobe Dynamic Media Classicには eCatalog ビューアプリセットが用意されており、管理者は独自の eCatalog ビューアプリセットを作成することもできます。

プリセットを作成するには、最初から作成するか、Adobe Dynamic Media Classic提供の eCatalog ビューアプリセットから作成して、新しい名前で保存します。 製本する際に、会社の特性を表し、トーンを設定できるように独自の eCatalog ビューアプリセットを作成することができます。

eCatalog ビューアプリセットには、ページ間の移動、ズーム、検索、「スキン」の選択のための多くの設定が用意されています。 これらのコントロールの外観とビューアの表示方法は、eCatalog ビューアプリセットの選択によって異なります。

次の手順に従って eCatalog ビューアプリセットを作成します（管理者である必要があります）。

1. グローバルナビゲーションバーで、**[!UICONTROL 設定]**/**[!UICONTROL ビューアプリセット]** に移動します。
1. ビューアプリセット画面で、最初から新規に作成するか、既存の eCatalog ビューアプリセットを編集して作成する方法で、eCatalog ビューアプリセットを作成します。

   * **eCatalog ビューアプリセットの作成**:「**[!UICONTROL 追加]**」を選択します。 ビューアプリセットを追加ダイアログボックスで、プラットフォームを選択し、「eCatalog ビューア」を選択したあと、「**[!UICONTROL 追加]**」を選択します。

   * **eCatalog ビューアプリセットの編集**:eCatalog ビューアプリセットを選択し、「**[!UICONTROL 編集]** を選択します。 プリセットの作成が完了したら、「**[!UICONTROL 名前を付けて保存]**」を選択します。

1. `Configure Viewer` ページで、eCatalog ビューアプリセットの名前を入力します。
1. `Configure Viewer` ページで、必要なオプションを設定します。

   説明を読む場合は、オプションの横にある **[!UICONTROL 情報ヒント]** アイコンを選択します。

   プレビューページには、設定を更新および変更したときにビューアが表示されます。

1. （オプション） **[!UICONTROL 情報パネルの設定]** の **[!UICONTROL 情報サーバー URL]** オプションには、ビューアによって置き換えられる次の特別なトークンを含めることができます。

   | トークン | 置換後 | 説明 |
   | --- | --- | --- |
   | `$1$` | rollover_key 値 | マップの `<area>` 要素からの項目識別子。 |
   | `$2$` | frame | 画像セット内で現在表示されているフレームのシーケンス番号。 |
   | `$3$` | 画像ルート | 画像コマンドで指定された最初の項目の最初のパス要素（通常、画像セットを指定するカタログエントリの画像カタログ ID）。 |

1. （オプション） **[!UICONTROL 情報パネル設定]** の **[!UICONTROL レスポンステンプレート]** ボックスに、画像マップの情報を取得する際にAdobe Dynamic Media Classicでエラーが発生した場合に表示するテキストを入力します。 例えば、システムで会社名と eCatalog 名は取得されるが、ロールオーバー識別子は取得されない場合に、このメッセージがユーザに表示されます。

>[!NOTE]
>
>eCatalog 自体で定義されたテンプレートの代わりにこの応答テンプレートを使用するには、情報サーバーの URL の末尾に `fmt=1` を追加します。 例：`https://.../$3$/$4$/$1$/?FMT=1`。

1. **[!UICONTROL 保存]** を選択します。
1. **[!UICONTROL デフォルト]** を選択して、作成した eCatalog ビューアプリセットが、Web ページ上に eCatalog を表示するために使用されるようにします。

eCatalog ビューアプリセットを削除するには、ビューアプリセット画面でプリセットを選択して、「**[!UICONTROL 削除]**」を選択します。

>[!MORELIKETHIS]
>
>* [ビューアプリセット](application-setup.md#viewer_presets)
