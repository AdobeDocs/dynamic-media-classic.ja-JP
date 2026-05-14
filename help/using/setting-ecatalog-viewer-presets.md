---
title: eCatalog ビューアプリセットの設定
description: Adobe Dynamic Media ClassicでeCatalog ビューアプリセットを設定する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Viewers,Viewer Presets,eCatalog
role: User
exl-id: 4357e6b8-fbc5-4e93-9476-db92a7dc7464
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:57:04.669Z'
TQID: 'https://experienceleague.adobe.com/Ej7QeFT62FLz2hWS2w-ll2H9m2pkHXlMSJJDJTsgERg'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 483
ht-degree: 25%

---

# eCatalog ビューアプリセットの設定{#setting-up-ecatalog-viewer-presets}

eCatalog ビューアプリセットによって、eCatalog ビューアのスタイル、動作、外観が決まります。 Adobe Dynamic Media ClassicにはeCatalog ビューアプリセットが用意されており、管理者であれば、独自のeCatalog ビューアプリセットを作成することもできます。

プリセットを作成するには、最初から開始するか、Adobe Dynamic Media Classicが提供するeCatalog Viewer プリセットから開始して、新しい名前で保存します。 製本する際に、会社の特性を表し、トーンを設定できるように独自の eCatalog ビューアプリセットを作成することができます。

eCatalog ビューアプリセットには、ページからページへの移動、ズーム、検索、「スキン」の選択に関する多くの設定があります。 これらのコントロールの外観とビューアの表示方法は、eCatalog ビューアプリセットの選択によって異なります。

eCatalog ビューアプリセットを作成するには、次の手順に従います（管理者である必要があります）。

1. グローバルナビゲーションバーで、**[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**&#x200B;に移動します。
1. ビューアプリセット画面で、最初から新規に作成するか、既存の eCatalog ビューアプリセットを編集して作成する方法で、eCatalog ビューアプリセットを作成します。

   * **eCatalog ビューアプリセットを作成**:「**[!UICONTROL 追加]**」を選択します。 ビューアプリセットを追加ダイアログボックスで、プラットフォームを選択し、「eCatalog Viewer」を選択してから、「**[!UICONTROL 追加]**」を選択します。

   * **eCatalog ビューアプリセットの編集**: eCatalog ビューアプリセットを選択してから、**[!UICONTROL 編集]**&#x200B;を選択します。 プリセットの作成が完了したら、**[!UICONTROL 別名で保存]**&#x200B;を選択します。

1. `Configure Viewer` ページで、eCatalog Viewer プリセットの名前を入力します。
1. `Configure Viewer` ページで、必要なオプションを設定します。

   説明を読みたい場合は、オプションの横にある「**[!UICONTROL 情報のヒント]**」アイコンを選択します。

   プレビューページには、設定を更新および変更する際にビューアが表示されます。

1. （オプション） **[!UICONTROL 情報パネル設定]**&#x200B;で、**[!UICONTROL 情報サーバーURL]** オプションに、次の特殊トークンを含めることができます。このトークンは、ビューアによって置き換えられます。

   | トークン | 置換後 | 説明 |
   | --- | --- | --- |
   | `$1$` | rollover_key 値 | マップの`<area>`要素からの項目識別子。 |
   | `$2$` | frame | 画像セット内で現在表示されているフレームのシーケンス番号。 |
   | `$3$` | イメージルート | 画像コマンドで指定された最初の項目の最初のパス要素（通常、画像セットを指定するカタログエントリの画像カタログ ID）。 |

1. （オプション）「**[!UICONTROL 情報パネル設定]**」の「**[!UICONTROL 応答テンプレート]**」ボックスに、Adobe Dynamic Media Classicで画像マップの情報を取得する際にエラーが発生した場合に表示するテキストを入力します。 例えば、システムで会社名と eCatalog 名は取得されるが、ロールオーバー識別子は取得されない場合に、このメッセージがユーザに表示されます。

>[!NOTE]
>
>eCatalog自体で定義されたテンプレートの代わりにこの応答テンプレートを使用するには、Information Server URLの末尾に`fmt=1`を追加します。 例：`https://.../$3$/$4$/$1$/?FMT=1`。

1. **[!UICONTROL 保存]**&#x200B;を選択します。
1. 作成したeCatalog ビューアプリセットが、Web ページにeCatalogを表示するために使用されるeCatalog ビューアプリセットになるように、**[!UICONTROL Default]**&#x200B;を選択します。

eCatalog ビューアプリセットを削除するには、ビューアプリセット画面で選択し、**[!UICONTROL 削除]**&#x200B;を選択します。

>[!MORELIKETHIS]
>
>* [ビューアプリセット](application-setup.md#viewer_presets)
