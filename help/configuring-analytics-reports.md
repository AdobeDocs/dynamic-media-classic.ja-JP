---
title: Adobe Analytics レポートの設定
description: Adobe Analyticsレポートの設定方法を説明します。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Mediaクラシック
role: Data Engineer,Administrator,Business Practitioner
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
translation-type: tm+mt
source-git-commit: 98463dbc24e141547d01bd3f71b1b9fe3a692c14
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 46%

---

# Adobe Analytics レポートの設定{#configuring-adobe-analytics-reports}

Adobe Analytics で Adobe Analytics レポートに含める情報を指定するには、Adobe Analytics 設定画面に移動します。レポートを設定した後、この画面リストは、情報を取得する各ビューアイベントに対して、対応するAdobe Analytics変数とDynamic Mediaクラシック変数を設定します。 これらのビューアイベント、Adobe Analytics変数、Dynamic Mediaクラシック変数の組み合わせによって、レポートされる情報が決まります。

ビューアイベントを変数に関連付ける他に、Adobe Analytics設定画面には、ビューアイベントのアクティブ化、編集および削除を行うためのオファーツールがあります。

>[!NOTE]
>
>Adobe AnalyticsでAdobe Analyticsレポートの設定を変更する場合は、必ずAdobeDynamic MediaクラシックからAdobe Analyticsに再度ログオンし、Adobe Analyticsの設定を再度保存してから再公開してください。

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

