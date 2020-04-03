---
title: eCatalogでの情報パネルのコンテンツの管理
seo-title: eCatalogでの情報パネルのコンテンツの管理
description: 'null'
seo-description: eCatalogで情報パネルのコンテンツを管理する方法を説明します。
uuid: 5aa634f9-0874-4bb5-a3d9-8ce4d5577941
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
discoiquuid: be277831-77cc-4011-ae30-e75c18eec99b
translation-type: tm+mt
source-git-commit: d5bf894d56687561c93ef08762bc19d3597225e6

---


# eCatalogでの情報パネルのコンテンツの管理{#managing-info-panel-content-in-ecatalogs}

eCatalog 内のロールオーバーに画像マップテキストを使用するだけでなく、情報パネルを使用して、リンクを含む多数のロールオーバーテキストを追加できます。また、期限付きキャッシュを使用し、コンテンツを更新するスケジュールを設定して、情報パネルを管理することもできます。

Dynamic Media Classicの次の機能を使用して、情報パネルの設定とデータを管理できます。

* 情報パネル設定パネルでは、情報パネルのテキスト表示に使用するテンプレート、エラーのデフォルト応答、情報をキャッシュする時間数を指定できます。eCatalog を自動的に公開するかどうかを指定することもできます。
* 情報パネルのデータフィードパネルでは、情報パネルのロールオーバーテキストに表示するテキストを含む CSV ファイルを指定したり、情報を更新する時刻を設定したりできます。
* メタデータを取り込みダイアログボックス（ページをマップビューからアクセス）では、ロールオーバーテキストの情報を含むタブ区切りの TXT ファイルを読み込むことができます。ロールオーバーテキストには、この TXT オプションまたはデータフィードパネルの CSV ファイルオプションを使用できます。
* ページをマップビューには、特定の画像マップに表示する xml をプレビューするオプションがあります。

## eCatalogの応答テンプレートの設定 {#set-up-a-response-template-for-ecatalogs}

情報パネルでのテキスト表示に使用する応答テンプレートを 3 つのプリセットから選択できます。これらのプリセットの応答テンプレートによって、情報パネルでの情報の表示方法、行数と列数、文字サイズ、フォントなどが決まります。プリセットの応答テンプレートを選択することも、独自のテンプレートを作成することもできます。

>[!NOTE]
>
>ビューアプリセットで応答テンプレートを設定することもできます。To use the Response Template in the Viewer Preset instead, add `fmt=1` to the end of the Information Server URL in the Viewer Preset.
>
>詳しくは、[eCatalog ビューアプリセットの設定](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets)を参照してください。

1. eCatalog をダブルクリックして詳細ビューで開きます。
1. 情報パネル設定パネルをクリックして開きます。
1. 次のいずれかの方法で応答テンプレートを選択します。

   * 応答テンプレートメニューからプリセットを選択します。テンプレートデザインの XML が「ユーザテンプレート」ボックスに表示されます。
   * 「カスタム」を選択して、独自の応答テンプレートを作成します。「ユーザテンプレート」ボックスに、テンプレートの XML 定義を入力します。プリセットのテンプレートを基に、独自のテンプレートを作成できます。

1. （オプション）「初期設定の応答」ボックスに、画像マップの情報を取得する際にエラーが発生した場合に表示するテキストを入力します。 例えば、システムで会社名と eCatalog 名は取得されるが、ロールオーバー識別子は取得されない場合に、このメッセージがユーザに表示されます。
1. 「応答 TTL」ボックスに、データをキャッシュするまでの時間数を入力します。

   * データが 1 日中頻繁に更新される場合は、数値を小さくします。
   * データの変更が比較的少なく、頻繁に更新する必要がない場合は、数値を大きくします。初期設定は 10 時間です。

1. Click **Publish**.

## Import source content for the Info Panel in eCatalogs {#import-source-content-for-the-info-panel-in-ecatalogs}

eCatalog の情報パネルのソーステキストには、カンマ区切り形式（CSV）またはタブ区切り形式（TXT）のファイルを使用できます。タブ区切り形式のファイルは、エンコードが UTF16（Unicode）である必要があります。ファイルの種類によって、読み込む方法が異なります。

ソースコンテンツの形式を設定するときは、次のガイドラインに従ってください。

* タブやカンマで区切ったデータに、ロールオーバーテンプレートに必要な列数があることを確認します。
* データの最初の項目または列をロールオーバー識別子（画像マップ URL の rollover_key 値に関連付けられている）にします。
* 識別子の後のタブまたはカンマで区切った各項目を、応答テンプレート内で置換する項目にします（最初の列は $1$、2 番目の列は $2$ などと置換される）。

### Import CSV content into eCatalogs from an externally hosted location {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. eCatalog をダブルクリックして詳細ビューで開きます。
1. 情報パネルのデータフィードパネルをクリックして開きます。
1. 「外部にホストされている CSV ファイルの場所」ボックスに CSV ファイルの URL を入力します。URL はこのフィールドにペーストすることも、直接入力することもできます。
1. （オプション）スケジュールを更新メニューを使用してコンテンツの更新時刻を指定し、「追加」をクリックします。複数の更新時刻を選択できます。各更新時刻は「時間を更新」ボックスに表示されます（時刻を削除するには、その時刻を選択して「削除」をクリックします）。
1. （オプション）「今すぐ更新を実行」をクリックして、コンテンツをすぐに更新します。

### タブ区切りファイルまたは CSV ファイルの読み込み {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. eCatalog をダブルクリックして詳細ビューで開きます。
1. 情報パネル設定パネルをクリックして開きます。
1. **「S7Infoコンテンツをアップロード」をクリックします**。
1. Click **Browse**, select the tab-delimited TXT file, CSV or SSV file you want to use, and click **Open**.
1. 「**アップロード**」をクリックします。

ダイナミックMedia Classicから、アップロードが成功したかどうかを知らせる電子メールが送信されます。

## 画像マップのロールオーバーキーテキストのプレビュー {#preview-rollover-key-text-for-an-image-map}

ページをマップ画面を使用すると、eCatalog の特定のページにある画像マップの情報パネルテキストを簡単に表示することができます。

1. eCatalog のロールオーバー時に表示される「編集」ボタンをクリックします。
1. 「ページをマップ」をクリックします。
1. 画面右側の上部にある表で、表示メニューから「情報パネル」を選択します。

   情報パネルテキストを含む各画像マップの横に、rollover-key テキストが表示されます。

