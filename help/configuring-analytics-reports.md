---
title: Adobe Analytics レポートの設定
seo-title: Adobe Analytics レポートの設定
description: 'null'
seo-description: Adobe Analyticsレポートの設定方法を説明します。
uuid: bf210f68-dcb0-4e86-be04-0a8b2117ef2a
contentOwner: 管理者
content-type: 参照
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: f4c8c2b3-cc95-416f-9a5d-da81c231dfc2
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Adobe Analytics レポートの設定{#configuring-adobe-analytics-reports}

Adobe Analytics で Adobe Analytics レポートに含める情報を指定するには、Adobe Analytics 設定画面に移動します。レポートを設定した後、この画面には、情報を必要とする各ビューアイベントに対して、対応するAdobe Analytics変数とDynamic Media Classic変数が表示されます。 これらのビューアイベント、Adobe Analytics変数、ダイナミックメディアクラシック変数の組み合わせによって、レポートされる情報が決まります。

ビューアイベントを変数と関連付ける機能のほか、Adobe Analytics 設定画面にはビューアイベントをアクティブ化、編集および削除するためのツールがあります。

>[!NOTE]
>
>Adobe Analytics で Adobe Analytics レポート設定を変更するときは常に、Adobe Scene7 Publishing System から再度 Adobe Analytics にログオンし、Adobe Analytics 設定を再保存してから再公開するようにしてください。

詳しくは、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

詳しくは、[設定情報の公開](publishing-analytics-configuration-information.md#publishing_adobe_analytics_configuration_information)を参照してください。

## Dynamic Media Classicビューアイベントと変数へのAdobe Analytics変数の割り当て {#assigning-adobe-analytics-variables-to-scene-viewer-events-and-variables}

Adobe Analytics設定画面を使用して、ビューアイベントをAdobe Analytics変数およびDynamic Media Classic変数に関連付けます。 各ビューアイベントに対して、1つのAdobe Analytics変数と1つのDynamic Media Classic変数を選択します。 Adobe Analytics 設定画面を開く方法については、[Adobe Analytics へのログイン](log-analytics.md#log_in_to_adobe_analytics)を参照してください。

**Adobe Analytics変数をダイナミックMedia Classicビューアのイベントと変数に割り当てるには**

1. After you log in to Adobe Analytics from within Dynamic Media Classic and select a report suite, on the Adobe Analytics Configuration page, in the far right column of the table, activate a viewer event by clicking **Enable**.
1. 「変数」列で、目的のビューアイベントの矢印ボタンをクリックして、変数ペア選択機能を表示します。

   詳しくは、[ビューアイベント](configuring-analytics-reports.md#viewer_events)を参照してください。

1. Dynamic Media Classic変数を追加します。

   ダイナミック [メディアクラシック変数を参照してくださ](configuring-analytics-reports.md#scene7_variables)い。

1. Adobe Analytics 変数を追加します。
1. （オプション）別の変数ペアを追加するには、「**追加**」をクリックします。
1. 「**保存**」をクリックします。

   「保存」をクリックすると、ビューアイベント、そのAdobe Analytics変数およびDynamic Media Classic変数がAdobe Analytics設定画面に表示されます。

1. 右下隅の「**閉じる**」をクリックします。
1. **公開**／**公開を送信**&#x200B;をクリックし、画像サービング公開を実行します。

   ビューアに含まれる情報をDynamic Media Classicサーバーで使用できるようにするには、公開が必要です。

### ビューアイベント {#viewer-events}

ビューアイベントは、ユーザがダイナミックメディアクラシックビューアで実行するアクションを表します。 ユーザーが特定のアクション（サムネールのクリック、ビデオの開始または停止など）を開始すると、ビューアは Web ページに対して、イベントとそのイベントに関連付けられたデータを「ブロードキャスト」します。

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
| PLAY | **X**（ビデオ） | ビデオビューアで、ユーザが再生ボタンをクリックしてビデオの再生を開始したとき。<br><br>**** 注意：Adobe Analyticsハートビートベースのビデオレポートを使用している場合は、Dynamic Media ClassicでAdobe Analyticsを設定する際に、変数をこのビューアイベントにマップする必要はありません。 ビデオハートビートは、標準搭載のダイナミックメディアクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| PAUSE | **X**（ビデオ） | ビデオビューアで、ユーザが一時停止ボタンをクリックしてビデオを一時停止したとき。<br><br>**** 注意：Adobe Analyticsハートビートベースのビデオレポートを使用している場合は、Dynamic Media ClassicでAdobe Analyticsを設定する際に、変数をこのビューアイベントにマップする必要はありません。 ビデオハートビートは、標準搭載のダイナミックメディアクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| STOP | **X**（ビデオ） | ビデオビューアで、ユーザーが停止ボタンをクリックしてビデオの再生を停止したとき。<br><br>**** 注意：Adobe Analyticsハートビートベースのビデオレポートを使用している場合は、Dynamic Media ClassicでAdobe Analyticsを設定する際に、変数をこのビューアイベントにマップする必要はありません。 ビデオハートビートは、標準搭載のダイナミックメディアクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| MILESTONE | **X**  (ビデオ) | ビデオビューアでは、ユーザーがビデオを 0、25、50、75 または 100 パーセント見ると Milestone イベントが生成されます。<br><br>**** 注意：Adobe Analyticsハートビートベースのビデオレポートを使用している場合は、Dynamic Media ClassicでAdobe Analyticsを設定する際に、変数をこのビューアイベントにマップする必要はありません。 ビデオハートビートは、標準搭載のダイナミックメディアクラシックHTML5ビデオビューアおよびMixedMediaビューアと連携します。 ビデオプレーヤーは Adobe Analytics ビデオレポート内で表示される追跡データを生成します。See [Enabling Adobe Analytics Video Reports](enabling-analytics-video-reports.md). |
| SWATCH | X（フライアウト、ズーム） | このビューアイベントは Scene7 Publishing System の PAGE ビューアイベントにマッピングされます。 |
| ZOOM | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。<br> |
| PAN | **X**（eCatalog、スピンセット、ズーム） | Adobe Analytics では追跡されません。<br> |
| SPIN | **X**（スピンセット） | Adobe Analytics では追跡されません。<br> |


### Dynamic Media Classic変数 {#scene-variables}

For each viewer event on Adobe Analytics Configuration screen, choose a Adobe Analytics variable and a *Dynamic Media Classic variable*. ダイナミックメディアクラシック変数は、レポートで取得できるデータを表します。 例えば、`searchTerm` 変数は eCatalog 検索に使用されるキーワードを表示します。

次の表に、ダイナミックメディアクラシック変数を示します。

| Dynamic Media Classic変数 | 説明 |
|--- |:--- |
| asset | Scene7 Publishing System アセット ID またはビデオパスファイル。 |
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

* **アクティブ化**「有効 **[!UICONTROL 化]** 」をクリックして、選択し **[!UICONTROL たビューアイベン]** トをアクティブ化または非アクティブ化します。

* **編集ビュ**&#x200B;ーアイベントを選択し、「変数を表 **[!UICONTROL 示/編集]** 」グレーボタンをクリックします。 「ダイナミックメディアクラシック変数」と「Adobe Analytics変数」ドロップダウンリストで、それぞれのリストから別の変数を選択します。 詳しくは、ダイナミックMedia Classicビューアイベントと変数へのAdobe Analytics変数の割り当てを参照してください。

* **ビューア**&#x200B;イベントの削除を参照し、「変数を表示/ **[!UICONTROL 編集]** 」グレーボタンをクリックします。 Click **[!UICONTROL Delete]**.
