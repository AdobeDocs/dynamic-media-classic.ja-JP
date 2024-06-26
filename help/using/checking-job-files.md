---
title: ジョブ ファイルの確認
description: Adobe Dynamic Media Classicでジョブファイルを確認する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
topic: Administration, Content Management
level: Intermediate
source-git-commit: bb229047c0c9b3855453ea15dcd1f9754bc65cef
workflow-type: tm+mt
source-wordcount: '1622'
ht-degree: 23%

---

# ジョブ ファイルの確認{#checking-job-files}

Adobe Dynamic Media Classicへのファイルのアップロードや、Adobe Dynamic Media Classic サーバーに公開するファイルを監視するために、Adobe Dynamic Media Classicにはジョブページが用意されています。 ジョブページでジョブのレビュー、アップロード、公開を行ったり、ジョブのステータスを確認したり、このページからジョブの公開をキャンセルしたりできます。 また、アップロードおよび公開ジョブをスケジュールすることもできます。

アセットをアップロードすると、ジョブメニューの横に、ジョブが処理中であることを示す回転する模様のアイコンと、処理中のファイル数が表示されます。このアイコンを選択して、アクティブなジョブの詳細を表示することができます。

>[!NOTE]
>
>最近公開したジョブのリストは、最新のアクティビティページにも表示されます。を選択 **[!UICONTROL 最近]** をクリックします。

## ジョブページについて {#about-the-jobs-page}

を選択 **[!UICONTROL ジョブ]** グローバルナビゲーションバーので、ジョブ ページが開きます。 初期設定では、ジョブは新しい順に表示されます。

ジョブページの「ヒストリー」タブに、ジョブに関する次の情報が表示されます。

* **[!UICONTROL ジョブタイプ]**：ジョブタイプを示すアイコン。アップロードと公開は、最も一般的なジョブタイプです。

* **[!UICONTROL ジョブ名]**：ジョブの名前。 名前には、ユーザーが入力した名前の部分と日時が含まれます。

* **[!UICONTROL 開始日時]**：ジョブの開始時刻。

* **[!UICONTROL 合計]**：転送されたファイルの数。

* **[!UICONTROL 警告（警告）]**：ジョブ内の警告の数（ある場合）。 警告は、ジョブ全体が完了するのに影響を与えなかった問題を示します。これらの警告は、隠しファイルに関するものであるため、通常、無視することができます。例： `.DS_store` ファイル（Mac）と Thumbs.db ファイル（Windows®）には、画像ファイルをユーザーに表示する方法が記載されています。 ただし、これらのファイルに関する警告エントリは、Adobe Dynamic Media Classicでのこれらのファイルの使用方法に関係しないので、無視できます。 ジョブ名をダブルクリックして、警告に関する詳細情報を入手することができます。

* **[!UICONTROL E （エラー）]**：ジョブでエラーが発生した場合、その数がリストされます。 ジョブ名をダブルクリックして、エラーに関する詳細情報を入手することができます。

* **[!UICONTROL 期間]**：ジョブの完了に要した時間。

* **[!UICONTROL ステータス]**：ジョブのステータスを表示します。

* **[!UICONTROL 宛先]**：アップロードジョブの場合、宛先はファイルがアップロードされた会社名とフォルダーです。 このカテゴリは、公開用ジョブには適用されません。

* **[!UICONTROL 送信者]**：アセットをアップロードしたユーザーをリストします。

>[!NOTE]
>
>を選択して、進行中の公開およびアップロードのジョブをキャンセルできます **[!UICONTROL キャンセル]** ボタンがプログレスバーの隣に表示されます。

## ジョブページでのビューの変更 {#changing-views-on-the-jobs-page}

ジョブを並べ替えたり、ジョブページの「ヒストリー」タブの表示方法を変更するには、次の手順に従います。

* **[!UICONTROL 並べ替え]**：列名を選択して、特定の列でリストを並べ替えます。 列名の横にあるスイッチを選択して、降順または昇順で並べ替えることができます。

* **[!UICONTROL 日付範囲]**：を選択します **[!UICONTROL 日付範囲]** メニューを選択し、ジョブのリストを現在の日付、前週または前月に絞り込むオプションを選択します。 を選択 **[!UICONTROL カスタム日付範囲]**&#x200B;を入力してから、特定の日付範囲を入力します。

* **[!UICONTROL ジョブタイプ]**：を選択します **[!UICONTROL ジョブタイプ]** メニューと選択 **[!UICONTROL 公開]** または **[!UICONTROL Upload]** リストを絞り込んで、ジョブを公開したり、ジョブをアップロードしたりします。 を選択 **[!UICONTROL すべて]** 両方のタイプのジョブを表示する場合

