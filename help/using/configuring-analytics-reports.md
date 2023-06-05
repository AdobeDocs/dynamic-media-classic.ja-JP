---
title: Adobe Analyticsレポートの設定
description: Adobe Dynamic Media ClassicでAdobe Analyticsレポートを設定する方法を説明します。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 27%

---

# Adobe Analyticsレポートの設定{#configuring-adobe-analytics-reports}

Adobe Analyticsレポートに必要な情報をAdobe Analyticsに伝えるには、 Adobe Analytics設定画面に移動します。 レポートを設定すると、この画面には、情報を取得する各ビューアイベントに対して、対応するAdobe Analytics変数とAdobe Dynamic Media Classic変数が表示されます。 これらのビューアイベント、Adobe Analytics変数、Adobe Dynamic Media Classic変数の組み合わせによって、レポートされる情報が決まります。

Adobe Analyticsの設定画面には、ビューアイベントを変数に関連付ける以外に、ビューアイベントをアクティブ化、編集および削除するためのツールも用意されています。

>[!NOTE]
>
>Adobe Analytics内でAdobe Analyticsレポート設定を変更する場合は、必ずAdobe Dynamic Media Classic内からAdobe Analyticsに再度ログオンし、Adobe Analytics設定を再保存してから、再公開してください。

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

詳しくは、 [設定情報を公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information).

## Adobe Analytics変数をAdobe Dynamic Media Classicビューアイベントと変数に割り当てる {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Adobe Analytics設定画面を使用して、ビューアイベントをAdobe Analytics変数とAdobe Dynamic Media Classic変数に関連付けます。 ビューアイベントごとに、1 つのAdobe Analytics変数と 1 つのAdobe Dynamic Media Classic変数を選択します。 Adobe Analytics 設定画面を開く方法については、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

**Adobe Analytics変数をAdobe Dynamic Media Classicビューアのイベントと変数に割り当てるには：**

