---
title: Adobe Analytics レポートの設定
description: Adobe Dynamic Media ClassicでAdobe Analytics レポートを設定する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '1234'
ht-degree: 18%

---

# Adobe Analytics レポートの設定{#configuring-adobe-analytics-reports}

Adobe Analytics レポートに必要な情報をAdobe Analyticsに伝えるには、Adobe Analytics設定画面に移動します。 この画面には、設定レポートに従って、情報を求めるビューアイベントごとに、対応するAdobe Analytics変数とAdobe Dynamic Media Classic変数が一覧表示されます。 これらのビューアのイベント/Adobe Analytics変数/Adobe Dynamic Media Classic変数の組み合わせによって、レポートする情報が決まります。

Adobe Analytics設定画面では、ビューアイベントを変数に関連付ける以外に、ビューアイベントをアクティベート、編集および削除するためのツールも提供しています。

>[!NOTE]
>
>Adobe Analytics内でAdobe Analytics レポートの設定を変更した場合は、必ずAdobe Dynamic Media ClassicからAdobe Analyticsに再度ログオンし、Adobe Analytics設定を再保存してから、再公開してください。

[Adobe Analyticsへのログオン ](log-analytics.md#log_in_to_adobe_analytics) を参照してください。

[Publishの設定に関する情報 ](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information) を参照してください。

## Adobe Analytics変数のAdobe Dynamic Media Classic ビューアイベントおよび変数への割り当て {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Adobe Analytics設定画面を使用して、ビューアイベントをAdobe Analytics変数とAdobe Dynamic Media Classic変数に関連付けます。 ビューアイベントごとに、1 つのAdobe Analytics変数と 1 つのAdobe Dynamic Media Classic変数を選択します。 Adobe Analytics設定画面を開く手順については、[Adobe Analyticsへのログオン ](log-analytics.md#log_in_to_adobe_analytics) を参照してください。

**Adobe Analytics変数をAdobe Dynamic Media Classic ビューアイベントと変数に割り当てるには：**

1. Dynamic Media Classic内からAdobe Analyticsにログインし、レポートスイートを選択した後、Adobe Analytics設定ページの右側のテーブル列で、「**[!UICONTROL 有効]**」を選択してビューアイベントをアクティベートします。
1. 変数列で、目的のビューアイベントの矢印ボタンを選択して変数ペア選択を表示します。

   詳しくは、[ビューアイベント](configuring-analytics-reports.md#viewer_events)を参照してください。

1. Adobe Dynamic Media Classic変数を追加します。

   [Adobe Dynamic Media Classic変数 ](configuring-analytics-reports.md#scene7_variables) を参照してください。

1. Adobe Analytics 変数を追加します。
1. （オプション）別の変数のペアを追加するには、「**[!UICONTROL 追加]**」を選択します。
1. **[!UICONTROL 保存]** を選択します。

   「**[!UICONTROL 保存]**」を選択すると、ビューアイベント、Adobe Analytics変数およびAdobe Dynamic Media Classic変数がAdobe Analytics設定画面に一覧表示されます。

1. 右下隅にある「**[!UICONTROL 閉じる]** を選択します。
1. 画像サービング公開を実行するには、**[!UICONTROL Publish]**/**[!UICONTROL Publishを送信]** に移動します。

   ビューアに含まれる情報をAdobe Dynamic Media Classic サーバーで使用できるようにするには、公開する必要があります。

### ビューアイベント {#viewer-events}

ビューアイベントは、Dynamic Media Classic ビューアでユーザーが実行するアクションを表します。 ユーザーがアクション（サムネールの選択、ビデオの開始や停止など）を開始すると、ビューアはイベントを web ページに「ブロードキャスト」します。 そのイベントに関連付けられたデータもプッシュされます。

次の表に、Adobe Analytics設定画面に追加できるビューアイベントを示します。

| ビューアイベント | HTML5 ビューアプラットフォームのサポートとビューア | 説明 |
| --- | --- | --- |
| LOAD | **X**（eCatalog、フライアウト、スピンセット、ビデオ、ズーム） | ユーザーがビューアを起動したとき |
| PAGE | **X**（eCatalog） | eCatalog では、ユーザーがページを切り替えると同時に、ターゲットズームビューアでは、ユーザーが別のターゲットやカラースウォッチを選択すると同時に回転します。 |
| SWAP | **X**（eCatalog、フライアウト、スピンセット、ビデオ、ズーム） | ユーザーが別のサムネイルを選択して別の画像を表示する場合。 |
| ITEM | **X**（eCatalog） | ロールオーバーが定義されている画像マップをサポートするビューアで、ユーザがポインタを画像マップに合わせ、ロールオーバーテキストを読むとき。 |
| HREF | **X**（eCatalog） | 画像マップをサポートするビューアで、ユーザーが画像マップ内の URL を選択したとき。 |
| TARGET | | ターゲットズームビューアで、ユーザーがズームターゲットを選択して画像の一部にズームする場合。 |
| SEARCH | | eCatalog で、ユーザが単語検索を実行したとき。 |
| PLAY | **X**（ビデオ） | ビデオビューアで、ユーザーが「再生」を選択してビデオの再生を開始したとき。<br><br>**注意：** Adobe Analytics ハートビートベースのビデオレポートを使用している場合は、Adobe Dynamic Media ClassicでAdobe Analyticsを設定するときに、このビューアイベントに変数をマッピングする必要はありません。 ビデオハートビートは、標準のAdobe Dynamic Media Classic HTML5 ビデオおよび MixedMedia ビューアで機能します。 ビデオプレーヤーは、Adobe Analytics ビデオレポート内で表示するためのトラッキングデータを生成します。 [Adobe Analytics ビデオレポートの有効化 ](enabling-analytics-video-reports.md) を参照してください。 |
| PAUSE | **X**（ビデオ） | ビデオビューアで、ユーザーが **[!UICONTROL 一時停止]** を選択してビデオを凍結したとき。<br><br>**注意：** Adobe Analytics ハートビートベースのビデオレポートを使用している場合は、Adobe Dynamic Media ClassicでAdobe Analyticsを設定するときに、このビューアイベントに変数をマッピングする必要はありません。 ビデオハートビートは、標準のAdobe Dynamic Media Classic HTML5 ビデオおよび MixedMedia ビューアで機能します。 ビデオプレーヤーは、Adobe Analytics ビデオレポート内で表示するためのトラッキングデータを生成します。 [Adobe Analytics ビデオレポートの有効化 ](enabling-analytics-video-reports.md) を参照してください。 |
| STOP | **X**（ビデオ） | ビデオビューアで、ユーザーが **[!UICONTROL 停止]** を選択してビデオの再生を停止したとき。<br><br>**注意：** Adobe Analytics ハートビートベースのビデオレポートを使用している場合は、Adobe Dynamic Media ClassicでAdobe Analyticsを設定するときに、このビューアイベントに変数をマッピングする必要はありません。 ビデオハートビートは、標準のAdobe Dynamic Media Classic HTML5 ビデオおよび MixedMedia ビューアで機能します。 ビデオプレーヤーは、Adobe Analytics ビデオレポート内で表示するためのトラッキングデータを生成します。 [Adobe Analytics ビデオレポートの有効化 ](enabling-analytics-video-reports.md) を参照してください。 |
| MILESTONE | **X**（ビデオ） | ビデオビューアでは、ユーザーがビデオを 0、25、50、75 または 100 パーセント見ると Milestone イベントが生成されます。<br><br>**注意：** Adobe Analytics ハートビートベースのビデオレポートを使用している場合は、Adobe Dynamic Media ClassicでAdobe Analyticsを設定するときに、このビューアイベントに変数をマッピングする必要はありません。 ビデオハートビートは、標準のAdobe Dynamic Media Classic HTML5 ビデオおよび MixedMedia ビューアで機能します。 ビデオプレーヤーは、Adobe Analytics ビデオレポート内で表示するためのトラッキングデータを生成します。 [Adobe Analytics ビデオレポートの有効化 ](enabling-analytics-video-reports.md) を参照してください。 |
| SWATCH | **X**（フライアウト、ズーム） | このビューアイベントは、Adobe Dynamic Media Classicのページビューアイベントにマッピングされます。 |
| ZOOM | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。 |
| PAN | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。 |
| SPIN | **X**（スピンセット） | Adobe Analytics では追跡されません。 |

### Adobe Dynamic Media Classic変数 {#scene-variables}

Adobe Analytics設定画面の各ビューアイベントについて、Adobe Analytics変数と *Adobe Dynamic Media Classic変数* を選択します。 Adobe Dynamic Media Classic変数は、レポートに対して取得できるデータを表します。 例えば、`searchTerm` 変数は、eCatalog 検索で使用されるキーワードをリストします。

次の表に、Adobe Dynamic Media Classic変数を示します。

| Adobe Dynamic Media Classic変数 | 説明 |
| --- | --- |
| asset | Adobe Dynamic Media Classic アセット ID またはビデオパスファイル。 |
| viewerId | 各種ビューアタイプに割り当てられている任意の番号。 |
| pageLabel | eCatalog でビューアが表示するページ。 |
| label | ラベル値（文字列）。 |
| frame | 画像セット内のページまたはページ参照。 |
| rollover_keyRaw | 処理された部分だけでなく、HREF 値全体。 |
| rollover_keyProc | 画像マップ内で参照されているアイテムの ID（Href イベントと Item イベントについて有効）。 |
| searchTerm | eCatalog 検索で使用される語句。 |
| timeStamp | ビデオビューアで選択した再生、停止、一時停止。 |
| progress | Milestone イベントの完了率。 |
| targetId | id 値（数値）。 |

## ビューアイベントのアクティベート、編集、削除 {#activating-editing-and-deleting-viewer-events}

Adobe Analytics 設定画面で、ビューアイベントをアクティブ化、編集および削除できます。

* **アクティベート**：アクティベートする場合は「**[!UICONTROL 有効]**」を、アクティベートを解除する場合は「**[!UICONTROL 無効]** を選択します。

* **編集**：ビューアイベントを選択して、「**[!UICONTROL 表示/編集]** 変数グレーのボタンを選択します。 Adobe Dynamic Media Classic変数とAdobe Analytics変数のドロップダウンリストで、それぞれのリストから異なる変数を選択します。 詳しくは、[Adobe Dynamic Media Classic ビューアイベントと変数へのAdobe Analytics変数の割り当て ](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables) を参照してください。

* **削除**：ビューアイベントを選択して、「**[!UICONTROL 表示/編集]** 変数グレーのボタンを選択します。 「**[!UICONTROL 削除]**」を選択します。