詳しくは、[設定情報の公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

## Dynamic Mediaクラシックビューアのイベントと変数へのAdobe Analytics変数の割り当て{#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

ビューアイベントをAdobe Analytics変数およびDynamic Mediaクラシック変数に関連付けるには、Adobe Analytics設定画面を使用します。 各ビューアイベントに対して、1つのAdobe Analytics変数と1つのDynamic Mediaクラシック変数を選択します。 Adobe Analytics 設定画面を開く方法については、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

**Adobe Analytics変数をDynamic Mediaクラシックビューアのイベントと変数に割り当てるには**

1. Dynamic MediaクラシックからAdobe Analyticsにログインし、レポートスイートを選択した後、Adobe Analytics設定ページの右側の表の列で、「**[!UICONTROL 有効にする]**」をクリックしてビューアイベントをアクティブ化します。
1. 「変数」列で、目的のビューアイベントの矢印ボタンをクリックして、変数ペア選択機能を表示します。

   詳しくは、[ビューアイベント](configuring-analytics-reports.md#viewer_events)を参照してください。

1. 追加Dynamic Mediaクラシック変数。

   [Dynamic Mediaクラシック変数](configuring-analytics-reports.md#scene7_variables)を参照してください。

1. Adobe Analytics 変数を追加します。
1. （オプション）別の変数ペアを追加するには、「**追加**」をクリックします。
1. 「**保存**」をクリックします。

   「保存」をクリックすると、ビューアイベント、そのAdobe Analytics変数およびDynamic Mediaクラシック変数がAdobe Analytics設定画面に表示されます。

1. 右下隅の「**閉じる**」をクリックします。
1. **公開**／**公開を送信**&#x200B;をクリックし、画像サービング公開を実行します。

   ビューアに含まれる情報をDynamic Mediaクラシックサーバで使用できるようにするには、公開が必要です。

### ビューアイベント {#viewer-events}

ビューアのイベントは、Dynamic Mediaクラシックビューアでユーザが実行するアクションを記述します。 ユーザーが特定の操作（サムネールのクリック、ビデオの開始または停止など）を開始すると、ビューアはWebページに対して、そのイベントに関連付けられたデータと共にイベントを「ブロードキャスト」します。

次の表に、Adobe Analytics 設定画面に追加できるビューアイベントを示します。

| ビューアイベント | HTML5 ビューアプラットフォームのサポートとビューア | 説明 |
|--- |--- |--- |
| LOAD | **X**（eCatalog、フライアウト、スピンセット、ビデオ、ズーム） | ユーザがビューアを起動したとき。 |
| PAGE | **X**（eCatalog） | eCatalog でユーザーがページをめくったとき。ターゲットズームビューアでユーザーが別のターゲットまたはカラースウォッチをクリックしたとき。 |
| SWAP | **X**（eCatalog、フライアウト、スピンセット、ビデオ、ズーム） | ユーザが別のサムネールをクリックして、別の画像を表示したとき。 |
| ITEM | **X**（eCatalog） | ロールオーバーが定義されている画像マップをサポートするビューアで、ユーザがポインタを画像マップに合わせ、ロールオーバーテキストを読むとき。 |
| HREF | **X**（eCatalog） | 画像マップをサポートするビューアで、ユーザが画像マップ内の URL をクリックしたとき。 |
| TARGET |  | ターゲットズームビューアで、ユーザがズームターゲットをクリックして画像の一部をズームしたとき。 |
| SEARCH |  | eCatalog で、ユーザが単語検索を実行したとき。 |
| PLAY | **X**（ビデオ） | ビデオビューアで、ユーザが再生ボタンをクリックしてビデオの再生を開始したとき。<br><br>**注意：Adobe Analyticsハートビートベースのビデオレポートを使用し** ている場合、Dynamic MediaクラシックでAdobe Analyticsを設定する際に、このビューアイベントに変数をマップする必要はありません。ビデオハートビートは、標準搭載のDynamic MediaクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。「[Adobe Analyticsビデオレポートの有効化](enabling-analytics-video-reports.md)」を参照してください。 |
| PAUSE | **X**（ビデオ） | ビデオビューアで、ユーザが一時停止ボタンをクリックしてビデオを一時停止したとき。<br><br>**注意：Adobe Analyticsハートビートベースのビデオレポートを使用し** ている場合、Dynamic MediaクラシックでAdobe Analyticsを設定する際に、このビューアイベントに変数をマップする必要はありません。ビデオハートビートは、標準搭載のDynamic MediaクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。「[Adobe Analyticsビデオレポートの有効化](enabling-analytics-video-reports.md)」を参照してください。 |
| STOP | **X**（ビデオ） | ビデオビューアで、ユーザーが停止ボタンをクリックしてビデオの再生を停止したとき。<br><br>**注意：Adobe Analyticsハートビートベースのビデオレポートを使用し** ている場合、Dynamic MediaクラシックでAdobe Analyticsを設定する際に、このビューアイベントに変数をマップする必要はありません。ビデオハートビートは、標準搭載のDynamic MediaクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。「[Adobe Analyticsビデオレポートの有効化](enabling-analytics-video-reports.md)」を参照してください。 |
| MILESTONE | **X**  (ビデオ) | ビデオビューアでは、ユーザーがビデオを 0、25、50、75 または 100 パーセント見ると Milestone イベントが生成されます。<br><br>**注意：Adobe Analyticsハートビートベースのビデオレポートを使用し** ている場合、Dynamic MediaクラシックでAdobe Analyticsを設定する際に、このビューアイベントに変数をマップする必要はありません。ビデオハートビートは、標準搭載のDynamic MediaクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。「[Adobe Analyticsビデオレポートの有効化](enabling-analytics-video-reports.md)」を参照してください。 |
| SWATCH | X（フライアウト、ズーム） | このビューアイベントは、Dynamic MediaクラシックのPAGE Viewerイベントにマップされます。 |
| ZOOM | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。<br> |
| PAN | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。<br> |
| SPIN | **X**（スピンセット） | Adobe Analytics では追跡されません。<br> |


### Dynamic Mediaクラシック変数{#scene-variables}

Adobe Analytics設定画面のビューアイベントごとに、Adobe Analytics変数と&#x200B;*Dynamic Mediaクラシック変数*&#x200B;を選択します。 Dynamic Mediaクラシック変数は、レポートで取得できるデータを表します。 例えば、`searchTerm` 変数は eCatalog 検索に使用されるキーワードを表示します。

次の表に、Dynamic Mediaクラシック変数を示します。

| Dynamic Mediaクラシック変数 | 説明 |
|--- |:--- |
| asset | Dynamic MediaクラシックアセットIDまたはビデオパスファイル |
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

## ビューアイベントのアクティブ化、編集、削除  {#activating-editing-and-deleting-viewer-events}

Adobe Analytics 設定画面で、ビューアイベントをアクティブ化、編集および削除できます。

* **ActivatingClick**
Enableをクリックして、選択したビューアイベントをアクティブ化または ****  **** 無効化します。

* ****
編集ビューアのイベントを選択し、 **[!UICONTROL 表示/]** 変数を編集グレーボタンをクリックします。「Dynamic Mediaクラシック変数」と「Adobe Analytics変数」のドロップダウンリストで、それぞれのリストから別の変数を選択します。 詳しくは、「Dynamic Mediaクラシックビューアイベントと変数へのAdobe Analytics変数の割り当て」を参照してください。

* ****
削除ビューアのイベントを選択し、 **[!UICONTROL 表示/]** 変数を編集グレーボタンをクリックします。**[!UICONTROL 「削除」]**&#x200B;をクリックします。