1. Adobe Dynamic Media Classic内からAdobe Analyticsにログインしてレポートスイートを選択した後、右側の表の列のAdobe Analytics設定ページで、「 **[!UICONTROL 有効にする]**.
1. 「変数」列で、目的のビューアイベントの矢印ボタンを選択して、変数ペア選択を表示します。

   詳しくは、[ビューアイベント](configuring-analytics-reports.md#viewer_events)を参照してください。

1. Adobe Dynamic Media Classic変数を追加します。

   詳しくは、 [Adobe Dynamic Media Classic変数](configuring-analytics-reports.md#scene7_variables).

1. Adobe Analytics 変数を追加します。
1. （オプション）別の変数のペアを追加するには、「 **[!UICONTROL 追加]**.
1. 選択 **[!UICONTROL 保存]**.

   次を選択した後： **[!UICONTROL 保存]**、ビューアイベント、そのAdobe Analytics変数およびそのAdobe Dynamic Media Classic変数が、Adobe Analytics設定画面に表示されます。

1. 右下隅で、「 **[!UICONTROL 閉じる]**.
1. に移動します。 **[!UICONTROL 公開]** > **[!UICONTROL 公開を送信]** 画像サービング公開を実行する場合。

   ビューアに含まれる情報をAdobe Dynamic Media Classicサーバーで利用できるようにするには、公開が必要です。

### ビューアイベント {#viewer-events}

ビューアイベントは、Adobe Dynamic Media Classicビューアでユーザーが実行するアクションを記述します。 ユーザーがサムネールの選択や、ビデオの開始または停止などの特定のアクションを開始すると、ビューアは、そのイベントに関連付けられたデータと共に、Web ページにイベントを「ブロードキャスト」します。

次の表に、 Adobe Analytics設定画面に追加できるビューアイベントを示します。

| ビューアイベント | HTML5 ビューアプラットフォームのサポートとビューア | 説明 |
| --- | --- | --- |
| LOAD | **X**（eCatalog、フライアウト、スピンセット、ビデオ、ズーム） | ユーザーがビューアを起動したとき |
| PAGE | **X**（eCatalog） | eCatalog で、ユーザがページをめくるとき。ターゲットズームビューアで、ユーザが別のターゲットまたはカラースウォッチを選択したとき。 |
| SWAP | **X**（eCatalog、フライアウト、スピンセット、ビデオ、ズーム） | ユーザが別のサムネールを選択して別の画像を表示する場合。 |
| ITEM | **X**（eCatalog） | ロールオーバーが定義されている画像マップをサポートするビューアで、ユーザがポインタを画像マップに合わせ、ロールオーバーテキストを読むとき。 |
| HREF | **X**（eCatalog） | 画像マップをサポートするビューアで、ユーザーが画像マップ内の URL を選択したとき。 |
| TARGET |  | ターゲットズームビューアで、ユーザがズームターゲットを選択して画像の一部をズームしたとき。 |
| SEARCH |  | eCatalog で、ユーザが単語検索を実行したとき。 |
| PLAY | **X**（ビデオ） | ビデオビューアで、ユーザーが「再生」を選択してビデオの再生を開始したとき。<br><br>**注意：** Adobe Analyticsハートビートベースのビデオレポートを使用している場合、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、変数をこのビューアイベントにマッピングする必要はありません。 ビデオハートビートは、標準搭載のAdobe Dynamic Media ClassicHTML5 ビデオビューアおよび MixedMedia ビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。詳しくは、 [Adobe Analyticsビデオレポートを有効にする](enabling-analytics-video-reports.md). |
| PAUSE | **X**（ビデオ） | ビデオビューアで、ユーザーが **[!UICONTROL 一時停止]** ビデオを固定する場合。<br><br>**注意：** Adobe Analyticsハートビートベースのビデオレポートを使用している場合、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、変数をこのビューアイベントにマッピングする必要はありません。 ビデオハートビートは、標準搭載のAdobe Dynamic Media ClassicHTML5 ビデオビューアおよび MixedMedia ビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。詳しくは、 [Adobe Analyticsビデオレポートを有効にする](enabling-analytics-video-reports.md). |
| STOP | **X**（ビデオ） | ビデオビューアで、ユーザーが **[!UICONTROL 停止]** ：ビデオの再生を停止します。<br><br>**注意：** Adobe Analyticsハートビートベースのビデオレポートを使用している場合、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、変数をこのビューアイベントにマッピングする必要はありません。 ビデオハートビートは、標準搭載のAdobe Dynamic Media ClassicHTML5 ビデオビューアおよび MixedMedia ビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。詳しくは、 [Adobe Analyticsビデオレポートを有効にする](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (ビデオ) | ビデオビューアでは、ユーザーがビデオを 0、25、50、75 または 100 パーセント見ると Milestone イベントが生成されます。<br><br>**注意：** Adobe Analyticsハートビートベースのビデオレポートを使用している場合、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、変数をこのビューアイベントにマッピングする必要はありません。 ビデオハートビートは、標準搭載のAdobe Dynamic Media ClassicHTML5 ビデオビューアおよび MixedMedia ビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。詳しくは、 [Adobe Analyticsビデオレポートを有効にする](enabling-analytics-video-reports.md). |
| SWATCH | **X**（フライアウト、ズーム） | このビューアイベントは、Adobe Dynamic Media Classicの PAGE ビューアイベントにマッピングされます。 |
| ZOOM | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。 |
| PAN | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。 |
| SPIN | **X**（スピンセット） | Adobe Analytics では追跡されません。 |

### Adobe Dynamic Media Classic変数 {#scene-variables}

Adobe Analytics設定画面のビューアイベントごとに、Adobe Analytics変数と *Adobe Dynamic Media Classic変数*. Adobe Dynamic Media Classic変数は、レポートに対して取得できるデータを表します。 例えば、`searchTerm` 変数は eCatalog 検索に使用されるキーワードを表示します。

次の表に、Adobe Dynamic Media Classic変数を示します。

| Adobe Dynamic Media Classic変数 | 説明 |
| --- | --- |
| asset | Adobe Dynamic Media Classicアセット ID またはビデオパスファイル。 |
| viewerId | 各種ビューアタイプに割り当てられている任意の番号。 |
| pageLabel | eCatalog でビューアが表示するページ。 |
| label | ラベル値（文字列）。 |
| frame | 画像セット内のページまたはページ参照。 |
| rollover_keyRaw | HREF 値全体（処理される部分だけではありません）。 |
| rollover_keyProc | 画像マップ内で参照されているアイテムの ID（Href イベントと Item イベントについて有効）。 |
| searchTerm | eCatalog 検索で使用される語句。 |
| timeStamp | ビデオビューアで選択された再生、停止および一時停止。 |
| progress | Milestone イベントの完了率。 |
| targetId | ID 値（数字）。 |

## ビューアイベントのアクティブ化、編集、削除 {#activating-editing-and-deleting-viewer-events}

Adobe Analytics 設定画面で、ビューアイベントをアクティブ化、編集および削除できます。

* **有効化**  — 選択 **[!UICONTROL 有効にする]** 有効にするか **[!UICONTROL 無効にする]** ：選択したビューアイベントを非アクティブ化します。

* **編集**  — ビューアイベントを選択し、「 **[!UICONTROL 表示/編集]** 変数グレーのボタン。 「 Adobe Dynamic Media Classic変数」ドロップダウンリストと「 Adobe Analytics変数」ドロップダウンリストで、それぞれのリストから異なる変数を選択します。 詳しくは、 [Adobe Dynamic Media Classicビューアイベントと変数へのAdobe Analytics変数の割り当て](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables).

* **削除**  — ビューアイベントを選択し、 **[!UICONTROL 表示/編集]** 変数グレーのボタン。 選択 **[!UICONTROL 削除]**.
