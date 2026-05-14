---
title: Adobe Analytics レポートの設定
description: Adobe Dynamic Media ClassicでAdobe Analytics レポートを設定する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T17:43:06.354Z'
TQID: 'https://experienceleague.adobe.com/GiljiYJVAfOfWB78ZruSnTP01haCDv9fLKESpq7t5YA'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 1251
ht-degree: 20%

---

# Adobe Analytics レポートの設定{#configuring-adobe-analytics-reports}

Adobe AnalyticsにAdobe Analytics レポートに必要な情報を伝えるには、Adobe Analyticsの設定画面に移動します。 この画面では、設定レポートに従って、対応するAdobe Analytics変数とAdobe Dynamic Media Classic変数の情報を必要とする各ビューアイベントが一覧表示されます。 これらのビューアーイベント、Adobe Analytics変数、Adobe Dynamic Media Classic変数の組み合わせにより、報告される情報が決まります。

ビューア イベントを変数に関連付けるだけでなく、Adobe Analyticsの設定画面には、ビューア イベントをアクティブ化、編集、削除するためのツールが表示されます。

>[!NOTE]
>
>Adobe Analytics内でAdobe Analytics レポートの設定を変更する場合は、必ずAdobe Dynamic Media Classic内からAdobe Analyticsにログオンし、Adobe Analyticsの設定を再保存してから再公開してください。

