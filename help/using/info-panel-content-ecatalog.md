---
title: eCatalog 内の情報パネルのコンテンツを管理
description: Adobe Dynamic Media Classicの eCatalog で情報パネルのコンテンツを管理する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 57%

---

# eCatalog 内の情報パネルのコンテンツを管理{#managing-info-panel-content-in-ecatalogs}

eCatalog 内のロールオーバーに画像マップテキストを使用するだけでなく、情報パネルを使用して、リンクを含む多数のロールオーバーテキストを追加できます。また、期限付きキャッシュを使用し、コンテンツを更新するスケジュールを設定して、情報パネルを管理することもできます。

Adobe Dynamic Media Classicの次の機能を使用して、情報パネルの設定とデータを管理できます。

* 情報パネル設定パネルでは、情報パネルのテキスト表示に使用するテンプレート、エラーのデフォルト応答、情報をキャッシュする時間数を指定できます。eCatalog を自動的に公開するかどうかを指定することもできます。
* 情報パネルのデータフィードパネルでは、情報パネルのロールオーバーテキストに表示するテキストを含む CSV ファイルを指定し、情報を更新する時間をスケジュールできます。
* メタデータを取り込みダイアログボックス（ページをマップビューからアクセス）では、ロールオーバーテキストの情報を含むタブ区切りの TXT ファイルを読み込むことができます。ロールオーバーテキストには、この TXT オプションまたはデータフィードパネルの CSV ファイルオプションを使用できます。
* ページをマップビューには、特定の画像マップに表示する xml をプレビューするオプションがあります。

## eCatalog 用の応答テンプレートの設定 {#set-up-a-response-template-for-ecatalogs}

情報パネルでのテキスト表示に使用する応答テンプレートを 3 つのプリセットから選択できます。これらのプリセットの応答テンプレートによって、情報パネルでの情報の表示方法、行数と列数、文字サイズ、フォントなどが決まります。プリセットの応答テンプレートを選択することも、独自のテンプレートを作成することもできます。

>[!NOTE]
>
>ビューアプリセットで応答テンプレートを設定することもできます。代わりに応答テンプレートをビューアプリセットで使用するには、を追加します。 `fmt=1` をビューアプリセットの情報サーバ URL の最後に追加します。
>
>詳しくは、 [eCatalog ビューアプリセットの設定](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. eCatalog をダブルクリックすると、詳細ビューで開きます。
1. を選択します。 **[!UICONTROL 情報パネルの設定]** パネル。
1. 次のいずれかの方法で応答テンプレートを選択します。

   * 応答テンプレートメニューからプリセットを選択します。テンプレートデザインの XML が「ユーザテンプレート」ボックスに表示されます。
   * 独自の応答テンプレートを作成するには、「 **[!UICONTROL カスタム]**. 「ユーザテンプレート」ボックスに、テンプレートの XML 定義を入力します。プリセットのテンプレートを基に、独自のテンプレートを作成できます。

1. （オプション）「デフォルトの応答」ボックスに、画像マップの情報の取得でAdobe Dynamic Media Classicがエラーになった場合に表示するテキストを入力します。 例えば、システムで会社名と eCatalog 名は取得されるが、ロールオーバー識別子は取得されない場合に、このメッセージがユーザに表示されます。
1. 「応答 TTL」ボックスに、データをキャッシュするまでの時間数を入力します。

   * データが 1 日中頻繁に更新される場合は、数値を小さくします。
   * データが比較的安定しており、1 日を通じて頻繁に更新する必要がない場合は、数値を大きくします。 初期設定は 10 時間です。

1. 選択 **[!UICONTROL 公開]**.

## eCatalog の情報パネルのソースコンテンツを読み込む {#import-source-content-for-the-info-panel-in-ecatalogs}

eCatalog の情報パネルのソーステキストには、カンマ区切り形式（CSV）またはタブ区切り形式（TXT）のファイルを使用できます。タブ区切り形式のファイルは、エンコードが UTF16（Unicode）である必要があります。ファイルの種類によって、読み込む方法が異なります。

ソースコンテンツの形式を設定するときは、次のガイドラインに従ってください。

* タブやカンマで区切ったデータに、ロールオーバーテンプレートに必要な列数があることを確認します。
* データの最初の項目または列をロールオーバー識別子（画像マップ URL の rollover_key 値に関連付けられている）にします。
* 識別子の後の各タブ区切りまたはコンマ区切りの項目が、応答テンプレート内で置き換える項目であることを確認します。したがって、最初の列は$1$に、2 番目の列は$2$に置き換えられます。

### CSV コンテンツを外部でホストされている場所から eCatalog に読み込む {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. eCatalog をダブルクリックすると、詳細ビューで開きます。
1. を選択します。 **[!UICONTROL InfoPanel Datafeed]** パネル。
1. 「外部にホストされている CSV ファイルの場所」ボックスに CSV ファイルの URL を入力します。URL はこのフィールドにペーストすることも、直接入力することもできます。
1. （オプション）更新をスケジュールメニューを使用して、コンテンツを更新する時間を指定し、 **[!UICONTROL 追加]**. 複数の更新時刻を選択できます。各更新時刻は「時間を更新」ボックスに表示されます( 時間を削除するには、時間を選択し、 **[!UICONTROL 削除]**.)
1. （オプション）「 」を選択します。 **[!UICONTROL 今すぐ更新を実行]** 」をクリックして、コンテンツを直ちに更新します。

### タブ区切りファイルまたは CSV ファイルの読み込み {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. eCatalog をダブルクリックすると、詳細ビューで開きます。
1. を選択します。 **[!UICONTROL 情報パネルの設定]** パネル。
1. 選択 **[!UICONTROL S7Info コンテンツをアップロード]**.
1. 選択 **[!UICONTROL 参照]**、使用するタブ区切りの TXT ファイル、CSV ファイルまたは SSV ファイルを選択し、「 」を選択します。 **[!UICONTROL 開く]**.
1. 選択 **[!UICONTROL アップロード]**.

Adobe Dynamic Media Classicから、アップロードが成功したかどうかを知らせる電子メールが送信されます。

## 画像マップのロールオーバーキーテキストのプレビュー {#preview-rollover-key-text-for-an-image-map}

ページをマップ画面を使用すると、eCatalog の特定のページにある画像マップの情報パネルテキストを簡単に表示することができます。

1. カタログのロールオーバーを選択 **[!UICONTROL 編集]** 」ボタンをクリックします。
1. 選択 **[!UICONTROL ページをマッピング]**.
1. 画面の右側にあるテーブルの上部で、「 」を選択します。 **[!UICONTROL 情報パネル]** を選択します。

   情報パネルテキストを含む各画像マップの横にロールオーバーキーテキストが表示されます。