* **[!UICONTROL 表示]**：に移動します **[!UICONTROL 表示]** > **[!UICONTROL マイ ジョブ]** または **[!UICONTROL 表示]** > **[!UICONTROL すべてのジョブ]** リストを、ユーザーが注文したジョブまたはユーザーが会社で注文したジョブに絞り込みます。

## ジョブの詳細レポートの表示、コピー、印刷 {#viewing-copying-or-printing-a-job-details-report}

「ジョブ」ページでレポートの名前をダブルクリックすると、「ジョブの詳細」ページが開きます。 このページには、ジョブ内のファイルに関する概要レポートが表示されます。を選択 **[!UICONTROL 詳細を表示]** これにより、エントリのAdobe Dynamic Media Classic ID、宛先パス、ステータス情報を確認できます。 Adobe Dynamic Media Classicで使用できないフォントを必要とするPDFまたは PostScript ファイルをアップロードした場合、レポートには不足しているフォントが一覧表示されます。

この情報は、クリップボードにコピーすることができます。

1. [ ジョブ ] ページでレポートの名前をダブルクリックします。
1. ジョブの詳細ページで、次の項目を選択します **[!UICONTROL 詳細を表示]** エントリに関する詳細なレポートを取得する
1. を選択 **[!UICONTROL クリップボードにコピー]**.

## 繰り返し発生するアップロードジョブと公開ジョブの処理 {#handling-recurring-upload-and-publish-jobs}

「アップロード」ページと「公開」ページで作成した繰り返しアップロードジョブと公開ジョブは、ジョブ ページの「スケジュール済み」タブに表示されます。 「スケジュール済み」タブで定期ジョブを編集または削除することができます。

グローバルナビゲーションバーのジョブ ボタンを選択し、ジョブ ページで **[!UICONTROL スケジュール済み]** タブを使用して、繰り返しジョブを編集および削除できます。

>[!NOTE]
>
>でジョブリストをフィルタリングできます。 **[!UICONTROL スケジュール済み]** tab キーを押すと「」が表示されます **[!UICONTROL ジョブタイプ]** および **[!UICONTROL 表示]** メニュー。 ジョブタイプを選択すると、リストを絞り込んで、特定の種類のジョブを公開できます。 を選択 **[!UICONTROL 表示]** 自分が作成したジョブや社内の全員が作成したジョブを表示するオプションがあります。

### 繰り返しジョブの編集、削除、一時停止、再開 {#editing-deleting-pausing-and-resuming-recurring-jobs}

ジョブ ページで繰り返しジョブを選択し、ジョブを編集または削除する場合は、次の手順に従います。

* **繰り返しジョブの編集**：を選択します **[!UICONTROL 編集]** ボタンをクリックし、[ スケジュールされたジョブの編集 ] ダイアログ ボックスにスケジュール情報を入力します。 選択した間隔でジョブを繰り返す場合は、 **[!UICONTROL リピート]** > **[!UICONTROL カスタム]**.