[Adobe Analyticsにログオンする](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

[構成情報の公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

## Adobe Dynamic Media Classic ビューアのイベントおよび変数へのAdobe Analytics変数の割り当て {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Adobe Analytics設定画面を使用して、ビューアイベントをAdobe Analytics変数およびAdobe Dynamic Media Classic変数に関連付けます。 各ビューアーイベントに対して、1つのAdobe Analytics変数と1つのAdobe Dynamic Media Classic変数を選択します。 Adobe Analytics Configuration画面を開く方法については、[Adobe Analyticsへのログオン &#x200B;](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

**Adobe Dynamic Media Classic ビューアのイベントと変数にAdobe Analytics変数を割り当てるには：**

1. Dynamic Media Classic内からAdobe Analyticsにログインし、レポートスイートを選択した後、Adobe Analytics設定ページの右側のテーブル列で、**[!UICONTROL 有効]**&#x200B;を選択してビューアイベントをアクティブ化します。
1. 「変数」列の下に、目的のビューアイベントの矢印ボタンを選択して、変数ペアの選択ツールを表示します。

   詳しくは、[ビューアイベント](configuring-analytics-reports.md#viewer_events)を参照してください。

1. Adobe Dynamic Media Classic変数を追加します。

   [Adobe Dynamic Media Classic変数](configuring-analytics-reports.md#scene7_variables)を参照してください。

1. Adobe Analytics 変数を追加します。
1. （オプション）別の変数ペアを追加するには、**[!UICONTROL 追加]**&#x200B;を選択します。
1. **[!UICONTROL 保存]**&#x200B;を選択します。

   **[!UICONTROL Save]**&#x200B;を選択すると、ビューアイベント、そのAdobe Analytics変数、およびそのAdobe Dynamic Media Classic変数がAdobe Analytics Configuration画面に表示されます。

1. 右下隅で、**[!UICONTROL 閉じる]**&#x200B;を選択します。
1. **[!UICONTROL パブリッシュ]** / **[!UICONTROL パブリッシュを送信]**&#x200B;に移動して、画像サービング パブリッシュを実行します。

   ビューアに含まれる情報をAdobe Dynamic Media Classic サーバーで利用できるようにするには、公開が必要です。

### ビューアイベント {#viewer-events}

Viewer イベントは、Dynamic Media Classic ビューアでユーザーが実行するアクションを表します。 ユーザーがサムネールの選択やビデオの開始または停止などのアクションを開始すると、ビューアはWeb ページにイベントを「ブロードキャスト」します。 そのイベントに関連するデータもプッシュされます。

次の表に、Adobe Analytics Configuration画面に追加できるビューアイベントを示します。

| ビューアイベント | HTML5 ビューアプラットフォームのサポートとビューア | 説明 |
| --- | --- | --- |
| LOAD | **X**（eCatalog、フライアウト、スピンセット、ビデオ、ズーム） | ユーザーがビューアを開始すると |
| PAGE | **X**（eCatalog） | eCatalogsでは、ユーザーがページを切り替える場合、ターゲットズームビューアでは、ユーザーが別のターゲットまたはカラースウォッチを選択する場合。 |
| SWAP | **X**（eCatalog、フライアウト、スピンセット、ビデオ、ズーム） | ユーザーが別のサムネールを選択すると、別の画像が表示されます。 |
| ITEM | **X**（eCatalog） | ロールオーバーが定義されている画像マップをサポートするビューアで、ユーザがポインタを画像マップに合わせ、ロールオーバーテキストを読むとき。 |
| HREF | **X**（eCatalog） | 画像マップをサポートするビューアで、ユーザーが画像マップ内のURLを選択すると。 |
| TARGET | | ターゲットズームビューアでは、ユーザーがズームターゲットを選択すると、画像の一部にズームされます。 |
| SEARCH | | eCatalog で、ユーザが単語検索を実行したとき。 |
| PLAY | **X**（ビデオ） | ビデオビューアで、「再生」を選択すると、ビデオの再生が開始されます。<br><br>**注意：** Adobe Analytics ハートビートベースのビデオレポートを使用している場合、Adobe Dynamic Media ClassicでAdobe Analyticsを設定するときに、このビューアイベントに変数をマッピングする必要はありません。 ビデオ ハートビートは、Adobe Dynamic Media Classic HTML5 ビデオおよびMixed Media ビューアで動作します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。 [Adobe Analytics ビデオレポートの有効化](enabling-analytics-video-reports.md)を参照してください。 |
| PAUSE | **X**（ビデオ） | ビデオビューアで、ユーザーが&#x200B;**[!UICONTROL 一時停止]**&#x200B;を選択してビデオをフリーズすると、ビデオがフリーズされます。<br><br>**注：** Adobe Analytics ハートビートベースのビデオレポートを使用している場合、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、このビューアイベントに変数をマッピングする必要はありません。 ビデオ ハートビートは、Adobe Dynamic Media Classic HTML5 ビデオおよびMixed Media ビューアで動作します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。 [Adobe Analytics ビデオレポートの有効化](enabling-analytics-video-reports.md)を参照してください。 |
| STOP | **X**（ビデオ） | ビデオビューアで、ユーザーが&#x200B;**[!UICONTROL 停止]**&#x200B;を選択してビデオの再生を停止すると、ビデオの再生が停止します。<br><br>**注意：** Adobe Analytics ハートビートベースのビデオレポートを使用している場合、Adobe Dynamic Media ClassicでAdobe Analyticsを設定する際に、このビューアイベントに変数をマッピングする必要はありません。 ビデオ ハートビートは、Adobe Dynamic Media Classic HTML5 ビデオおよびMixed Media ビューアで動作します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。 [Adobe Analytics ビデオレポートの有効化](enabling-analytics-video-reports.md)を参照してください。 |
| MILESTONE | **X**（ビデオ） | ビデオビューアでは、ユーザーがビデオの0、25、50、75、または100%を視聴すると、マイルストーンイベントが生成されます。<br><br>**注意：** Adobe Analytics ハートビートベースのビデオレポートを使用している場合は、Adobe Dynamic Media ClassicでAdobe Analyticsを設定するときに、このビューアイベントに変数をマッピングする必要はありません。 ビデオ ハートビートは、Adobe Dynamic Media Classic HTML5 ビデオおよびMixed Media ビューアで動作します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。 [Adobe Analytics ビデオレポートの有効化](enabling-analytics-video-reports.md)を参照してください。 |
| SWATCH | **X**（フライアウト、ズーム） | このビューアーイベントは、Adobe Dynamic Media ClassicのPAGE ビューアーイベントにマッピングされます。 |
| ZOOM | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。 |
| PAN | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。 |
| SPIN | **X**（スピンセット） | Adobe Analytics では追跡されません。 |

### Adobe Dynamic Media Classic変数 {#scene-variables}

Adobe Analytics Configuration画面の各ビューアーイベントについて、Adobe Analytics変数と&#x200B;*Adobe Dynamic Media Classic変数*&#x200B;を選択します。 Adobe Dynamic Media Classic変数は、レポート用に取得できるデータを表します。 例えば、`searchTerm`変数には、eCatalog検索で使用されるキーワードが一覧表示されます。

次の表に、Adobe Dynamic Media Classicの変数を示します。

| Adobe Dynamic Media Classic変数 | 説明 |
| --- | --- |
| asset | Adobe Dynamic Media Classic アセット IDまたはビデオパスファイル。 |
| viewerId | 各種ビューアタイプに割り当てられている任意の番号。 |
| pageLabel | eCatalog でビューアが表示するページ。 |
| label | ラベル値（文字列）。 |
| frame | 画像セットで参照されるページまたはページ。 |
| rollover_keyRaw | HREF値全体ではなく、処理済みの部分も含まれます。 |
| rollover_keyProc | 画像マップ内で参照されているアイテムの ID（Href イベントと Item イベントについて有効）。 |
| searchTerm | eCatalog 検索で使用される語句。 |
| timeStamp | ビデオビューアで選択した再生、停止、一時停止。 |
| progress | Milestone イベントの完了率。 |
| targetId | ID値（数値）。 |

## ビューアイベントのアクティブ化、編集、削除 {#activating-editing-and-deleting-viewer-events}

Adobe Analytics 設定画面で、ビューアイベントをアクティブ化、編集および削除できます。

* **アクティブ化**：選択したビューアイベントをアクティブ化するには、**[!UICONTROL アクティブ化]**&#x200B;を選択するか、**[!UICONTROL 無効にする]**&#x200B;を選択します。

* **編集**: ビューアーイベントを選択し、**[!UICONTROL 表示/編集]**&#x200B;変数グレーのボタンを選択します。 Adobe Dynamic Media Classic変数とAdobe Analytics変数のドロップダウンリストで、それぞれのリストから異なる変数を選択します。 詳しくは、[Adobe Dynamic Media Classic ビューアのイベントおよび変数へのAdobe Analytics変数の割り当て](#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables)を参照してください。

* **削除**：ビューアーイベントを選択し、**[!UICONTROL 表示/編集]**&#x200B;変数グレーのボタンを選択します。 **[!UICONTROL 削除]**&#x200B;を選択します。
