---
title: ジョブファイルを確認
description: Adobe Dynamic Media Classicでジョブファイルを確認する方法を説明します。
uuid: 8241a894-3014-4a5c-96ef-71f3aaa3716a
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: d53ae5dd-8daf-4d87-b9a6-3039bad30538
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: b6b11e1c-5eda-4bdb-8ffb-ecd3678f2352
topic: Administration, Content Management
level: Intermediate
source-git-commit: a9bd472705bce32f63a5710c3266e51256d17a00
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 24%

---

# ジョブファイルを確認{#checking-job-files}

Adobe Dynamic Media Classicへのファイルアップロードと、Adobe Dynamic Media Classicサーバーに公開するファイルを監視するために、Adobe Dynamic Media Classicではジョブページを提供します。 ジョブページで、アップロードおよび公開ジョブを確認したり、ジョブのステータスを確認したり、ジョブの公開をキャンセルすることができます。また、アップロードおよび公開ジョブをスケジュールすることもできます。

アセットをアップロードすると、ジョブメニューの横に、ジョブが処理中であることを示す回転する模様のアイコンと、処理中のファイル数が表示されます。アイコンを選択して、アクティブなジョブの詳細を表示できます。

>[!NOTE]
>
>最近公開したジョブのリストは、最新のアクティビティページにも表示されます。選択 **[!UICONTROL 最近]** グローバルナビゲーションバーの

## ジョブページについて {#about-the-jobs-page}

選択 **[!UICONTROL ジョブ]** をクリックして、ジョブページを開きます。 初期設定では、ジョブは新しい順に表示されます。

ジョブページの「ヒストリー」タブに、ジョブに関する次の情報が表示されます。

* **[!UICONTROL ジョブタイプ]**  — ジョブの種類を示すアイコン。アップロードと公開が最も一般的なジョブの種類です。

* **[!UICONTROL ジョブ名]**  — ジョブの名前。 名前には、名前のユーザーが入力した部分と日時が含まれます。

* **[!UICONTROL 開始済み]**  — ジョブが開始されたとき。

* **[!UICONTROL 合計]**  — 転送されたファイルの数。

* **[!UICONTROL W（警告）]**  — ジョブ内の警告の数（存在する場合）。 警告は、ジョブ全体が完了するのに影響を与えなかった問題を示します。これらの警告は、隠しファイルに関するものであるため、通常、無視することができます。例： `.DS_store` ファイル (Mac) および Thumbs.db ファイル (Windows®) には、ユーザーに画像ファイルを表示する方法に関する情報が含まれています。 ただし、これらのファイルに関する警告エントリは、Adobe Dynamic Media Classicでの使用方法に関係しないので、無視できます。 ジョブ名をダブルクリックして、警告に関する詳細情報を入手することができます。

* **[!UICONTROL E（エラー）]**  — ジョブ内のエラー数をリストします（存在する場合）。 ジョブ名をダブルクリックして、エラーに関する詳細情報を入手することができます。

* **[!UICONTROL 期間]**  — ジョブの完了に要した時間。

* **[!UICONTROL ステータス]**  — ジョブのステータスを表示します。

* **[!UICONTROL 宛先]**  — アップロードジョブの場合、会社名、ファイルのアップロード先のフォルダー。 このカテゴリは、公開用のジョブには適用されません。

* **[!UICONTROL 送信者]**  — アセットをアップロードしたユーザーのリストが表示されます。

>[!NOTE]
>
>処理中の公開ジョブとアップロードジョブをキャンセルするには、 **[!UICONTROL キャンセル]** ボタンをクリックします。

## ジョブページのビューを変更します {#changing-views-on-the-jobs-page}

ジョブを並べ替えたり、ジョブページの「ヒストリー」タブの表示方法を変更するには、次の手順に従います。

* **[!UICONTROL 並べ替え]**  — 特定の列でリストを並べ替える列名を選択します。 列名の横にあるスイッチを選択して、降順または昇順で並べ替えることができます。

* **[!UICONTROL 日付範囲]**  — を選択します。 **[!UICONTROL 日付範囲]** メニューを開き、ジョブのリストを現在の日付、前の週または前の月に絞り込むオプションを選択します。 選択 **[!UICONTROL カスタム日付範囲]**&#x200B;をクリックし、特定の日付範囲を入力します。

* **[!UICONTROL ジョブタイプ]**  — を選択します。 **[!UICONTROL ジョブタイプ]** メニューと選択 **[!UICONTROL 公開]** または **[!UICONTROL アップロード]** を使用して、公開ジョブまたはアップロードジョブのリストを絞り込みます。 選択 **[!UICONTROL すべて]** をクリックして、両方のタイプのジョブを表示します。