参照： [カスタムアップロードまたは公開ジョブの時間間隔の作成](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **繰り返しジョブの削除**：を選択します **[!UICONTROL 削除]** ボタン。

* **繰り返しジョブの一時停止（および再開）**:「アクティブ」列で、チェックボックスの選択を解除してジョブを一時停止します。チェックボックスを選択して、一時停止したジョブを再開します。

### カスタムアップロードまたは公開ジョブの時間間隔の作成 {#creating-a-custom-upload-or-publish-job-time-interval}

（FTP 経由で）アップロードまたは公開ジョブのカスタム時間間隔を作成するには、アップロードまたは公開ページで、に移動します。 **[!UICONTROL リピート]** > **[!UICONTROL カスタム]**. 次に、アップロードジョブまたはパブリッシュジョブを繰り返す間隔を説明する数値とワイルドカードをルールボックスに入力します。

「ルール」ボックスに指定するアップロードおよび公開のカスタム時間間隔の構文は、次のとおりです。

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

例： `0 15 10 * * ?` ジョブのスケジュールを毎日 10:15.00 に設定します。

次の表とリストに、「ルール」ボックスで時間間隔を指定する方法を示します。

この表に、時間単位、指定可能な値、およびサポートしているワイルドカードを示します。

| 時間単位 | 指定可能な値 | コメント | サポートされているワイルドカード |
|--- |--- |--- |--- |
| 秒 | 0 ～ 59 |  | `,: * /` |
| 分 | 0 ～ 59 |  | `,: * /` |
| 時間 | 0 ～ 23 | 24 時間表記を使用のこと. | `,: * /` |
| 日付 | 1 ～ 31 | 「日付」と「曜日」の両方に数値を指定することはできません。 これらのフィールドの 1 つが、 `?` ワイルドカード文字。 | `,: * / ? L C` |
| 月 | 1 ～ 12 または Jan、Feb、Mar、Apr、May、Jun、Jul、Aug、Sep、Oct、Nov、Dec | 値では大文字と小文字が区別されます。 | `,: * /` |
| 曜日 | Mon、Tue、Wed、Thu、Fri、Sat、Sun | 値では大文字と小文字が区別されます。 「日付」と「曜日」の両方に数値を指定することはできません。 これらのフィールドの 1 つが、 `?` ワイルドカード文字。 | `,: * / ? L C #` |
| 年（オプション） | 空白、または 1970 ～ 2099 |  | `,: * /` |


次の表に、「ルール」ボックスに指定可能なワイルドカード文字とその使用方法を示します。

| ワイルドカード文字 | 名前 | 意味 |
| --- | --- | --- |
| `*` | アスタリスク | すべての値（例：「every minute」）。 |
| `?` | 疑問符 | 特定の値なし（例：「指定された時間内の任意の分」）。 |
| `,` | カンマ | その他の値（例：「Monday and Wednesday」） |
| `-` | ハイフン | 値の範囲（例：「月曜日から金曜日」）。 |
| `/` | スラッシュ | 増分（例：「15 分ごと」）。 |
| `L` | 大文字の L | 最後の「曜日」または「曜日」（これらのフィールドでのみ使用可能）。 例えば、月が 1 月の場合、「日」フィールドの L 値により、ジョブが 1 月 31 日にスケジュールされます。 「曜日」フィールドには、この文字を単独で入力して、土曜日にジョブをスケジュールできます。 数字と共に使用できます（例： `6L`）を選択して、その月の最終金曜日を指定します。 指定しない `L` コンマまたはハイフンのワイルドカードを使用します。 |
| `#` | シャープ記号 | その月の「N 番目」の平日（「曜日」フィールドでのみ使用可能） 例： `6#3` 「曜日」フィールドには、月の第 3 金曜日を指定します。 この `6` 「金曜日」（週の 6 日目）とを示す `3` 月の 3 回目を示します。 |
| `C` | 大文字の C | 最初のカレンダー「曜日」または「曜日」（これらのフィールドでのみ使用できます）。 例えば、の値を指定します。 `1C` 「月の日」の場合、5 日目以降のカレンダーの最初の日がスケジュールされます。 「曜日」フィールドで、を指定します `1C` カレンダーの最初の日を日曜日またはそれ以降に設定します。 |

「ルール」ボックスの時間間隔の例を次に示します。

* `0 0 12 * * ?` ：毎日正午
* `0 15 10 ? * *` ：午前 10:15 （毎日）
* `0 0/5 14 * * ?`：毎日午後 2:00～2:55 の間、5 分間隔
* `0 0/5 14,18 * * ?` ：毎日 5 分ごと（午後 2:00～2:55 まで）、および 5 分ごと（毎日 6:00～6:55 まで）
* `0 10,44 14 ? 3` :3 月の毎週水曜日の午後 2 時 10 分および午後 2 時 44 分（水）
* `0 15 10 ? *` ：月 – 金の午前 10:15 （毎週平日）
* `0 15 10 20 * ?` ：毎月 20 日 10 時 15 分現在
* `0 15 10 L * ?` ：毎月最終日の午前 10 時 15 分
* `0 15 10 ? * 6L` ：毎月最終金曜日の午前 10 時 15 分
* `0 15 10 * * 6#3` ：毎月第 3 金曜日 10 時 15 分

## アップロードジョブまたは公開ジョブをトリガーとして使用 {#using-an-upload-or-publish-job-as-a-trigger}

FTP を介してアセットをアップロードする場合や公開ジョブを実行する場合は、アップロードの完了時に開始するように後続のジョブをスケジュールできます。 （他のジョブの開始がスケジュールされている場合、ここでスケジュールしたジョブはキューに入れられます）。 新しいジョブは、指定したアドレスに通知を送信し、その場所のコードをトリガーできるようにします。 この継続されるアップロードジョブの名前は、現在のアップロードジョブと同じ名前になりますが、先頭に _Pub が付きます。

あるアップロードジョブまたは公開ジョブを別のジョブとトリガーするには、次のオプションを選択します **[!UICONTROL 詳細]** （アップロードまたは公開ページ） 次に、「HTTP 通知」テキストフィールドに URL を入力します。
