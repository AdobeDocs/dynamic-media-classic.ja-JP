---
title: Adobe Analytics レポートの設定
description: Adobe Analyticsレポートの設定方法を説明します。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: d9fda3b8-7da8-4a30-a5f8-9bb34ec1b43d
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 46%

---

# Adobe Analytics レポートの設定{#configuring-adobe-analytics-reports}

Adobe Analytics で Adobe Analytics レポートに含める情報を指定するには、Adobe Analytics 設定画面に移動します。レポートを設定すると、この画面には、情報が必要な各ビューアイベントに対して、対応するAdobe Analytics変数とDynamic Media Classic変数が表示されます。 これらのビューアイベント、Adobe Analytics変数、Dynamic Media Classic変数の組み合わせによって、レポートされる情報が決まります。

Adobe Analytics設定画面には、ビューアイベントを変数に関連付ける以外に、ビューアイベントをアクティブ化、編集および削除するためのツールが用意されています。

>[!NOTE]
>
>Adobe Analytics内でAdobe Analyticsレポート設定を変更する場合は、必ずAdobeDynamic Media ClassicからAdobe Analyticsに再度ログオンし、Adobe Analytics設定を再保存してから、再公開してください。

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

詳しくは、[設定情報の公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

## Dynamic Media Classicビューアイベントと変数へのAdobe Analytics変数の割り当て {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Adobe Analytics設定画面を使用して、Adobe Analytics変数とDynamic Media Classic変数にビューアイベントを関連付けます。 ビューアイベントごとに、1つのAdobe Analytics変数と1つのDynamic Media Classic変数を選択します。 Adobe Analytics 設定画面を開く方法については、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

**Adobe Analytics変数をDynamic Media Classicビューアのイベントと変数に割り当てるには**

1. Dynamic Media Classic内からAdobe Analyticsにログインしてレポートスイートを選択した後、Adobe Analyticsの設定ページの右側の表の列で、「**[!UICONTROL 有効]**」をクリックしてビューアイベントをアクティブにします。
1. 「変数」列で、目的のビューアイベントの矢印ボタンをクリックして、変数ペア選択機能を表示します。

   詳しくは、[ビューアイベント](configuring-analytics-reports.md#viewer_events)を参照してください。

1. Dynamic Media Classic変数を追加します。

   [Dynamic Media Classic変数](configuring-analytics-reports.md#scene7_variables)を参照してください。

1. Adobe Analytics 変数を追加します。
1. （オプション）別の変数ペアを追加するには、「**追加**」をクリックします。
1. 「**保存**」をクリックします。

   「保存」をクリックすると、ビューアイベント、そのAdobe Analytics変数およびDynamic Media Classic変数がAdobe Analytics設定画面に表示されます。

1. 右下隅の「**閉じる**」をクリックします。
1. **公開**／**公開を送信**&#x200B;をクリックし、画像サービング公開を実行します。

   ビューアに含まれる情報をDynamic Media Classicサーバーで利用するには、公開が必要です。

### ビューアイベント {#viewer-events}

ビューアイベントは、Dynamic Media Classicビューアでユーザーが実行するアクションを記述します。 ユーザーがサムネールのクリックやビデオの開始または停止など、特定のアクションを開始すると、ビューアはイベントをWebページに「ブロードキャスト」し、そのイベントに関連付けられたデータもブロードキャストします。

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
| PLAY | **X**（ビデオ） | ビデオビューアで、ユーザが再生ボタンをクリックしてビデオの再生を開始したとき。<br><br>**注意：** Adobe Analyticsハートビートベースのビデオレポートを使用している場合、Dynamic Media ClassicでAdobe Analyticsを設定する際に、このビューアイベントに変数をマッピングする必要はありません。ビデオハートビートは、標準搭載のDynamic Media Classic HTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。[Adobe Analyticsビデオレポートの有効化](enabling-analytics-video-reports.md)を参照してください。 |
| PAUSE | **X**（ビデオ） | ビデオビューアで、ユーザが一時停止ボタンをクリックしてビデオを一時停止したとき。<br><br>**注意：** Adobe Analyticsハートビートベースのビデオレポートを使用している場合、Dynamic Media ClassicでAdobe Analyticsを設定する際に、このビューアイベントに変数をマッピングする必要はありません。ビデオハートビートは、標準搭載のDynamic Media Classic HTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。[Adobe Analyticsビデオレポートの有効化](enabling-analytics-video-reports.md)を参照してください。 |
| STOP | **X**（ビデオ） | ビデオビューアで、ユーザーが停止ボタンをクリックしてビデオの再生を停止したとき。<br><br>**注意：** Adobe Analyticsハートビートベースのビデオレポートを使用している場合、Dynamic Media ClassicでAdobe Analyticsを設定する際に、このビューアイベントに変数をマッピングする必要はありません。ビデオハートビートは、標準搭載のDynamic Media Classic HTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。[Adobe Analyticsビデオレポートの有効化](enabling-analytics-video-reports.md)を参照してください。 |
| MILESTONE | **X**  (ビデオ) | ビデオビューアでは、ユーザーがビデオを 0、25、50、75 または 100 パーセント見ると Milestone イベントが生成されます。<br><br>**注意：** Adobe Analyticsハートビートベースのビデオレポートを使用している場合、Dynamic Media ClassicでAdobe Analyticsを設定する際に、このビューアイベントに変数をマッピングする必要はありません。ビデオハートビートは、標準搭載のDynamic Media Classic HTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。[Adobe Analyticsビデオレポートの有効化](enabling-analytics-video-reports.md)を参照してください。 |
| SWATCH | X（フライアウト、ズーム） | このビューアイベントは、Dynamic Media ClassicのPAGEビューアイベントにマッピングされます。 |
| ZOOM | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。<br> |
| PAN | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。<br> |
| SPIN | **X**（スピンセット） | Adobe Analytics では追跡されません。<br> |


### Dynamic Media Classic変数 {#scene-variables}

Adobe Analytics設定画面の各ビューアイベントに対して、Adobe Analytics変数と&#x200B;*Dynamic Media Classic変数*&#x200B;を選択します。 Dynamic Media Classic変数は、レポートに対して取得できるデータを表します。 例えば、`searchTerm` 変数は eCatalog 検索に使用されるキーワードを表示します。

次の表に、Dynamic Media Classic変数を示します。

| Dynamic Media Classic変数 | 説明 |
|--- |:--- |
| asset | Dynamic Media ClassicアセットIDまたはビデオパスファイル。 |
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

* ****
ActivatingClick選択したビ **** ューアイベントをアクティベ **** ートまたは無効にするには、「Enable」をクリックします。

* ****
編集ビューアイベントを選択し、「表 **[!UICONTROL 示/変数を編]** 集」グレーボタンをクリックします。「 Dynamic Mediaクラシック変数」と「 Adobe Analytics変数」ドロップダウンリストで、それぞれのリストから異なる変数を選択します。 詳しくは、 Dynamic Media Classicビューアイベントと変数へのAdobe Analytics変数の割り当てを参照してください。

* ****
削除ビューアイベントを選択し、「表 **[!UICONTROL 示/変数を編]** 集」グレーボタンをクリックします。**[!UICONTROL 「削除」]**&#x200B;をクリックします。