* **[!UICONTROL 表示]**  — に移動します。 **[!UICONTROL 表示]** > **[!UICONTROL マイジョブ]** または **[!UICONTROL 表示]** > **[!UICONTROL すべてのジョブ]** を使用して、注文したジョブまたは社内の担当者が注文したジョブにリストを絞り込むことができます。

## ジョブの詳細レポートの表示、コピー、印刷 {#viewing-copying-or-printing-a-job-details-report}

ジョブページでレポートの名前をダブルクリックして、ジョブの詳細ページを開きます。 このページには、ジョブ内のファイルに関する概要レポートが表示されます。選択 **[!UICONTROL 詳細を表示]** そのため、エントリのAdobe Dynamic Media Classic ID、宛先パス、ステータス情報を確認できます。 Adobe Dynamic Media Classicで使用できないPDFを必要とするフォントまたは PostScript ファイルをアップロードした場合、レポートには見つからないフォントが表示されます。

この情報は、クリップボードにコピーすることができます。

1. ジョブページでレポートの名前をダブルクリックします。
1. ジョブの詳細ページで、「 」を選択します。 **[!UICONTROL 詳細を表示]** エントリに関する詳細なレポートを取得します。
1. 選択 **[!UICONTROL クリップボードにコピー]**.

## 繰り返し発生するアップロードジョブと公開ジョブの処理 {#handling-recurring-upload-and-publish-jobs}

アップロードページと公開ページで作成した定期的なアップロードジョブと公開ジョブは、ジョブページの「スケジュール済み」タブに表示されます。 「スケジュール済み」タブで定期ジョブを編集または削除することができます。

グローバルナビゲーションバーで「ジョブ」ボタンを選択し、ジョブページで、 **[!UICONTROL Scheduled]** 」タブを使用して、定期ジョブを編集および削除できます。

>[!NOTE]
>
>ジョブリストは、 **[!UICONTROL Scheduled]** タブに **[!UICONTROL ジョブタイプ]** および **[!UICONTROL 表示]** メニュー。 特定の種類の公開ジョブにリストを絞り込むためのジョブタイプを選択します。 を選択します。 **[!UICONTROL 表示]** 」オプションを使用します。

### 定期ジョブの編集、削除、一時停止、再開 {#editing-deleting-pausing-and-resuming-recurring-jobs}

ジョブページで定期ジョブを選択し、編集または削除する場合は次の手順に従います。

* **繰り返しジョブの編集**  — を選択します。 **[!UICONTROL 編集]** ボタンをクリックして、スケジュール済みジョブを編集ダイアログボックスにスケジュール情報を入力します。 任意の間隔でジョブを繰り返し実行する場合は、次に移動します。 **[!UICONTROL 繰り返し]** > **[!UICONTROL カスタム]**.

