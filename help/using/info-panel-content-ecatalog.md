---
title: eCatalog の情報パネルコンテンツの管理
description: Adobe Dynamic Media Classicの eCatalog で情報パネルコンテンツを管理する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: bfb9c5a4-5068-4adb-9fe2-a4ead8656289
topic: Integrations
level: Experienced
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '871'
ht-degree: 53%

---

# eCatalog の情報パネルコンテンツの管理{#managing-info-panel-content-in-ecatalogs}

eCatalog 内のロールオーバーに画像マップテキストを使用するだけでなく、情報パネルを使用して、リンクを含む多数のロールオーバーテキストを追加できます。また、時間制限されたキャッシュを使用したり、コンテンツの更新をスケジュールしたりして、InfoPanel を管理することもできます。

Adobe Dynamic Media Classicの以下の機能を使用して、InfoPanel の設定とデータを管理できます。

* 情報パネル設定パネルでは、情報パネルのテキスト表示に使用するテンプレート、エラーのデフォルト応答、情報をキャッシュする時間数を指定できます。eCatalog を自動的に公開するかどうかを指定することもできます。
* InfoPanel データフィードパネルでは、InfoPanel ロールオーバーテキストに表示するテキストを含む CSV ファイルを指定し、情報を更新する時間をスケジュールできます。
* メタデータを取り込みダイアログボックス（ページをマップビューからアクセス）では、ロールオーバーテキストの情報を含むタブ区切りの TXT ファイルを読み込むことができます。ロールオーバーテキストには、この TXT オプションまたはデータフィードパネルを CSV ファイルオプションと共に使用できます。
* ページをマップビューには、特定の画像マップに表示する xml をプレビューするオプションがあります。

## eCatalog の応答テンプレートの設定 {#set-up-a-response-template-for-ecatalogs}

情報パネルでのテキスト表示に使用する応答テンプレートを 3 つのプリセットから選択できます。これらのプリセットの応答テンプレートによって、情報パネルでの情報の表示方法、行数と列数、文字サイズ、フォントなどが決まります。プリセットの応答テンプレートを選択することも、独自のテンプレートを作成することもできます。

>[!NOTE]
>
>ビューアプリセットで応答テンプレートを設定することもできます。ビューアプリセットで応答テンプレートを代わりに使用するには、次を追加します。 `fmt=1` をビューアプリセット内の情報サーバー URL の末尾に追加します。
>
>参照： [eCatalog ビューアプリセットの設定](setting-ecatalog-viewer-presets.md#setting_up_ecatalog_viewer_presets).

1. eCatalog をダブルクリックして、詳細表示で開きます。
1. 「」を選択します **[!UICONTROL InfoPanel セットアップ]** パネル。
1. 次のいずれかの方法で応答テンプレートを選択します。

   * 応答テンプレートメニューからプリセットを選択します。テンプレートデザインの XML が「ユーザテンプレート」ボックスに表示されます。
   * 独自の応答テンプレートを作成するには、以下を選択します **[!UICONTROL カスタム]**. 「ユーザテンプレート」ボックスに、テンプレートの XML 定義を入力します。プリセットのテンプレートを基に、独自のテンプレートを作成できます。

1. （オプション）「デフォルトのレスポンス」ボックスに、イメージマップの情報の取得でAdobe Dynamic Media Classicでエラーが発生した場合に表示するテキストを入力します。 例えば、システムで会社名と eCatalog 名は取得されるが、ロールオーバー識別子は取得されない場合に、このメッセージがユーザに表示されます。
1. 「応答 TTL」ボックスに、データをキャッシュするまでの時間数を入力します。

   * データが 1 日中頻繁に更新される場合は、数値を小さくします。
   * データが比較的安定しており、1 日を通じて頻繁に更新する必要がない場合は、この値を大きくします。 初期設定は 10 時間です。

1. を選択 **[!UICONTROL 公開]**.

## eCatalogs の情報パネルのソースコンテンツの読み込み {#import-source-content-for-the-info-panel-in-ecatalogs}

eCatalog の情報パネルのソーステキストには、カンマ区切り形式（CSV）またはタブ区切り形式（TXT）のファイルを使用できます。タブ区切り形式のファイルは、エンコードが UTF16（Unicode）である必要があります。ファイルの種類によって、読み込む方法が異なります。

ソースコンテンツの形式を設定するときは、次のガイドラインに従ってください。

* タブやカンマで区切ったデータに、ロールオーバーテンプレートに必要な列数があることを確認します。
* データの最初の項目または列をロールオーバー識別子（画像マップ URL の rollover_key 値に関連付けられている）にします。
* 識別子の後の各タブまたはコンマ区切りの項目が、応答テンプレートに置き換える項目であることを確認してください。 したがって、最初の列は$1$に、2 番目の列は$2$に、というように置き換えられます。

### 外部でホストされている場所から eCatalog に CSV コンテンツを読み込む {#import-csv-content-into-ecatalogs-from-an-externally-hosted-location}

1. eCatalog をダブルクリックして、詳細表示で開きます。
1. 「」を選択します **[!UICONTROL InfoPanel データフィード]** パネル。
1. 「外部にホストされている CSV ファイルの場所」ボックスに CSV ファイルの URL を入力します。URL はこのフィールドにペーストすることも、直接入力することもできます。
1. （オプション） スケジュール更新メニューを使用してコンテンツを更新する時間を指定し、次のオプションを選択します **[!UICONTROL 追加]**. 複数の更新時刻を選択できます。各更新時刻は「時間を更新」ボックスに表示されます（時間を削除するには、時間を選択して次を選択します **[!UICONTROL 削除]**.）
1. （オプション）を選択 **[!UICONTROL 今すぐ更新を実行]** コンテンツを直ちに更新します。

### タブ区切りファイルまたは CSV ファイルの読み込み {#import-a-tab-delimited-or-csv-file}

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>SR changed this section 10/23/2012</p>

 -->

1. eCatalog をダブルクリックして、詳細表示で開きます。
1. 「」を選択します **[!UICONTROL InfoPanel セットアップ]** パネル。
1. を選択 **[!UICONTROL S7Info コンテンツのアップロード]**.
1. を選択 **[!UICONTROL 参照]**&#x200B;で、使用するタブ区切り TXT ファイル、CSV ファイル、SSV ファイルを選択し、を選択します **[!UICONTROL 開く]**.
1. を選択 **[!UICONTROL Upload]**.

Adobe Dynamic Media Classicから電子メールメッセージが送信され、アップロードが成功したかどうかが通知されます。

## 画像マップのロールオーバーキーテキストのプレビュー {#preview-rollover-key-text-for-an-image-map}

ページをマップ画面を使用すると、eCatalog の特定のページにある画像マップの情報パネルテキストを簡単に表示することができます。

1. カタログのロールオーバーの選択 **[!UICONTROL 編集]** ボタン。
1. を選択 **[!UICONTROL ページのマッピング]**.
1. 画面右側のテーブルの上部で、次を選択します **[!UICONTROL 情報パネル]** 表示メニューから選択します。

   情報パネルテキストを含む各画像マップの横にロールオーバーキーテキストが表示されます。