詳しくは、 [カスタムのアップロードまたは公開ジョブの時間間隔の作成](checking-job-files.md#creating_a_custom_upload_or_publish_job_time_interval).

* **繰り返しジョブの削除**  — を選択します。 **[!UICONTROL 削除]** 」ボタンをクリックします。

* **繰り返しジョブの一時停止（および再開）** - 「アクティブ」列で、チェックボックスの選択を解除してジョブを一時停止します。一時停止したジョブを再開するには、チェックボックスを選択します。

### カスタムのアップロードまたは公開ジョブの時間間隔の作成 {#creating-a-custom-upload-or-publish-job-time-interval}

アップロード（FTP 経由）または公開ジョブのカスタム時間間隔を作成するには、アップロードページまたは公開ページで、に移動します。 **[!UICONTROL 繰り返し]** > **[!UICONTROL カスタム]**. 次に、アップロードジョブまたは公開ジョブが繰り返される時間間隔を記述する「ルール」ボックスに数字やワイルドカードを入力します。

「ルール」ボックスに指定するアップロードおよび公開のカスタム時間間隔の構文は、次のとおりです。

`[seconds]` `[minutes]` `[hour of day]` `[day of month]` `[month]` `[day of week]`

例： `0 15 10 * * ?` は、ジョブを毎日 10:15.00 にスケジュールします。

次の表とリストに、「ルール」ボックスで時間間隔を指定する方法を示します。

この表に、時間単位、指定可能な値、およびサポートしているワイルドカードを示します。

| 時間単位 | 指定可能な値 | コメント | サポートされているワイルドカード |
|--- |--- |--- |--- |
| 秒 | 0 ～ 59 |  | `, - * /` |
| 分 | 0 ～ 59 |  | `, - * /` |
| 時間 | 0 ～ 23 | 24 時間表記を使用のこと. | `, - * /` |
| 日付 | 1 ～ 31 | 「曜日」と「曜日」の両方に数値を指定することはできません。 これらのフィールドの 1 つで、 `?` ワイルドカード文字。 | `, - * / ? L C` |
| 月 | 1 ～ 12 または Jan、Feb、Mar、Apr、May、Jun、Jul、Aug、Sep、Oct、Nov、Dec | 値では大文字と小文字が区別されます。 | `, - * /` |
| 曜日 | Mon、Tue、Wed、Thu、Fri、Sat、Sun | 値では大文字と小文字が区別されます。 「曜日」と「曜日」の両方に数値を指定することはできません。 これらのフィールドの 1 つで、 `?` ワイルドカード文字。 | `, - * / ? L C #` |
| 年（オプション） | 空白、または 1970 ～ 2099 |  | `, - * /` |


次の表に、「ルール」ボックスに指定可能なワイルドカード文字とその使用方法を示します。

| ワイルドカード文字 | 名前 | 意味 |
| --- | --- | --- |
| `*` | アスタリスク | すべての値（例：「毎分」）。 |
| `?` | 疑問符 | 特定の値はありません（例：「指定された時間内の任意の分」）。 |
| `,` | カンマ | その他の値（例：「月曜日と水曜日」）。 |
| `-` | ハイフン | 値の範囲（例：月～金）。 |
| `/` | スラッシュ | 増分（例：「15 分ごと」）。 |
| `L` | 大文字の L | 過去の「日」または「曜日」（これらのフィールドでのみ使用可能）。 例えば、月が 1 月の場合、「日」フィールドに L 値を指定すると、1 月 31 日のジョブのスケジュールが設定されます。 「曜日」フィールドには、この文字だけを入力して、土曜日にジョブをスケジュールできます。 数値と共に使用できます ( 例： `6L`) をクリックして、今月の最後の金曜日を指定します。 指定しない `L` にワイルドカード（コンマまたはハイフン）を使用します。 |
| `#` | シャープ記号 | 月の「N」曜日（「曜日」フィールドのみ使用可能）。 例： `6#3` 「曜日」フィールドに、月の第 3 金曜日を指定します。 The `6` は「金曜日」（週の 6 日目）を表し、 `3` は、その月の 3 番目の値を示します。 |
| `C` | 大文字の C | 最初のカレンダー「日」または「曜日」（これらのフィールドでのみ使用可能）。 例えば、 `1C` 「日」の場合は、5 日目以降に発生するカレンダーの最初の日をスケジュールします。 「曜日」フィールドに、 `1C` は、日曜日以降に発生するカレンダーの最初の日をスケジュールします。 |

「ルール」ボックスの時間間隔の例を次に示します。

* `0 0 12 * * ?` ：毎日正午
* `0 15 10 ? * *` ：毎日午前 10 時 15 分
* `0 0/5 14 * * ?`：毎日午後 2:00 ～ 2:55 までの 5 分ごと
* `0 0/5 14,18 * * ?` ：毎日午後 2:00 ～ 2:55 まで 5 分おき、毎日午後 6:00 ～ 6:55 まで 5 分おき
* `0 10,44 14 ? 3` :3 月の毎週水曜日の午後 2:10 と午後 2:44 に水
* `0 15 10 ? *` ：月～金、平日の午前 10:15
* `0 15 10 20 * ?` ：毎月 20 日の午前 10 時 15 分
* `0 15 10 L * ?` ：毎月最終日の午前 10:15
* `0 15 10 ? * 6L` ：毎月最終金曜日の午前 10:15
* `0 15 10 * * 6#3` ：毎月第 3 金曜日の午前 10 時 15 分

## アップロードジョブまたは公開ジョブをトリガーとして使用 {#using-an-upload-or-publish-job-as-a-trigger}

FTP を使用してアセットをアップロードする場合や公開ジョブを実行する場合は、アップロードが完了した時点で後続のジョブを開始するようにスケジュールできます。 （他のジョブが開始するようにスケジュールされている場合、ここでスケジュールしたジョブは後ろのキューに追加されます）。 新しいジョブは、指定したアドレスに通知を送信し、その場所にあるコードをトリガーできるようにします。 この継続されるアップロードジョブの名前は、現在のアップロードジョブと同じ名前になりますが、先頭に _Pub が付きます。

1 つのアップロードジョブまたは公開ジョブを別のトリガーにするには、 **[!UICONTROL 詳細]** をクリックします。 次に、「HTTP 通知」テキストフィールドに URL を入力します。
