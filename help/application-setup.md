---
title: アプリケーション設定
description: Adobe Dynamic Media Classicのアプリケーション領域を設定する方法について説明します。 アプリケーション領域では、一般的な設定の入力、画像、ビューアおよびビデオエンコーディングプリセットの作成、初期設定のビューアとメタデータの定義、公開設定およびビデオ SEO 設定を行うことができます。 また、この領域を使用してバッチセットプリセットを設定し、2D スピンセットを自動生成することもできます。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: 3f96606e-ef5c-4c01-aa0f-3148f14e28be
source-git-commit: 121081e90b68357f7602924cd6ced0c0256b378f
workflow-type: tm+mt
source-wordcount: '11303'
ht-degree: 42%

---

# アプリケーション設定{#application-setup}

アプリケーション設定ページを使用して、一般設定の入力、画像プリセットの作成、ビデオエンコーディングプリセット、ビューアプリセットの作成、デフォルトのビューアおよびメタデータの定義を行うことができます。 バッチセットプリセットを設定して、2D スピンセット（例： ）、公開設定、ビデオ SEO 設定を自動生成することもできます。

>[!NOTE]
>
>Adobe Dynamic Media Classic管理者のみが、アプリケーション設定ページで設定を変更できます。

## 全般設定 {#general-settings}

アプリケーションの一般設定ページを開くには、グローバルナビゲーションバーで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 一般設定]**.

### サーバ

アカウントの作成時に、Adobe Dynamic Media Classicが会社に割り当てられたサーバーを自動的に提供します。 これらのサーバは、Web サイトとアプリケーションの URL 文字列を生成するのに使用されます。これらの URL 呼び出しは、アカウントに固有です。

関連トピック [セキュアテストサービスのテスト](testing-assets-making-them-public.md#testing_the_secure_testing_service).

* **[!UICONTROL 公開先サーバー名]**  — このサーバーは、アカウントに固有のすべてのシステム生成 URL 呼び出しで使用される、ライブコンテンツ配信ネットワーク (CDN) サーバーです。 Adobe Dynamic Media Classicのサポート技術者に指示されない限り、このサーバー名を変更しないでください。

* **[!UICONTROL オリジンサーバー名]**  — このサーバーは、品質保証テストにのみ使用されます。 Adobe Dynamic Media Classicのサポート技術者から指示されない限り、このサーバー名を変更しないでください。

<!-- **AGM Server Name** This server is used for Web-to-Print templates. This server is set on a company-wide basis. Do not change this server name unless instructed to do so by an Adobe DynamicMedia Classic support technician. -->

* **[!UICONTROL Test&amp;Target サーバ名]** - Test&amp;Target の URL （.com まで）。 この URL の取得方法については、統合を参照してください。 [!DNL Adobe Dynamic Media Classic] と [!DNL Adobe Target Standard/Premium].

<!-- **Test Publish Context Server Name** -->

* **[!UICONTROL iOSストリーミングサーバ名]** - [!DNL Adobe Dynamic Media Classic] iOSストリーミングサーバ このサーバは、HTTP プロトコルを使用して iOS ベースのデバイスにストリーミングビデオを配信します。

* **[!UICONTROL プログレッシブビデオサーバ名]** - [!DNL Adobe Dynamic Media Classic] プログレッシブビデオサーバ。 このサーバは、HTTP プロトコルを使用してプログレッシブビデオを配信します。

* **[!UICONTROL 非公開アセットの URL を表示]**  — 必要に応じて、このオプションを選択します [!DNL Adobe Dynamic Media Classic] ：アセットをプレビューする際に、公開されているかどうかに関わらず URL を表示します。 アセットが公開されていない場合は、URL は機能しません。ただし、この URL を予定や組織的な目的で使用することができます。

<!-- **Allow AIR install** Select this option to allow users to download Adobe Dynamic Media Classic desktop version to their local hard drives. Users install the application from the Desktop Version area of the Personal Setup screen. -->

<!-- AIR users must manually uninstall their existing app and reinstall from the web version of Adobe Dynamic Media Classic (in Personal Settings). After this one-time reinstallation, you are prompted to upgrade whenever the server has a newer version of Adobe Dynamic Media Classic AIR. Adobe Dynamic Media Classic is integrated with the Application Update Framework which streamlines the upgrade process. -->

* **[!UICONTROL CDN 無効化テンプレート]** - CDN（コンテンツ配信ネットワーク）キャッシュの無効化に使用するテンプレートを指定します。

   例えば、を参照する画像 URL（画像プリセットまたは画像の修飾子を含む）を入力するとします `<ID>`の代わりに、次の例のように特定の画像 ID を使用します。

   `https://sample.scene7.com/is/image/Company/<ID>?$s7product$`

   テンプレートにが含まれている場合 `<ID>`その後、Adobe Dynamic Media Classicが `https://<server>/is/image`で、 `<server>` は、一般設定で定義される公開サーバー名です。

   CDN 無効化テンプレートを設定し、 Backpack_B という名前の画像を選択して、 **[!UICONTROL ファイル]** > **[!UICONTROL CDN を無効にする]** CDN 無効化インターフェイスでは、次のように生成された URL が生成されます。

   `https://sample.scene7.com/is/image/Company/Backpack_B?$s7product$`

   URL リストボックスで、 **[!UICONTROL 続行]** をクリックして、特定の画像 URL 呼び出しのキャッシュをクリアします。 また、URL リストボックスに URL を入力または貼り付けて、URL を追加することもできます。事前にテンプレートを設定する必要はありません。

   CDN 無効化テンプレートを選択して CDN 無効化リクエストをおこなうと、ユーザーインターフェイスにインジケーターがポップアップ表示されます。 キャッシュのクリアに要する時間の見積もりを提供します。

   同様に、Adobe Dynamic Media Classic内で **[!UICONTROL ファイル]** > **[!UICONTROL CDN を無効にする]**&#x200B;の場合、各画像は、保存されたテンプレート URL で参照されます。 したがって、Web サイトで参照される各 URL（製品の詳細や検索結果など）を参照する CDN 無効化テンプレートを定義できます。 これにより、キャッシュの無効化の対象として 1 つ以上の画像を選択したときに、それらの URL が自動的にインターフェイスに入力されます。

   詳しくは、[コンテンツのキャッシング](dmc-platform-overview.md#content_caching)を参照してください。

   詳しくは、[アセットの再公開と CDN の遅延](publishing-files.md#republished_assets_and_cdn_delays)を参照してください。

### 参照

* **[!UICONTROL プロジェクトを表示]**  — プロジェクトをAdobe Dynamic Media Classicのアセット編成の手段として使用できるかどうかを指定します。 詳しくは、 [プロジェクトで作業を整理する](/help/organizing-projects.md).

* **[!UICONTROL サンプルの eVideo コンテンツを表示]** - eVideo サンプルコンテンツの表示をオンまたはオフにします。

* **[!UICONTROL 生成されたコンテンツを表示]**  — フォルダーに、アセットから生成されたコンテンツを表示します。 例えば、PDFファイルがアップロード時にラスタライズされると、Adobe Dynamic Media Classicは元のPDFの各ページに対して 1 つの画像を作成します。 「生成されたコンテンツを表示」が選択されている場合、元の PDF がアップロードされたときに生成された各画像が、PDF がアップロードされたフォルダの PDF とともに表示されます。

* **[!UICONTROL エンコードされたビデオを表示]**  — デフォルトでは選択解除（オフ）されています。

   エンコードされた、同じビデオから派生したものを多数検索する必要なく、Adobe Dynamic Media Classicでビデオをすばやく検索および参照するには、このオプションをオフ（デフォルト）にします。 マスタービデオサムネール（アップロードし、派生物の作成に使用したソースビデオ）と、「親」アダプティブビデオセットサムネール（エンコードされたビデオセットの「子」派生物を含む）のみが表示されます。

   ただし、「マスタービデオ」または「アダプティブビデオセット」から、個々のエンコードされたビデオにアクセスできます。このようなアクセスを行うには、ビデオサムネール画像をダブルクリックして、詳細ビューを開きます。次に、 **[!UICONTROL エンコードされたビデオ]** をクリックし、すべての「子」ビデオにアクセスできるようにします。

   また、 **[!UICONTROL ファイル]** > **[!UICONTROL 再処理]** を使用して、アダプティブビデオセットから直接、エンコードされた「子」ビデオを作成します。 Adobe Dynamic Media Classicは、アダプティブビデオセットの「親」マスタービデオを自動的に検索し、それをソースビデオとしてトランスコードに使用します。 ただし、新しく作成した個々のエンコードされたビデオを保存すると、検索または参照するときには表示されません。しかし、詳細ビューの「エンコードされたビデオ」タブからはアクセスできます。

   詳しくは、 [ビデオのアップロードとトランスコード](uploading-encoding-videos.md#uploading_and_encoding_videos).

   検索または参照時に、エンコードされたすべてのビデオ派生物にアクセスできるようにしておくには、**[!UICONTROL 「エンコードされたビデオを表示」]**&#x200B;を選択します。

   ビルドメニューには、個々のビデオでのみ機能する、または、オプションで機能するアクションがあります。この機能により、**[!UICONTROL 「エンコードされたビデオを表示」]**&#x200B;がどう設定されているかに関係なく、エンコードされたすべてのビデオ派生物を必ず表示するようになり、ユーザはその中から選択できます。上書きするビルドアクション **[!UICONTROL エンコードされたビデオを表示]** 含める設定 **[!UICONTROL アダプティブビデオセット]**、および **[!UICONTROL eCatalogs]**.

   >[!NOTE]
   >
   >Adobe Dynamic Media Classicを使用してビデオアセットをアップロードおよびエンコードしなかった場合、Adobe Dynamic Media Classicには、このオプションが選択解除されていても、個々にエンコードされたビデオがすべて表示されます。

* **[!UICONTROL サブフォルダの更新ボタンを表示]**  — サブフォルダの [ 更新 ] ボタンの表示/非表示を切り替えます。

### Adobe Dynamic Media Classic FTP アカウント

* **[!UICONTROL サーバー]** - FTP アカウントサーバーを一覧表示します。

* **[!UICONTROL ユーザー名]** - FTP アカウントのユーザー名を一覧表示します。

### アプリケーションへのアップロード

関連トピック [デフォルトのアップロードジョブオプション](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/569_Default%20Job%20Options_converted%20renamed_Getting%20Started-AVS) トレーニングビデオ。

* **[!UICONTROL 画像を上書き]** - Adobe Dynamic Media Classicでは、2 つのファイルに同じ名前を付けることは許可されていません。 各項目のAdobe Dynamic Media Classic ID（画像名からファイル名拡張子を取り除いた部分）は一意である必要があります。 この規則のため、アップロードダイアログボックスには上書きオプションがあります。このオプションの実際の効果は、指定した「画像を上書き」オプションによって異なります。これらのオプションは、置き換え画像のアップロード方法、つまり元の画像を置き換えるか、画像を重複させるかを指定します。重複する画像名には「-1」が付けられます（例えば、chair.tif は chair-1.tif に変更されます）。これらのオプションは、元の画像とは別のフォルダにアップロードされる画像や、元の画像と異なるファイル名拡張子（JPG、TIF、PNG など）を持つ画像に影響を与えます詳しくは、 [「画像を上書き」オプションを使用する](#using-the-overwrite-images-option).

   * **[!UICONTROL 現在のフォルダでベース名と拡張子が同じファイルを上書き]**  — このオプションは最も厳格な置換規則です。 置き換え画像を元の画像と同じフォルダにアップロードし、置き換え画像と元の画像のファイル名拡張子が同じになっている必要があります。これらの要件が満たされない場合は、重複する画像が作成されます。

   * **[!UICONTROL 現在のフォルダでベース名が同じファイルを上書き]**  — 置き換え画像を元の画像と同じフォルダーにアップロードする必要があります。ただし、ファイル名の拡張子は元の画像と異なる場合があります。 例えば、chair.jpg を chair.tif に置き換える場合などです。

   * **[!UICONTROL 任意のフォルダでベース名と拡張子が同じファイルを上書き]**  — 置き換え画像のファイル名拡張子が元の画像と同じである必要があります（例えば、chair.jpg は chair.tif ではなく chair.jpg を置き換える必要があります）。 ただし、置き換え画像を、元の画像と別のフォルダにアップロードできます。更新された画像は新しいフォルダにあり、元の場所のファイルはなくなります。

   * **[!UICONTROL 任意のフォルダでベース名が同じファイルを上書き]**  — このオプションは、最も包括的な置換規則です。 置き換え画像を、元の画像と別のフォルダにアップロードでき、ファイル名拡張子が異なるファイルをアップロードして、元のファイルと置き換えることができます。元のファイルが別のフォルダにある場合、置き換え画像は、アップロード先の新しいフォルダに存在します。

* **[!UICONTROL 公開を保持]** - Adobe Dynamic Media Classicにアップロードされた置き換え画像が、置き換える画像の「公開準備完了」設定を保持するか、アップロード時に設定を指定するかを指定します。

* **[!UICONTROL 初期設定のカラープロファイル]** - CMYK 画像を追加する際に、初期設定のカラープロファイルオプションの一部として適用するカラープロファイルを指定します。

* **[!UICONTROL デフォルトのアップロードオプション]**  — アップロードオプションをアップロードダイアログボックスが開きます。このダイアログボックスでは、デフォルトのアップロードオプションを指定できます。 これらのオプションについて詳しくは、[アップロードオプション](/help/uploading-files.md#upload_options)を参照してください。

### アプリケーションの画像マップエディタ

* **[!UICONTROL 初期設定の画像マッピング HREF]**  — 画像マッピングの HREF 列に使用されるデフォルトの URL を定義します。 この URL は、画像マップの作成時に表示されるデフォルトの URL です。

* **[!UICONTROL 初期設定の画像マッピングテンプレート]**  — 画像マッピングの HREF テンプレートのデフォルト JavaScript を定義します。 ここでカスタムコードを設定し、画像マップを選択したときに実行されるようにすることができます。

### アプリケーションのその他の設定

* **[!UICONTROL ごみ箱のクリーンアップの警告]**  — ごみ箱に入っているアセットは、7 日以内に自動的に削除されます。 ごみ箱内のアセットが完全に削除される 4 日前に会社の管理者に通知を送信する場合、「ごみ箱の項目が自動的に削除される前に電子メールを送信する」を選択します。詳しくは、 [ごみ箱フォルダーを管理](/help/trash-folder.md).

## 「画像を上書き」オプションを使用する {#using-the-overwrite-images-option}

Adobe Dynamic Media Classicでは、2 つのファイルに同じ名前を付けることは許可されていません。 各項目のAdobe Dynamic Media Classic ID（画像名からファイル名拡張子を取り除いた部分）は一意である必要があります。 この規則のため、アップロードダイアログボックスには「画像を上書き」オプションがあります。このオプションの正確な効果は、各会社のAdobe Dynamic Media Classic内部設定の設定によって異なります。

以前に画像をアップロードしてから元のファイルを変更（または置き換え）した場合、「上書き」オプションを選択すると、Adobe Dynamic Media Classicによる画像の置き換え方法が指定されます。 画像に関する情報は変わりませんが、古い画像は新しい画像に置き換わります。フォルダーに、まだAdobe Dynamic Media Classicにない画像も含まれている場合、これらの画像は追加されます。

アップロードした画像が何らかの形で変更された（画像が変更された）が、画像への参照が同じままの場合には、このオプションを使用します。Adobe® PDF をアップロードしてリッピングする場合にも、上書きは便利です。Adobe Dynamic Media Classicを微調整するには *リップ* 画像をアップロードし、アップロードダイアログボックスで ICC カラープロファイルオプションを調整して、上書き機能を使用して再アップロードします。

実稼動サーバーからの画像にアクセスするために使用されるAdobe Dynamic Media Classic ID は、画像ファイル名から派生します。 ファイル名に使用する大文字と小文字は、既存のファイルの置き換え時と、画像へのアクセスに使用されるAdobe Dynamic Media Classic ID の両方で重要です。 Adobe Dynamic Media Classicにアップロードする前に、ファイル名での大文字と小文字の使用が正しいことを確認してください。同じ画像で大文字と小文字が異なるAdobe Dynamic Media Classic ID が使用されないようにします。

このオプションを選択しない場合、既存の画像と同じファイル名のすべての画像は、重複と見なされて追加されません。

## 画像プリセット {#image-presets}

画像プリセット画面は、画像プリセットを作成および編集するのに使用します。画像プリセットを使用すると、Adobe Dynamic Media Classicは同じマスター画像から異なるサイズの画像を動的に配信できます。 各画像プリセットは、画像を表示するための定義済みサイズおよび形式に関するコマンドの集まりです。画像プリセットを作成する際に、画像配信用のサイズを選択します。 また、表示用に画像を配信する際に、画像の外観を最適化するための書式設定コマンドを選択します。

管理者は、アセット書き出し用のプリセットを作成できます。ユーザーは、画像を書き出す際にプリセットを選択できます。また、管理者が指定した仕様に合わせて画像を再フォーマットできます。

画像プリセット画面を開くには、グローバルナビゲーションバーでに移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**.

詳しくは、 [スマートイメージング](https://experienceleague.adobe.com/docs/experience-manager-65/assets/dynamic/imaging-faq.html#dynamic).

### 画像プリセットの作成と編集 {#creating-and-editing-image-presets}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**.
1. プリセットを作成するか、既存のプリセットから開始します。

   * **画像プリセットの作成**  — 選択 **[!UICONTROL 追加]**.
   * **既存のプリセットからの画像プリセットの作成**  — 作成したい画像プリセットに最も近い画像プリセットを選択し、「 **[!UICONTROL 編集]**.

1. プリセットを追加（または編集）ページで、プリセットの名前を入力します。
1. 目的のプリセットオプションを設定します。

   詳しくは、[画像プリセットのオプション](application-setup.md#image_preset_options)を参照してください。

1. 選択 **[!UICONTROL 保存]**&#x200B;または既存のプリセットから開始した場合は、「 」を選択します。 **[!UICONTROL 名前を付けて保存]**.
1. 独自の画像でプリセットをプレビューするには、「 」を選択します。 **[!UICONTROL 参照]** 画像を選択します。 デフォルトの画像でプレビューする場合は、「 **[!UICONTROL リセット]**.

画像プリセットを編集するには、画像プリセット画面で名前を選択し、次に「 」を選択します **[!UICONTROL 編集]**. 画像プリセットを削除するには、削除する画像プリセットを選択し、 **[!UICONTROL 削除]**.

### 画像プリセットのオプション {#image-preset-options}

プリセットを追加画面およびプリセットを編集画面には、画像プリセットを作成および編集するための次のオプションがあります。

* **[!UICONTROL プリセット名]**  — スペースを含めずに、わかりやすい名前を入力します。 ユーザーがこの画像プリセットを識別しやすくするために、名前に画像サイズの仕様を含めます。

* **[!UICONTROL 幅と高さ]**  — 画像が配信されるサイズをピクセル単位で入力します。

* **[!UICONTROL 形式]**  — メニューからフォーマットを選択します。 「GIF」、「JPEG」、「PDF」または「TIFF」の形式を選択すると、次のような選択肢が表示されます。

   * GIF カラー量子化オプション

      * **[!UICONTROL タイプ]** - 「アダプティブ」（デフォルト）、「Web」または「Macintosh」を選択します。 次を選択した場合、 **[!UICONTROL GIF（アルファ付き）]**&#x200B;の場合、「Macintosh」オプションは使用できません。

      * **[!UICONTROL ディザ]** - 「拡散」または「オフ」を選択します。

      * **[!UICONTROL 色数]**  — スライダーをドラッグして 2-255 と入力します。

      * **[!UICONTROL カラーリスト]**  — コンマ区切りのリストを入力します。 たとえば、白、灰色、黒の場合は、と入力します。 `000000,888888,ffffff`.
   * JPEG オプション

      * **[!UICONTROL 品質]**  — 圧縮レベルのJPEGを制御します。 この設定は、ファイルサイズと画質の両方に影響を与えます。JPEG品質は 1～100 である。

      * **[!UICONTROL JPGの色度ダウンサンプリングを有効にする]**  — 目は高周波の色情報に対して高周波の輝度より感度が低いので、JPEG画像は画像情報を輝度と色成分に分割する。 JPEG 画像を圧縮すると、輝度成分は最大解像度が維持され、色成分はピクセルのグループの平均化によりダウンサンプリングされます。ダウンサンプリングにより、知覚される品質にほとんど影響を与えることなく、データ量が 1/2 から 1/3 に削減されます。ダウンサンプリングは、グレースケール画像では使用できません。この方法は、コントラストが高い画像（テキストがオーバーレイされた画像など）で圧縮の量を低減させるのに役立ちます。
   * PDF および TIFF のオプション

      * **[!UICONTROL 圧縮]**  — 圧縮アルゴリズムを選択します。



* **[!UICONTROL カラースペース]**  — カラースペースを選択します。

* **[!UICONTROL シャープ]** - 「シンプルシャープを有効にする」オプションを選択すると、すべての拡大縮小の実行後、画像に対して基本的なシャープフィルターが適用されます。 シャープにより、異なるサイズで画像を表示したときに生じるぼかしを補正できます。

   シャープ、再サンプルモードおよびアンシャープマスクについて詳しくは、 [画像にシャープを適用](sharpening-image.md#sharpening_an_image). 関連トピック [シャープ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/547_sharpening1_converted%20renamed_Done-AVS) トレーニングビデオ。

* **[!UICONTROL 再サンプルモード]** - 「再サンプリングモード」オプションを選択します。 これらのオプションは、ダウンサンプリングした画像をシャープにします。

* **[!UICONTROL B 線形]**  — 最も速い再サンプリング方法。目に見えるエイリアスアーティファクトが一部発生します。

* **[!UICONTROL バイキュービック法]** - Image Server の CPU 使用率は増加しますが、目に見えるエイリアスアーティファクトが減少した、よりシャープな画像が得られます。

* **[!UICONTROL シャープ 2]**  — バイキュービック法オプションよりも少しシャープな結果が得られますが、Image Server の CPU コストはさらに大きくなります。

* **[!UICONTROL トリリニア法]**  — 高い解像度と低い解像度の両方を使用します（使用可能な場合）。エイリアスが問題の場合にのみ推奨されます。 この方法では、周波数の高いデータが削減されるため JPEG のサイズが小さくなります。

* **[!UICONTROL アンシャープマスク]**  — シャープを微調整するには、次のオプションを選択します。

* **[!UICONTROL 金額]**  — 端のピクセルに適用されるコントラストを制御します。 初期設定値は 1.0 です。高解像度画像では、この値を 5.0 まで高めることができます。適用量は、フィルタ強度の度合いと考えることができます。

* **[!UICONTROL 半径]**  — シャープに影響するエッジピクセルの周囲のピクセル数を決定します。 高解像度画像では、1 ～ 2 の値を入力します。小さい値を指定すると端のピクセルのみがシャープになります。大きい値を指定すると幅広い領域のピクセルがシャープになります。適切な値は、画像のサイズに依存します。

* **[!UICONTROL しきい値]**  — アンシャープマスクフィルターを適用した場合に無視するコントラストの範囲を決定します。 つまり、このオプションは、端のピクセルとしてみなされてシャープが適用される前に、シャープを適用したピクセルが周囲の領域とどの程度異なるようになるべきかを指定します。ノイズの発生を防止するためにも、0.02 ～ 0.2 の範囲で試してください。初期設定値である 6 では、画像内のすべてのピクセルにシャープが適用されます。

* **[!UICONTROL カラースペース]**  — イメージが作成されたスペース ( 通常はRGB（オリジナル）) と輝度スペース（強度）のどちらを使用するかを指定します。

* **[!UICONTROL カラー]** 次のオプションを選択します。

* **[!UICONTROL 出力カラープロファイル]**  — 選択 **[!UICONTROL デフォルトを使用]** またはAdobe Dynamic Media Classicで使用できる ICC カラープロファイルの 1 つ。

   詳しくは、[ICC プロファイル](icc-profiles.md#icc_profiles)も参照してください。

* **[!UICONTROL レンダリングインテント]**  — カラープロファイルのデフォルトのレンダリング方法を上書きする場合は、オプションを選択します。 デフォルトの ICC プロファイルの 1 つがカラー変換のターゲットカラースペースの場合に、このオプションを使用します。 または、出力デバイス（プリンターまたはモニター）は、このプロファイルによって特徴付けられ、指定されたレンダリングインテントは、このプロファイルに対して有効です。

* **[!UICONTROL 埋め込みプロファイル]**  — この画像をAdobe® Photoshop®で開いた場合に、このプロファイルが使用されるようにするには、このオプションを選択します。

* **[!UICONTROL 印刷解像度]**  — この画像を印刷する解像度を選択します。デフォルトは 72 ピクセルです。

* **[!UICONTROL URL 修飾子]**  — 設定ではなく、画像プリセットを定義する URL 修飾子を指定する場合は、ここに修飾子を入力します。

* **[!UICONTROL サンプル画像 URL]** - Dynamic Media Image Server が、追加または編集しようとしている画像プリセットで画像を配信する際に使用する「生の」URL 文字列をリストします。 この URL 文字列は、プリセットを追加画面またはプリセットを編集画面で選択したすべての形式設定をエンコードします。

### 画像プリセットの編集、削除、非アクティブ化 {#editing-removing-or-deactivating-an-image-preset}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**.
1. 画像プリセット画面の表でプリセットを選択し、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL 編集]** 次に、プリセットを編集ダイアログボックスで新しいオプションを指定します。
   * 選択 **[!UICONTROL 削除]** をクリックして、リストからプリセットを削除します。
   * 選択を解除する **[!UICONTROL アクティブ]** プリセット名の横にあるチェックボックスをオンにします。

## アダプティブビデオプリセットのアクティベートとアクティベート解除 {#activating-or-deactivating-adaptive-video-presets}

Adobe Dynamic Media Classicはアダプティブビデオエンコーディングプリセットを提供します。 これは 16:9 アダプティブビデオプリセットと 4:3 アダプティブビデオプリセットの両方を組み合わせて 1 つのグループにした、プリセットのマスターリストです。これらの定義済みプリセットは、最も一般的なエンコーディング設定を反映しており、ターゲットとなっている携帯端末、タブレットおよびデスクトップでの再生用に最適化されています。

初期設定では、「アダプティブビデオ」エンコーディングプリセットのみがアクティブ化（有効化、つまり「オン」に）されます。必要に応じて、このプリセットを非アクティブ化することができます。非アクティブなアダプティブビデオプリセットは、アップロードオプションを設定ダイアログボックスの「eVideo」セクションに選択可能なオプションとして表示されません。

詳しくは、 [ビデオのアップロードとエンコード](uploading-encoding-videos.md#uploading_and_encoding_videos).

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

**アダプティブビデオプリセットをアクティブ化または非アクティブ化するには:**

1. Adobe Dynamic Media Classicの右上隅近くにある、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビデオプリセット]** > **[!UICONTROL アダプティブビデオプリセット]**.
1. アダプティブビデオプリセットページで、プリセット名の横にあるチェックボックスを選択解除して、アップロードオプションを設定ダイアログボックスの「eVideo オプション」リストからプリセットを削除します。
1. 選択 **[!UICONTROL 閉じる]**.

## ビデオファイルのエンコーディング用のビデオプリセット {#video-presets-for-encoding-video-files}

エンコーディングプリセットを選択するには、アップロードページの右下隅で、 **[!UICONTROL ジョブオプション]**. アップロードオプションを設定ダイアログボックスで、「eVideo オプション」を展開し、必要なビデオエンコーディングプリセットを選択します。

>[!NOTE]
>
>「アダプティブビデオ」を除き、アップロードオプションを設定ダイアログボックスには、他のすべてのアダプティブビデオまたは単一のビデオエンコーディングプリセットは表示されません。 Adobe Dynamic Media Classicの管理者は、アップロードオプションを設定ダイアログボックスに表示するビデオエンコーディングプリセットを決定します。

* 次のアダプティブビデオエンコーディングプリセットまたは単一のエンコーディングプリセットから選択します。

   * **[!UICONTROL 16:9 アダプティブビデオ]**  — デスクトップ、モバイル (iPhone、iPad、Android™)、タブレット (iPad、Android™) に配信する 16:9 の縦横比のビデオを、ビューアの接続速度に最適な解像度とビットレートで作成します。

   * **[!UICONTROL 4:3 アダプティブビデオ]**  — デスクトップ、モバイル (iPhone、iPad、Android™)、タブレット (iPad、Android™) への配信用に、ビューアの接続速度に最適な解像度とビットレートで、4:3 の縦横比のビデオを作成します。

   * **[!UICONTROL アダプティブビデオ]**  — あらゆる縦横比で機能し、モバイル、タブレットおよびデスクトップに配信するビデオを作成する単一のエンコーディングプリセット。 このプリセットを使用してエンコードされたアップロード済みのソースビデオには、固定の高さが設定されますが、幅はビデオの縦横比を維持するように自動的に拡大縮小されます。

      この柔軟な「自動拡大縮小」は、独自のカスタムビデオエンコーディングプリセットを作成した場合にも初期設定で利用できます。

      詳しくは、 [ビデオエンコーディングプリセットの追加または編集](uploading-encoding-videos.md#adding_or_editing_a_video_encoding_preset).

   * **[!UICONTROL アダプティブビデオエンコーディング（16:9 または 4:3）]**  — デスクトップ、モバイル (iPhone、iPad、Android™) およびタブレット (iPad、Android™) に配信するための 16:9 および 4:3 の縦横比のビデオを作成します。 ビューアの接続速度に最も適した解像度とビットレートで最適化されたすべての要素。

      詳しくは、[アダプティブビデオエンコーディング（16:9 または 4:3）ビデオプリセット](application-setup.md#adaptive_video_encoding_16_9_or_4_3_video_presets)を参照してください。

   * **[!UICONTROL シングルエンコーディングプリセット]**

      >[!NOTE]
      >
      >ビデオを iPad に配信するには、モバイルエンコーディングプリセットまたはタブレットエンコーディングプリセットを選択します。 タブレットプリセットは特に iPad 用に設計され、一般に大きな画面サイズや接続の帯域幅の利点を活かせる高い解像度と品質を備えています。タブレットプリセットでエンコードされたビデオファイルを配信するには、モバイルサイトやアプリケーションでデバイス検出コードが必要です。このコードは、再生デバイスに応じて iPhone または iPad ビデオ表示を切り替えます。iPad へのビデオファイルの配信用のモバイルプリセットを選択する方がワークフローは簡単です。その理由は、iPhone と iPad の両方で同じビデオファイルを使用できるためです。ただし、画質は低い解像度の iPhone での表示用に標準化されます。

      * 「エンコーディングプリセット」グループの「エンコーディングプリセットを並べ替え」ドロップダウンリストで、「名前」または「サイズ」を選択して、名前または解像度サイズでプリセットを並べ替えます。
      * ビデオの再生に使用する解像度サイズと帯域幅に基づいて、エンコーディングプリセットを選択します。
      * 「アダプティブビデオエンコーディング」を選択し、ビデオごとに 1 つ以上のエンコーディングプリセットを選択できます。 例えば、1 つのアップロードジョブでデスクトップとモバイルの両方のファイルをエンコードできます。

次を選択した後： **[!UICONTROL アップロードを開始]**&#x200B;に設定すると、元のマスタービデオファイルがアップロードされ、マスターファイルからエンコードされたファイルが生成されます。

### エンコーディングプリセットオプションについて {#about-encoding-preset-options}

エンコーディングプリセットオプションのパラメータは次のとおりです。

* **[!UICONTROL ターゲット接続速度]**  — ターゲットエンドユーザーのインターネット接続速度。

* **[!UICONTROL エンコードされたファイルサフィックス]**  — 識別のためにエンコードされたビデオファイルに添付されるサフィックス。

* **[!UICONTROL ビデオビットレート（データレート）]**  — ビデオ再生の 1 秒を構成するエンコードされたデータの量（キロビット/秒）。

* **[!UICONTROL ピクセルの幅/高さ]**  — 画面画像の幅の寸法（ピクセル単位）。画面画像の高さの寸法（ピクセル単位）。

* **[!UICONTROL 1 秒あたりのフレーム数 (fps)]**  — ビデオの 1 秒あたりのフレーム数（静止画）。 米国および日本では、ほとんどのビデオが 29.97 fps で撮影され、ヨーロッパとアジア（日本を除く）では、ほとんどのビデオが 25 fps で撮影されます。映画は 24 fps で撮影されます。

* **[!UICONTROL オーディオビットレート]**  — オーディオ再生の 1 秒を構成するエンコードされたデータの量（キロビット/秒）。

以降に示す表に、ビデオプリセットを選択するためのベストプラクティスと、エンコードされたファイルを指定するために使用する命名規則を示します。

### アダプティブビデオ（初期設定） {#adaptive-video-default}

モバイル、タブレットおよびデスクトップに配信するビデオを作成するための、すべての縦横比で機能するエンコーディングプリセットです。このプリセット（初期設定でありベストプラクティスでもあるプリセット）を使用してエンコードされたアップロード済みのソースビデオには、固定の高さが設定されますが、幅はビデオの縦横比を維持するように自動的に拡大縮小されます。

**アダプティブビデオ（初期設定）**

|  | エンコーディングプリセット名／ツールヒントテキスト | エンコードファイルのサフィックス | ビデオのデータレート（Kbps） | 幅/高さ（ピクセル） | fps | オーディオビットレート（kbps） | 推奨 |
|--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 自動 x360、800 Kbps | _Mobile_Autox360p_800K | 800 | Autox360 | ソースと同じ | 64 | モバイル (iPhone、iPad、Android™) の場合 |
| 2 | 自動 x 480、1400 Kbps | _Tablet_Autox480p_1400K | 1400 | Autox480 | ソースと同じ | 96 | タブレット (iPad、Android™) の場合 |
| 3 | 自動 x 720、2600 Kbps | _Desktop_Autox720p_2600K | 2600 | Autox720 | ソースと同じ | 128 | デスクトップの場合 |

### アダプティブビデオエンコーディング（16:9 または 4:3）ビデオプリセット {#adaptive-video-encoding-or-video-presets}

次のアダプティブビデオエンコーディングプリセットは、アップロードしたビデオの縦横比に基づき自動的に選択された一連のエンコードプリセットを組み合わせたものです。例えば、4:3 のビデオをアップロードした場合、このビデオは&#x200B;**「アダプティブビデオエンコーディング (16:9 または 4:3)」**&#x200B;オプションのマスタープリセットリスト内にある 5 つの 4:3 プリセットをすべて使用し、自動的にエンコードされます。

エンコーディングオプションパラメーターについては、[エンコーディングプリセットオプションについて](application-setup.md#about_encoding_preset_options)を参照してください。

**アダプティブビデオエンコーディング（16:9 または 4:3）プリセット**

|  | エンコードプリセット名/ツールヒントテキスト | ターゲット接続速度（Kbps） | エンコードファイルのサフィックス | ビデオのデータレート（Kbps） | 幅/高さ（ピクセル） | fps | オーディオビットレート（kbps） | 推奨 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | ソースと同じ | 64 | 低解像度、3G |
| 2 | `4:3, 384x288px, Mobile (iPhone, iPad, Android™), (400 Kbps)` | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | ソースと同じ | 64 | 低解像度、3G |
| 3 | `16:9, 512x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | ソースと同じ | 64 | 中解像度、3G |
| 4 | `4:3, 384x288, Mobile (iPhone, iPad, Android™), (600 Kbps)` | 700 | _Mobile_384x288_600 | 600 | 384 x 288 | ソースと同じ | 64 | 中解像度、3G |
| 5 | `16:9, 640x360, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x360_800K | 800 | 640 x 360 | ソースと同じ | 80 | 中解像度、WiFi |
| 6 | `4:3, 640x480, Tablet (iPad, Android™), (800 Kbps)` | 900 | _iPad_640x480_800K | 800 | 640 x 480 | ソースと同じ | 80 | 中解像度、WiFi |
| 7 | `16:9, 768x432, Tablet (iPad, Android™), (1200 Kbps)` | 1.5 Mbps | _iPad_768x432_1200K | 1200 | 768 x 432 | ソースと同じ | 96 | 高解像度、WiFi |
| 8 | `4:3, 768x576, Tablet (iPad, Android™), (1200 Kbps)` | 1.5 Mbps | _iPad_768x576_1200K | 1200 | 768 x 576 | ソースと同じ | 96 | 高解像度、WiFi |
| 9 | `16:9, 1280x720, Desktop, (2000 Kbps)` | 3.0 Mbps | _1280x720_2000K | 2000 | 1280 x 720 | ソースと同じ | 128 | 高精細、ワイドスクリーン |
| 10 | `4:3, 1280x960, Desktop, (2000 Kbps)` | 3.0 Mbps | _1280x960_2000K | 2000 Kbps | 1280 x 960 | ソースと同じ | 128 | 高精細 |

### デスクトップビデオエンコーディングプリセット {#desktop-video-encoding-presets}

デスクトップコンピュータでの MP4 および OGV 対応のビデオエンコーディングプリセット

エンコードオプションパラメータについては、[エンコーディングプリセットオプションについて](application-setup.md#about_encoding_preset_options)を参照してください。

**H264 Main 3.2 - オーディオ AAC、MP4 ファイル拡張子**

|  | エンコードプリセット名/ツールヒントテキスト | ターゲット接続速度（Kbps） | エンコードファイルのサフィックス | ビデオのデータレート（Kbps） | 幅/高さ（ピクセル） | fps | オーディオビットレート（Kbps） | 推奨 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270（400 Kbps） | 500 | _480x270_400K | 400 | 480 x 270 | ソースと同じ | 64 | 低解像度のワイドスクリーン |
| 2 | 16:9、640x360（800 Kbps） | 900 | _640x360_800K | 800 | 640 x 360 | ソースと同じ | 80 | 中解像度のワイドスクリーン |
| 3 | 16:9、800x450（1200 Kbps） | 1.5 Mbps | _800x450_1200K | 1200 | 800 x 450 | ソースと同じ | 96 | 中～高解像度 |
| 4 | 16:9、1280x720（2000 Kbps） | 3.0 Mbps | _1280x720_2000K | 2000 年 | 1280 x 720 | ソースと同じ | 128 | 高精細、ワイドスクリーン |
| 5 | 4:3、320x240（400 Kbps） | 500 | _320x240_400K | 400 | 320 x 240 | ソースと同じ | 64 | 低解像度 |
| 6 | 4:3、480x360（800 Kbps） | 900 | _480x360_800K | 800 | 480 x 360 | ソースと同じ | 80 | 中解像度 |
| 7 | 4:3、640x480（1200 Kbps） | 1.5 Mbps | _640x480_1200K | 1200 | 640 x 480 | ソースと同じ | 96 | 中～高解像度 |
| 8 | 4:3、1280x960（2000 Kbps） | 3.0 Mbps | _1280x960_2000K | 2000 年 | 1280 x 960 | ソースと同じ | 128 | 高精細 |

**OGG Theora Vorbis - OGV ファイル拡張子**

|  | エンコードプリセット名/ツールヒントテキスト | ターゲット接続速度（Kbps） | エンコードファイルのサフィックス | ビデオのデータレート（Kbps） | 幅/高さ（ピクセル） | fps | オーディオビットレート（Kbps） | 推奨 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、480x270（400 Kbps）、OGG | 500 | _OGG_480x270_400K | 400 | 480 x 270 | ソースと同じ | 64 | 低解像度のワイドスクリーン |
| 2 | 16:9、640x360（800 Kbps）、OGG | 900 | _OGG_640x360_800K | 800 | 640 x 360 | ソースと同じ | 80 | 中解像度のワイドスクリーン |
| 3 | 16:9、800x450（1200 Kbps）、OGG | 1.5 Mbps | _OGG_800x450_1200K | 1200 | 800 x 450 | ソースと同じ | 96 | 中～高解像度 |
| 4 | 16:9、1280x720（2000 Kbps）、OGG | 3.0 Mbps | _OGG_1280x720_2000K | 2000 年 | 1280 x 720 | ソースと同じ | 128 | 高精細、ワイドスクリーン |
| 5 | 4:3、320x240（400 Kbps）、OGG | 500 | _OGG_320X240_400K | 400 | 320 x 240 | ソースと同じ | 64 | 低解像度 |
| 6 | 4:3、480x360（800 Kbps）、OGG | 900 | _OGG_480x360_800K | 800 | 480 x 360 | ソースと同じ | 80 | 中解像度 |
| 7 | 4:3、640x480（1200 Kbps）、OGG | 1.5 Mbps | _OGG_640x480_1200K | 1200 | 640 x 480 | ソースと同じ | 96 | 中～高解像度 |
| 8 | 4:3、1280x960（2000 Kbps）、OGG | 3.0 Mbps | _OGG_1280x960_2000K | 2000 年 | 1280 x 960 | ソースと同じ | 128 | 高精細 |

### モバイルビデオエンコーディングプリセット {#mobile-video-encoding-presets}

ソース fps と同じで、iPhone、iPad、Android™の各モバイルデバイス用のビデオエンコーディングプリセットです。

エンコードオプションパラメータについては、[エンコーディングプリセットオプションについて](application-setup.md#about_encoding_preset_options)を参照してください。

**H264 ベースライン 2.1 - オーディオ AAC、MP4 ファイル拡張子**

|  | エンコードプリセット名/ツールヒントテキスト | ターゲット接続速度（Kbps） | エンコードファイルのサフィックス | ビデオのビットレート（Kbps） | 幅/高さ（ピクセル） | fps | オーディオビットレート（Kbps） | 推奨 |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| 1 | 16:9、512x288、モバイル（400 Kbps） | 500 | _Mobile_512x288_400K | 400 | 512 x 288 | ソースと同じ | 64 | 低解像度、3G |
| 2 | 16:9、512x288、モバイル（600 Kbps） | 700 | _Mobile_512x288_600K | 600 | 512 x 288 | ソースと同じ | 64 | 中解像度、3G |
| 3 | 16:9、512x288、モバイル（800 Kbps） | 900 | _Mobile_512x288_800K | 800 | 512 x 288 | ソースと同じ | 80 | 中解像度、Wi-Fi |
| 4 | 16:9、512x288、モバイル（1000 Kbps） | 1.2 Mbps | _Mobile_512x288_1000K | 1000 | 512 x 288 | ソースと同じ | 80 | 高解像度、Wi-Fi |
| 5 | 16:9、512x288、モバイル（1200 Kbps） | 1.5 Mbps | _Mobile_512x288_1200K | 1200 | 512 x 288 | ソースと同じ | 96 | 高解像度、Wi-Fi |
| 6 | 4:3、384x288、モバイル（400 Kbps） | 500 | _Mobile_384x288_400K | 400 | 384 x 288 | ソースと同じ | 64 | 低解像度、3G |
| 7 | 4:3、384x288、モバイル（600 Kbps） | 700 | _Mobile_384x288_600K | 600 | 384 x 288 | ソースと同じ | 64 | 中解像度、3G |
| 8 | 4:3、448x336、モバイル（800 Kbps） | 900 | _Mobile_448x336_800K | 800 | 448x336 | ソースと同じ | 80 | 中解像度、Wi-Fi |
| 9 | 4:3、448x336、モバイル（1000 Kbps） | 1.2 Mbps | _Mobile_448x336_1000K | 1000 | 448x336 | ソースと同じ | 80 | 高解像度、Wi-Fi |
| 10 | 4:3、448x336、モバイル（1200 Kbps） | 1.5 Mbps | _Mobile_448x336_1200K | 1200 | 448x336 | ソースと同じ | 96 | 高解像度、Wi-Fi |

## ビューアプリセット {#viewer-presets}

>[!NOTE]
>
>**Flash視聴者向けの提供終了通知** - 2017 年 1 月 31 日、Adobe Dynamic Media ClassicはFlashビューアプラットフォームのサポートを正式に終了しました。

*ビューアプリセット*&#x200B;は、ユーザのコンピュータ画面および携帯端末上でリッチメディアアセットがどのように表示されるかを決定する設定です。管理者は、ビューアプリセットを作成できます。一連のビューア構成オプション用の設定があります。例えば、ビューアの表示サイズ、ズーム動作、カラースキーム、境界線およびフォントを変更できます。

ベストプラクティスとしては、Adobe Dynamic Media ClassicHTML5 ビデオビューアを使用します。 HTML5 ビデオビューアで使用されるプリセットは堅牢なビデオプレーヤーです。

を組み合わせて 1 つのプレーヤーにすると、次の操作が可能になります。

* HTML5 と CSS を使用して再生コンポーネントを設計する機能。
* 埋め込み再生がある。
* ブラウザーの機能に応じて、アダプティブストリーミングとプログレッシブストリーミングを使用します。

リッチメディアコンテンツのリーチをデスクトップ、タブレット、モバイルのユーザーに拡張し、ビデオエクスペリエンスを合理化します。

詳しくは、 [HTML5 ビューアについて](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only) (Adobeビューアリファレンスガイド )

詳しくは、 [Adobe Dynamic Media Classicビューアプリセットの互換性マトリックス](application-setup.md#scene7_viewer_preset_compatibility_matrix).

詳しくは、[ベストプラクティス：HTML5 ビデオビューアの使用](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer)を参照してください。

ビューアによっては、コミュニティ機能を追加できます。コミュニティ機能には、埋め込みボタン、電子メールボタン、リンクボタンおよびアクセスボタンがあります。これらのボタンを使用すると、閲覧者を使用するユーザーは、他のユーザーとビューアを共有したり、Adobe Dynamic Media Classic Web サイトを開いたりできます。

関連トピック [Adobeビューアリファレンスライブラリの例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

### レスポンシブデザインの Web ページ用ビューアのサポート {#viewer-support-for-responsive-designed-web-pages}

Web ページごとに異なるニーズがあります。別のブラウザウィンドウでHTML5 ビューアを開くリンクを提供する Web ページが必要な場合もあります。 ホスティングページに直接HTML5 ビューアを埋め込む必要がある場合もあります。 後者の場合、Web ページは静的レイアウトである可能性が高くなります。 また、「レスポンシブ」で、デバイスごと、またはブラウザーウィンドウのサイズごとに表示方法が変わります。 これらのニーズに対応するため、Adobe Dynamic Media Classicに付属のHTML5 ビューアでは、静的 Web ページとレスポンシブデザイン Web ページの両方をサポートしています。

レスポンシブビューアを Web ページに埋め込む方法について詳しくは、 [レスポンシブ画像ライブラリについて](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/c-about-responsive-static-image-library.html#image-serving-api), [レスポンシブ画像ライブラリの使用](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#image-serving-api)、および [コマンドリファレンス — コマンド属性](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/responsive-static-image-library/t-using-responsive-static-image-library.html#responsive-static-image-library).

### ビューアプリセットのタイプ {#viewer-preset-types}

管理者は、次のタイプのビューアプリセットを作成およびカスタマイズできます。

* **[!UICONTROL eCatalog ビューア]**  — 印刷したカタログを読む体験をシミュレートします。 ページ間の移動、ページ上の項目のズームイン/ズームアウト、画像マップを使用してページ上の項目に関する詳細を表示、またはカタログを検索することができます。 詳細情報を表示する情報パネルを含めたり、また画像マップ領域に有効な rollover_key 属性がある場合は画像マップ項目を含めたりすることもできます。情報パネルを含めるには、eCatalog ビューアプリセットウィンドウの情報パネルの設定パネルで、情報サーバの URL を指定します。

* **[!UICONTROL スウォッチセットビューア]**  — イメージを異なる色、マテリアル、テクスチャ、仕上げ、またはファブリックで表示します。 ユーザーがサムネールを選択して、画像のバリエーションを表示します。

* **[!UICONTROL 混在メディアセットビューア]** - 1 つのビューアで異なる種類のメディアを表示します。 スウォッチセット、スピンセット、画像およびビデオを含めることができます。異なるタイプのコンテンツを含むタブ、例えば、画像セットのタブとビデオのタブを設定できます。混在メディアセットで再生するビデオには、タイムラインとビデオコントロール（停止、一時停止、巻き戻し、再生など）がある標準のビデオビューアが使用されます。混在メディアセットビューアのプリセットを設定するときに、混在メディアセット内の各アセットタイプに使用するビューアを指定します。グリッドビューアまたはカルーセルビューアを使用して混在メディアセットを表示することもできます。

* **[!UICONTROL スピンセットビューア]**  — 複数の画像ビューを提供し、ユーザーがオブジェクトを回転させて、様々な面や角度を確認できるようにします。

* **ビデオビューア**  — ソースファイルの解像度のサイズまたはカスタムサイズを使用してビデオを表示します。 Adobe Dynamic Media Classicには、ビデオ再生用の定義済みのビューアプリセットが多数用意されています。管理者は、カスタムのビデオビューアプリセットを作成できます。 ビデオビューア設定のための 10 種類以上の設定が用意されています。サイズ、前景色と背景色、ビデオおよびオーディオコントロール、プログレスバー、ユーザーインターフェイススキン、ソーシャル機能、ヘルプ機能を設定できます。

* **[!UICONTROL ズームビューア]**  — 次の 3 種類のズームビューアを選択できます。

* **[!UICONTROL ズームビューア]** ：ユーザーが領域を選択してズームインできます。 画像を初期設定のサイズに戻す、ズームイン、ズームアウトの各コントロールを選択できます。

* **[!UICONTROL ズームビューア：フライアウト]**  — ズームされた領域の 2 つ目の画像を元の画像の横に表示します。 使用できるコントロールはなく、ユーザは表示する範囲の選択だけが可能です。

このビューアの完全な帯域幅使用量を決定する場合、メイン画像とフライアウト画像の両方がビューアに提供されます。メイン画像のサイズ（ステージの幅と高さ）とズーム率によって、フライアウト画像のサイズが決まります。フライアウト画像のサイズを大きくなり過ぎないようにするには、メイン画像のサイズとズーム率の値のバランスを保ってください。大きいサイズのメイン画像を使用する場合は、ズーム率の値を小さくします（フライアウト幅とフライアウト高さは、フライアウトウィンドウのサイズを決定しますが、ビューアに供給されるフライアウト画像のサイズは決定しません）。

例えば、350 x 350 pixel、ズーム率 3 のメイン画像の場合、表示されるフライアウト画像は 1050 x 1050 pixel になります。300 x 300 pixel、ズーム率 4 のメイン画像の場合、表示されるフライアウト画像は 1200 x 1200 pixel になります。JPEG の画質設定（推奨される設定は 80 ～ 90 です）に応じて、ファイルのサイズを大幅に小さくすることができます。メイン画像のサイズによりますが、推奨されるズーム率は 2.5 ～ 4 です。

### Adobe Dynamic Media Classicビューアプリセットの互換性マトリックス {#scene-viewer-preset-compatibility-matrix}

**Flash視聴者向けの提供終了通知**:2017 年 1 月 31 日、Adobe Dynamic Media ClassicはFlashビューアプラットフォームのサポートを正式に終了しました。

次の表に、現在使用可能なAdobe Dynamic Media Classicビューアプリセットを示します。 この表には、ビューアのデスクトップまたは携帯端末との互換性と、各ビューアで使用されるテクノロジも示されます。

関連トピック [Adobeビューアリファレンスライブラリの例](https://landing.adobe.com/en/na/dynamic-media/ctir-2755/live-demos.html).

ビューアでサポートされる Web ブラウザーとオペレーティングシステムのバージョンについて詳しくは、ビューアのリリースノートに記載されています。

詳しくは、 [Adobeビューアリファレンスリリースノート](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

|  | ビューアテクノロジ | デスクトップ | Apple iPhone | Apple iPad | Android™スマートフォン | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| ズームビューア |  |  |  |  |  |  |
| Universal_HTML5_Flyout | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_inline | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_Zoom_light | HTML5 | X | X | X | X | X |


|  | ビューアテクノロジ | デスクトップ | Apple iPhone | Apple iPad | Android™スマートフォン | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| イメージセットビューア |  |  |  |  |  |  |
| Universal_HTML5_フライアウト | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

|  | ビューアテクノロジ | デスクトップ | Apple iPhone | Apple iPad | Android™スマートフォン | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| スウォッチセットビューア |  |  |  |  |  |  |
| Universal_HTML5_フライアウト | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SwatchSet_light | HTML5 | X | X | X | X | X |

|  | ビューアテクノロジ | デスクトップ | Apple iPhone | Apple iPad | Android™スマートフォン | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| eCatalog ビューア |  |  |  |  |  |  |
| Universal_media5_eCatalog_Adv( ソーシャルHTMLとカタログ検索のサポートを含む ) | HTML5 | X | X | X | X | X |
| Universal_HTML5_eCatalog（ソーシャルメディアおよびカタログ検索のサポートを含む） | HTML5 | X | X | X | X | X |

|  | ビューアテクノロジ | デスクトップ | Apple iPhone | Apple iPad | Android™スマートフォン | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| スピンビューア |  |  |  |  |  |  |
| Universal_HTML5_SpinSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_SpinSet_light | HTML5 | X | X | X | X | X |

**eVideo ビューア**

Adobe Dynamic Media Classicは、MP4 H.264 ビデオのモバイルビデオ再生をサポートしています。

* このビデオ形式をサポートする BlackBerry®デバイスは、次の場所で見つけることができます。 [BlackBerry®でサポートされるビデオ形式](https://developer.blackberry.com/devzone/develop/supported_media/bb10_media_support.html)
* また、このビデオ形式をサポートする Windows®デバイスは、次の場所でも見つけることができます。 [Windows® Phone でサポートされるビデオ形式](https://docs.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)

|  | ビューアテクノロジ | デスクトップ | Apple iPhone | Apple iPad | Android™スマートフォン | Android™ Tablet | BlackBerry®スマートフォン | Windows® Phone |
|--- |--- |--- |--- |--- |--- |--- |--- |--- |
| Universal_HTML5_Video（クローズドキャプションのサポートを含む） 詳しくは、 [ベストプラクティス：ユニバーサルHTML5 ビデオビューアの使用](best-practice-using-html5-video.md#best_practice_using_the_html5_video_viewer) | HTML5 | X | X | X | X | X | X | X |
| Universal_HTML5_Video_social（クローズドキャプションおよびソーシャルメディアのサポートを含む） | HTML5 | X | X | X | X | X | X | X |

|  | ビューアテクノロジ | デスクトップ | Apple iPhone | Apple iPad | Android™スマートフォン | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| 混在メディアセットビューア |  |  |  |  |  |  |
| Universal_HTML5_MixedMedia_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_MixedMedia_light | HTML5 | X | X | X | X | X |

### サポートされているモバイルビューアのジェスチャに関する表 {#supported-mobile-viewers-gestures-matrix}

次の表に、iOS、Android™ 2.x および Android™ 3.x デバイスでサポートされているモバイルビューアのジェスチャーを示します。

|  | ビューアテクノロジ | デスクトップ | Apple iPhone | Apple iPad | Android™スマートフォン | Android™ Tablet |
|--- |--- |--- |--- |--- |--- |--- |
| イメージセットビューア |  |  |  |  |  |  |
| Universal_HTML5_フライアウト | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_dark | HTML5 | X | X | X | X | X |
| Universal_HTML5_ImageSet_light | HTML5 | X | X | X | X | X |

### ビューアプリセット画面について {#about-the-viewer-preset-screen}

ビューアプリセット画面で、ビューアプリセットを作成して管理します。この画面を開くには、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.

ビューアプリセット画面には、次のタスクを実行するためのツールがあります。

* **プリセットを追加**  — 選択 **[!UICONTROL 追加]** ビューアプリセットを追加ダイアログボックスで選択を行います。

       [ ビューアプリセットの追加と編集 ](application-setup.md#adding_and_editing_viewer_presets) を参照してください。
   
* **プリセットの編集**  — プリセットを選択し、「 **[!UICONTROL 編集]**.

       [ ビューアプリセットの追加と編集 ](application-setup.md#adding_and_editing_viewer_presets) を参照してください。
   
* **プリセットの削除**  — プリセットを選択し、「 **[!UICONTROL 削除]**.

* **プリセットの書き出し** -HTML5 のビューアプリセットを選択し、「 」を選択します。 **[!UICONTROL 書き出し]** をクリックして、別のビューアプリセットを作成および追加する際の基礎として使用できるように、ビューアスキンをダウンロードします。

       詳しくは、「HTML5 ビューアプリセットの書き出し」(application-setup.md#exporting_an_html5_viewer_preset) を参照してください。
   
* **ビューアプリセットリストのフィルタリング**  — 次のツールを使用してリストをフィルタリングします。

       *「**アクティブ/非アクティブ**」ドロップダウンリストを開き、アクティブなプリセット、非アクティブなプリセットまたはすべてのプリセットを表示するオプションを選択します。
       * 「**ビューア**」ドロップダウンリストを開き、特定の種類のビューアのみを表示するオプションを選択します。 選択**[!UICONTROL すべてのビューア]**をクリックして、すべてのビューアを表示します。
   
* **プリセットを並べ替え**  — 列見出し (**[!UICONTROL アクティブ]**, **[!UICONTROL タイプ]**, **[!UICONTROL プリセット]**&#x200B;または **[!UICONTROL Platform]**) をクリックして、列のリストを並べ替えます。 列見出しをもう一度選択すると、リストが降順（または昇順）に並べ替えられます。

* **プリセットのアクティベートとアクティベート解除**  — プリセットを選択し、「アクティブ」オプションを選択して、アクティブ化または非アクティブ化します。

       詳しくは、[ ビューアプリセットのアクティベートとアクティベート解除 ](application-setup.md#activating_or_deactivating_viewer_presets) を参照してください。
   
>[!NOTE]
>
>選択 **[!UICONTROL プレビュー]** ビューアプリセットページの右側で、選択したビューアプリセットでアセットがどのように表示されるかを確認できます。 別のアセットを表示するには、「 **[!UICONTROL 参照]** ビューアプリセットページで、アセットプレビューを選択ダイアログボックスで別のアセットを選択します。

### ビューアプリセットの追加と編集 {#adding-and-editing-viewer-presets}

を使用してビューアプリセットを追加する以外に、 **[!UICONTROL 追加]** ユーザーインターフェイスで、 **[!UICONTROL 書き出し]** をクリックして、ビューアプリセットを追加します。 既存のHTML5 ビューアプリセットを書き出し、それを新しいプリセットの基礎として使用します。

詳しくは、 [HTML5 のビューアプリセットの書き出し](application-setup.md#exporting_an_html5_viewer_preset).

関連トピック [ビューアプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

**ビューアプリセットを追加および編集するには:**

1. Adobe Dynamic Media Classicの右上隅近くにある、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.

   プリセットのリストをフィルタリングすることができます。例えば、ビデオビューアのプリセットのみを表示するには、表の真上にある「ビューア」ドロップダウンメニューから「ビデオビューア」を選択します。

1. ビューアプリセットページで、ビューアプリセット画面でビューアプリセットを追加または編集します。

   * **追加**  — ツールバーで、「 」を選択します。 **[!UICONTROL 追加]**. ビューアプリセットを追加ダイアログボックスで、プラットフォームを選択し、リッチメディアアセットタイプを選択します。

          選択**[!UICONTROL 名前を付けて保存]**」をクリックします。
      
   * **既存のビューアプリセットから開始して追加**  — 表で、ビデオビューアプリセットを選択し、「 **[!UICONTROL 編集]** をクリックします。

          ビデオビューアを再設定したら、「**」を選択します[!UICONTROL 名前を付けて保存]**をクリックして、「プリセット名」テキストフィールドに別の名前を入力してプリセットを保存します。
      
   * **編集**  — 既存のビューアプリセットを選択し、「 」を選択します **[!UICONTROL 編集]**.

1. ビューアを設定画面の「プリセット名」フィールドに、プリセット名を入力または編集します。
1. 必要に応じてその他のオプションを設定します。

   >[!NOTE]
   >
   >選択 **[!UICONTROL ソースと同じ]** を指定すると、エンコードされたビデオ自体の解像度サイズに合わせてビデオビューアのサイズが自動的に調整されます。 このオプションを選択した場合、「ステージの幅」と「ステージの高さ」を入力することはできません。 その代わり、これらのオプションはビデオ自体から取得されます。次を選択した場合、 **[!UICONTROL ソースと同じ]**&#x200B;で、「マージンサイズ」オプションを設定して、ビデオ再生領域の外側にあるスキンのサイズを反映します。 このマージンサイズは、ビデオコントロールのピクセル単位の高さと幅です。次の画像を使用して、使用する余白のサイズを決定できます。*

   ![ビデオビューアの余白の設定](assets/vs_video_viewer_configure_margin.png)

1. 次のいずれかの操作を行います。

   * 選択 **[!UICONTROL 名前を付けて保存]** 既存のプリセットから開始してビューアプリセットを追加した場合。
   * 選択 **[!UICONTROL 保存]** （ビューアプリセットを追加または編集した場合）

### HTML5 のビューアプリセットの書き出し {#exporting-an-html-viewer-preset}

既存のHTML5 ビューアプリセットを書き出して、HTML5 ビューアプリセットを作成する際の基礎として使用できます。 この書き出しオプションが便利なのは、ビューアプリセットをゼロから作成する必要がなくなる点にあります。代わりに、外観や動作が希望に近いプリセットを書き出すことで、それをデザインを調整するための出発点として使用できます。

Adobe Dynamic Media Classic内のすべてのデフォルトの標準提供ビューアプリセット CSS ファイルは、上のアセットを指す相対的な画像サービングパスを使用します。 `Scene7SharedAssets`. 例えば、以下は、ビューアプリセット CSS ファイル内の画像アセットの相対パス (

`Scene7SharedAsset`: `.s7videoviewer .s7fullscreenbutton[state][selected] { background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }`

ただし、自社のサイトでビューア CSS ファイルをホストする場合は、自社の環境で Image Server への明示的なパスを使用して、これらの相対画像パスを解決する必要があります。 例えば、上の相対パスを明示的なパスに更新する場合、次のようになります。 `https://s7d1.scene7.com` は、image server への直接パスです。 `https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha`

**HTML5 ビューアプリセットを書き出すには：**

```as3
.s7videoviewer .s7fullscreenbutton[state][selected] 
{ background-image: url(/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha); }
```

```as3
https://s7d1.scene7.com/is/image/Scene7SharedAssets/FullScreenButton_dark_sprite?scl=1&fmt=png-alpha
```

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.
1. ビューアプリセットツールバーの左側にある 2 番目のドロップダウンリストで、 **[!UICONTROL HTML5]**.
1. 左から 3 番目のドロップダウンリストで「**[!UICONTROL すべてのビューア]**」を選択します。
1. 新しいビューアプリセット「5 ビューアプリセット」の基礎として使用するHTMLプリセットを選択します。
1. ツールバーで、「 **[!UICONTROL 書き出し]**.
1. 選択したアセットを書き出しダイアログボックスで、 **[!UICONTROL 書き出しを送信]**.

   書き出し後、CSS ファイルを取得します。 そのファイルをダウンロードして展開します。

1. CSS ファイルを CSS エディタで開き、変更を行い、ファイルを保存します。
1. CSS ファイルをAdobe Dynamic Media Classicにアップロードします。

   詳しくは、 [ファイルをアップロード](uploading-files.md#uploading_files).

1. CSS ファイルをDynamic Media Image Server に公開します。

   詳しくは、 [ファイルを公開](publishing-files.md#publishing_files).

1. 新しいビューアプリセットを通常どおりに追加します。アップロードしたビューア CSS ファイルを選択します。

   詳しくは、 [ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets).

### ビューアプリセットをアクティベートまたはアクティベート解除 {#activating-or-deactivating-viewer-presets}

アセットを表示するための URL を作成するには、プレビューダイアログボックスの「プリセット」ドロップダウンリストを開き、ビューアプリセットを選択して、「 **[!UICONTROL URL をコピー]** ( [ビューアプリセットの URL をコピー](application-setup.md#copying_the_url_of_a_viewer_preset)) をクリックします。 このプリセットリストには、管理者がビューアプリセット画面で追加して管理するビューアプリセットが表示されます。例えば、ユーザが eCatalog をプレビューすると、すべてのアクティブな eCatalog ビューアプリセットがプレビューダイアログボックスの「プリセット」ドロップダウンリストに表示されます。

ビューアプリセット画面でビューアプリセットを非アクティブ化しないと、プレビューダイアログボックスの「プリセット」ドロップダウンリストの件数が増加します。

**ビューアプリセットをアクティブ化または非アクティブ化するには:**

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.
1. ビューアプリセットページで、を選択または選択解除します **[!UICONTROL アクティブ]** ビューアプリセットをアクティブ化または非アクティブ化するオプション

### ビューアプリセットの URL をコピー {#copying-the-url-of-a-viewer-preset}

アセットを公開した後に、ビューアプリセットの設定でアセットを表示するための URL をコピーすることができます。

URL がクリップボードにコピーされます。Web ページ、携帯端末またはアプリケーションの HTML コードで必要に応じてこの URL を使用することができます。

**ビューアプリセットの URL をコピーするには:**

1. 参照パネルからアセットを選択します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL と埋め込みコードパネルで、 **[!UICONTROL URL をコピー]** を選択します。
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

   ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
   ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
   ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL URL をコピー]**.

### ビューアプリセットの埋め込みコードをコピーする {#copying-the-embed-code-of-a-viewer-preset}

埋め込みコード機能を使用すると、選択したビューアプリセットのビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。

埋め込みコードダイアログボックスでは、コードの編集はできません。

**ビューアプリセットの埋め込みコードをコピーするには:**

1. アセットの参照パネルでアセットを選択します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側の URL パネルで、「 」を選択します。 **[!UICONTROL 埋め込みコード]**.
   * 選択 **[!UICONTROL グリッド表示]**. アセットの参照パネルで、1 つのアセットを選択し、サムネール画像の下の **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.

   ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL リスト表示]**. アセットの参照パネルで 1 つのアセットを選択し、サムネール画像の右側にあるに移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
   ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

   * 選択 **[!UICONTROL グリッド表示]**, **[!UICONTROL リスト表示]**&#x200B;または **[!UICONTROL 詳細ビュー]**. 同じツールバーで、に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**.
   ビューアリストページの表の「アクション」列で、を選択します。 **[!UICONTROL 埋め込みコード]**.

1. 埋め込みコードダイアログボックスで、「 **[!UICONTROL クリップボードにコピー]**.
1. 選択 **[!UICONTROL 閉じる]**.

## 初期設定のビューアの設定 {#configuring-default-viewers}

デフォルトビューアを使用して、Adobe Dynamic Media Classicでプレビューを使用する際にアセットに関連付けられるデフォルトのビューアを設定できます。 次のアセットタイプの初期設定のプレビュー環境を設定できます。

* 画像
* ビデオ
* スピンセット
* カタログ
* 画像セット
* スウォッチセット
* メディアセット

**初期設定ビューアを設定するには:**

1. 「設定」ドロップダウンリストで、「 **[!UICONTROL アプリケーション設定]**.
1. [ 設定 ] ウィンドウの左側のペインで、に移動します。 **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビューア]**
1. 選択 **[!UICONTROL 初期設定のビューア]**.
1. 初期設定ビューアウィンドウの各アセットタイプのドロップダウンリストで、アセットのプレビューに関連付けるビューアを選択します。
1. 初期設定ビューアウィンドウの右下隅で、 **[!UICONTROL 設定を保存]**.
1. Setup ウィンドウの右下隅で、 **[!UICONTROL 閉じる]** をクリックして、Asset ウィンドウに戻ります。

## メタデータビュー {#metadata-views}

*メタデータ*&#x200B;はアセットに関する標準化された情報です。メタデータを使用して、ワークフローを合理化し、アセットを整理し、検索を向上できます。Adobe Dynamic Media Classicは、IPTC(International Press Telecommunications Council) 標準とXMP(extensible metadata platform) 標準をサポートしています。 詳細ビューでアセットのメタデータを表示したり入力したりする前に、メタデータビューメニューを開くことができます。 そこから、表示またはアセットの説明に使用する一連のメタデータフィールドを選択できます。

Adobe Dynamic Media Classicには事前定義済みのメタデータビューが用意されており、管理者は独自のメタデータビューを作成して、ユーザーがメタデータの入力時に選択できるようにすることができます。

### メタデータビューの作成 {#creating-a-metadata-view}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL メタデータ]** > **[!UICONTROL メタデータビュー]**.
1. 選択 **[!UICONTROL 追加]**.
1. 「プリセット名」テキストフィールドに、ビューの名前を入力します。
1. （オプション）チェック **[!UICONTROL デフォルトにする]** を使用して、ユーザが詳細ビューでメタデータパネルを開いたときに表示されるビューを作成します。
1. （オプション）「 」を選択します。 **[!UICONTROL UDF を含める]** をクリックして、ビューにユーザ定義フィールドを含めます。 ユーザ定義フィールドは、詳細ビューのメタデータパネルの上部に表示されます。
1. ビューに必要なフィールドを選択します ( **[!UICONTROL すべてを選択]** をクリックして、すべてのフィールドを選択します )。
1. 選択 **[!UICONTROL 保存]**.

   ビュー用に選択したカテゴリとフィールドがプレビューパネルに表示されます。

### メタデータビューの管理 {#managing-metadata-views}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL メタデータ]** > **[!UICONTROL メタデータビュー]**.
1. 次のいずれかの操作を行います。

   * ビューをプレビューするには、ビューを選択します。ビューのフィールドがプレビューパネルに表示されます。
   * ビューを編集するには、ビューを選択し、 **[!UICONTROL 編集]**. 次に、プレビューパネルでフィールド名を選択または選択解除し、 **[!UICONTROL UDF を含める]** オプション。
   * ビューを削除するには、ビューを選択し、 **[!UICONTROL 削除]**.
   * ビューをデフォルトにするには、ビューを選択し、 **[!UICONTROL デフォルトにする]**. デフォルトのビューは、ユーザーがアセットを詳細ビューで開き、メタデータパネルに移動したときに表示されるビューです。

## メタデータプリセット {#metadata-presets}

メタデータプリセットにより、管理者はアセットに割り当てられたメタデータを制御したり管理したりできます。詳細ビューでは、ユーザーはアセットに関するメタデータを、その目的で提供されるフィールドに入力できます。 例えば、ユーザは所有者名、著作権情報、アドレスを入力できます。ユーザーがこの情報を正確かつ完全に入力するように、メタデータプリセットを作成できます。 詳細ビューでメタデータプリセットを選択すると、メタデータフィールドに事前定義済みの値が入力されます。 例えば、所有者名、著作権情報、アドレスが自動的に入力されます。

アセットを説明するためにユーザーが詳細ビューに自動的に入力できるメタデータ値のセットごとに、メタデータプリセットを作成します。

### メタデータプリセットの作成または編集 {#creating-or-editing-a-metadata-preset}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL メタデータ]** > **[!UICONTROL メタデータプリセット]**.
1. メタデータプリセット画面で、次のいずれかの操作を実行します。

   * プリセットを作成するには、「 **[!UICONTROL 追加]**. 「メタデータテンプレート名」テキストフィールドに、プリセットの名前を入力します。 選択 **[!UICONTROL メタデータビュー]**&#x200B;を選択し、ドロップダウンリストからビューを選択します ( [メタデータビュー](application-setup.md#metadata_views)) をクリックします。
   * 既存のプリセットを編集するには、メタデータプリセットリストからプリセットを選択し、「 」を選択します **[!UICONTROL 編集]**.

1. プリセットに含める見出しを展開し、プリセットに含めるフィールドに値を入力します。
1. 選択 **[!UICONTROL 保存]**.

   プリセット用に選択したカテゴリとフィールドがプレビューパネルに表示されます。

### メタデータプリセットの管理 {#managing-metadata-presets}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL メタデータ]** > **[!UICONTROL メタデータプリセット]**.
1. 次のいずれかの操作を行います。

   * プリセットをプレビューするには、プレビューするプリセットを選択します。プリセット情報（カテゴリとフィールド）がプレビュー画面に表示されます。
   * プリセットを削除するには、プリセットを選択し、「 」を選択します **[!UICONTROL 削除]**.

## ユーザ定義フィールド {#user-defined-fields}

Media Portal 管理者または会社管理者が、ユーザ定義のカスタムメタデータフィールドを作成できます。カスタムフィールドは、Adobe Dynamic Media Classicのアセットの整理に役立ちます。 必要に応じて、フィールドを「アクティブ」としてマークできます。 有効にすると、これらのカスタムメタデータフィールドの名前が詳細ビューのメタデータパネルに表示されます。 ユーザは、ユーザ定義メタデータフィールドに情報を入力して、アセットの説明を追加することができます。また、ユーザ定義メタデータフィールドを検索条件にすることもできます。

ユーザ定義メタデータフィールドの効果的な使用方法の 1 つとして、特定の発売（販売）でアセットのアクティブ化の時間を遅らせることができます。タイプに基づいて、「アクティベーション」フィールドを定義します *日付*. 次に、 **[!UICONTROL メタデータ]** 詳細ビューのパネルまたは **[!UICONTROL ファイル]** > **[!UICONTROL 情報を編集]**&#x200B;に設定すると、アセットをアクティベートするタイミングを指定できます。 Adobe Dynamic Media Classicは、アセットの公開ステータスと公開履歴を確認します。 アクティベーション時間内でない場合、公開ステータスは「未公開」と表示されます。

>[!NOTE]
>
>詳細ビューのメタデータパネルにユーザ定義のフィールドを表示するには、メタデータビューにユーザ定義のフィールドを含めます。 メタデータビュー画面で、「UDF を含める」オプションを選択します。詳しくは、[メタデータビュー](application-setup.md#metadata_views)を参照してください。

>[!NOTE]
>
>ユーザー定義のカスタムフィールドを使用してアセットを検索するには、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**&#x200B;を選択し、 **[!UICONTROL 検索に UDF を含める]**. 詳しくは、[個人設定](personal-setup.md#personal_setup)を参照してください。

### ユーザ定義のメタデータフィールドの作成 {#creating-a-user-defined-metadata-field}

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL メタデータ]** > **[!UICONTROL ユーザ定義フィールド]**.
1. 選択 **[!UICONTROL 追加]**
1. カスタムフィールドダイアログボックスで、目的のオプションを設定します。

   * **[!UICONTROL 名前]**  — メタデータフィールドの名前を入力します。

   * **[!UICONTROL タイプ]**  — ユーザーがメタデータフィールドに入力できる情報のタイプを定義するオプションを選択します。

   * **[!UICONTROL 文字列]**  — テキスト文字列。

   * **[!UICONTROL 整数]**  — 整数。

   * **[!UICONTROL 浮動小数]**  — 浮動小数点数。

   * **[!UICONTROL はい/いいえ]**  — はい/いいえのブール値。

   * **[!UICONTROL 日付]**  — 日付。 MM/DD/YYYY 形式で指定できます。

   * **[!UICONTROL ファイル名]**  — ファイルの名前。

   * **[!UICONTROL カラー]**  — 色の名前。

   * **[!UICONTROL Dimension]**  — アセットの幅と高さ。

   * **[!UICONTROL 型指定なし]**  — 後方互換性のため。 このオプションを選択してはいけません。

   * **[!UICONTROL デフォルト値]**  — オプションで、ユーザーが「 」フィールドに入力する可能性が最も高い値を入力します。 入力した値が、作成したフィールドの初期設定値になります。

   * **[!UICONTROL 適用先]**  — 特定のタイプのアセットにのみメタデータフィールドを適用する場合は、必要に応じてアセットタイプを選択します。

      >[!NOTE]
      >
      >を選択します。 **[!UICONTROL 適用先]** オプションは慎重に行ってください。 **[!UICONTROL 適用先]** 」オプションを使用して、ユーザー定義フィールドを作成する必要があります。 Adobe Dynamic Media Classicでは、ユーザー定義フィールドの名前、タイプおよびデフォルト値を編集できますが、 **[!UICONTROL 適用先]** 設定。*

1. 選択 **[!UICONTROL 保存]** メタデータフィールドの作成が完了したら、次の手順に従います。

### ユーザ定義フィールドの管理 {#manage-user-defined-fields}

ユーザ定義フィールド画面には、ユーザ定義のカスタムメタデータフィールドを管理するためのコマンドが用意されています。

Media Portal 管理者または会社管理者のみが、ユーザ定義フィールドを管理できます。

この画面を開くには、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL メタデータ]** > **[!UICONTROL ユーザ定義フィールド]**.

* **フィールドの編集**  — フィールドを選択し、「 **[!UICONTROL 編集]**.

* **フィールドの削除**  — フィールドを選択し、「 **[!UICONTROL 削除]**.

* **フィールドを有効化** - **[!UICONTROL アクティブ]** オプションをクリックします。 会社管理の役割を持っている場合、このオプションは表示されません。 このオプションは MediaPortal に関連しているので、個人設定で「 MediaPortal 機能を表示」を選択（オン）して、アクティベートされたフィールドを表示する必要があります。

## ファイルの最適化 {#optimize-files}

ファイルをAdobe Dynamic Media Classicにアップロードすると、ファイルがストレージと公開用に最適化されます。 ただし、アップロード処理を中断した場合は、一部の画像が最適化されません。この場合は、「画像がまだ最適化されていません」というメッセージが表示されます。これらのファイルは、管理者が最適化できます。

Adobe Dynamic Media Classicは、ファイルを検索し、以前に完全に最適化されていなかった画像のみを最適化します。

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]**&#x200B;を選択し、 **[!UICONTROL ファイルの最適化]**.
1. 最適化ジョブの情報を入力し、を選択します。 **[!UICONTROL 送信]**.

   複数の会社で作業をしている場合は、異なる会社のファイルは別個に最適化します。

## バッチセットプリセット {#batch-set-presets}

バッチセットプリセットを使用して、Adobe Dynamic Media Classicにアセットをアップロードするジョブの実行中に、画像セットまたはスピンセットを自動的に作成します。

会社の管理者は、まず、セット内でグループ化するアセットの命名規則を定義します。 次に、これらの画像を参照するバッチセットプリセットを作成できます。 各プリセットは、プリセット手法で定義された命名規則に一致する画像を使用してセットの構成方法を定義する、固有の名前を持ち自己完結した命令のセットです。

会社のアクティブなバッチセットプリセットはすべて、アップロードオプションを設定ダイアログボックスに表示されるので、各アップロードセッション中に適用するプリセットを指定できます。会社の管理者は、すべてのアクティブおよび非アクティブなバッチセットプリセットを確認できます。ファイルをアップロードすると、Adobe Dynamic Media Classicは、アクティブなプリセットで定義された命名規則に一致するすべてのファイルを含むセットを自動的に作成します。

### 初期設定の名前 {#default-naming}

会社の管理者は、バッチセットプリセット手法で使用する初期設定の命名規則を作成します。バッチセットプリセット定義で選択されたデフォルトの命名規則は、すべての Web サイトのセットをバッチ生成するために会社で必要なものです。 バッチセットプリセットは、定義する初期設定の命名規則を使用するために作成されます。会社が定義する初期設定の命名規則の例外の場合のために、固有のコンテンツのセットに必要な代替のカスタム命名規則を含むバッチセットプリセットを多数作成することができます。

バッチセットプリセット機能を使用する場合は、デフォルトの命名規則を設定する必要はありません。 ただし、Adobeのベストプラクティスでは、命名規則の要素を 1 つのセットにグループ化する数だけ定義する場合は、デフォルトの命名規則を使用することをお勧めします。 これにより、バッチセット作成を合理化できます。

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL バッチセットプリセット]** > **[!UICONTROL デフォルトの名前]**.
1. 「**[!UICONTROL フォームを表示]**」または「**[!UICONTROL コードを表示]**」を選択し、各要素に関する情報の表示と入力の方法を指定します。

   次の項目を選択できます。 **[!UICONTROL コードを表示]** チェックボックスをオンにして、選択した形式と同時に作成される正規表現値を表示します。 フォーム表示により制限を受ける場合、命名規則の要素を定義するために正規表現値を入力または変更できます。フォームビューで値を解析できない場合、フォームフィールドは非アクティブになります。

   >[!NOTE]
   >
   >非アクティブな形式フィールドは、無効な正規表現を表示しません。正規表現の正誤に関する検証は行われません。「結果」行で各要素に作成する正規表現の結果を確認することができます。完全な正規表現は、ページの一番下に表示されます。

1. 必要に応じて各要素を展開し、使用する命名規則を入力します。
1. 必要に応じて、「 」を選択します。 **[!UICONTROL 追加]** 別の命名規則を要素に追加する場合。 または、 **[!UICONTROL 削除]** 要素の命名規則を削除する場合。
1. 選択 **[!UICONTROL 名前を付けて保存]** プリセットの名前を入力します。 または、 **[!UICONTROL 保存]** （既存のプリセットを編集している場合）

または、形式フィールドを利用しないで、「コードを表示」を使用することもできます。このビューでは、正規表現を完全に使用して命名規則の定義を作成します。

定義には、一致とベース名という 2 つの要素を使用できます。これらのフィールドでは、命名規則のすべての要素を定義して、要素が含まれるセットを命名するために使用される規則の一部を指定できます。会社の個々の命名規則では、これらの要素ごとに 1 行以上の定義を使用できます。 固有の定義を必要なだけ使用して、メイン画像、カラー要素、代替表示要素およびスウォッチ要素などの個別の要素にグループ化することができます。

### バッチセットプリセットの作成 {#creating-a-batch-set-preset}

Adobe Dynamic Media Classicはバッチセットプリセットを使用して、一部の共通の情報やコンテンツを共有するアセットを、ビューアに表示する画像のセットに整理します。 バッチセットプリセットレシピは、Adobe Dynamic Media Classicでスケジュールしたアセット読み込みジョブと同時に、自動的に実行されます。

バッチセットプリセットを使用して、バッチセットプリセットを作成、編集および管理します。必要なすべてのアセット取り込みジョブをカバーするために、必要な数のプリセットを作成できます。 バッチセットプリセット定義には次の 2 つの形式があります。設定したデフォルトの命名規則用のものと、その場で作成するカスタムの命名規則用のものです。

フォームフィールドメソッドを使用してバッチセットプリセットを定義するか、コードメソッドを使用して正規表現を使用できます。 例： **[!UICONTROL デフォルトの名前]**&#x200B;を選択すると、 **[!UICONTROL コードビュー]** 同時に、フォームビューでを定義し、正規表現を使用して定義を作成します。 また、いずれかの表示をオフにして、一方の表示のみを使用することもできます。

関連トピック [2D スピンセットを自動生成するためのバッチセットプリセットの作成](application-setup.md#creating_a_batch_set_preset_for_the_auto_generation_of_a_2d_spin_set).

関連トピック [2D スピンセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/537_2d-spin_converted%20renamed_Done-AVS) トレーニングビデオ。

**バッチセットプリセットを作成するには:**

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL バッチセットプリセット]** > **[!UICONTROL バッチセットプリセット]**. 詳細ページの右上隅に設定されている&#x200B;**[!UICONTROL 「フォームを表示」]**&#x200B;は初期設定の表示です。
1. プリセットリストパネルで、「 **[!UICONTROL 追加]** をクリックして、ページの右側にある詳細パネルで定義フィールドをアクティブにします。
1. 詳細パネルの「プリセット名」フィールドにプリセットの名前を入力します。
1. 「バッチセットの種類」ドロップダウンメニューで、プリセットの種類を選択します。

   2D スピンセットを自動生成するには、「バッチセットの種類」ドロップダウンリストで「**[!UICONTROL 多軸スピンセット]**」を選択します。

1. 次のいずれかの操作を行います。

   * 以前に **[!UICONTROL アプリケーション設定]** > **[!UICONTROL バッチセットプリセット]** > **[!UICONTROL デフォルトの名前]**、展開 **[!UICONTROL アセットの命名規則]**&#x200B;を選択し、「ファイル名」ドロップダウンリストで、 **[!UICONTROL デフォルト]**.
   * プリセット設定時に命名規則を定義するには、を展開します。 **[!UICONTROL アセットの命名規則]**&#x200B;を選択し、「ファイル名」ドロップダウンリストで、 **[!UICONTROL カスタム]**.

1. 「シーケンスの順序」では、セットがAdobe Dynamic Media Classicでグループ化された後の画像の順序を定義します。 初期設定では、アセットはアルファベット順に並んでいます。ただし、カンマ区切りの正規表現リストを使用して順番を定義できます。
1. 命名規則と作成オプションの設定では、アセットの命名規則で定義したベース名にサフィックスとプリフィックスを指定します。また、Adobe Dynamic Media Classicのフォルダー構造内で画像セットを作成する場所も定義します。

   多数の画像セットを定義する場合は、これらのセットを、アセット自体を含むフォルダーとは別に保持します。 多くの顧客は、画像セットフォルダを作成し、生成されたバッチセットを配置するためにアプリケーションをリダイレクトしています。

1. 選択 **[!UICONTROL 保存]** をクリックします。

### 2D スピンセットを自動生成するためのバッチセットプリセットの作成 {#creating-a-batch-set-preset-for-the-auto-generation-of-a-d-spin-set}

「バッチセットの種類」の「**多軸スピンセット**」を使用して、2D スピンセットの生成を自動化する「手法」を作成できます。画像のグループ化では行と列の正規表現を使用するので、画像アセットが多次元の配列の対応する場所に正しく配置されます。

関連トピック [バッチセットプリセットの作成](application-setup.md#creating_a_batch_set_preset).

多軸スピンセットの行数または列数には、上限または下限はありません。

例として、*spin-2dspin* という名前の多軸スピンセットを作成します。1 行あたり 12 個の画像が含まれる 3 行のスピンセット画像セットがあります。画像の名前は次のとおりです。

```as3
spin-01-01
spin-01-02
… 
spin-01-12
spin-02-01
… 
spin-03-12
```

この情報を使用して、バッチセットの種類のレシピを次のように作成できます。

![レシピ画像をバッチ設定](assets/se_batch_set_recipe.png)

スピンセット内のアセット名で共有されている部分のグループ化は、（ハイライト表示されているように）「一致」フィールドに追加されます。 行と列を含むアセット名の可変部分は、それぞれ「行」フィールドと「列」フィールドに追加しています。

このスピンセットをアップロードして公開する際に、アップロードオプションを設定ダイアログボックスの&#x200B;**[!UICONTROL バッチセットプリセット]**&#x200B;の下に表示される 2D スピンセット手法の名前をアクティブ化します。

**2D スピンセットを自動生成するためのバッチセットプリセットを作成するには:**

1. に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL バッチセットプリセット]** > **[!UICONTROL バッチセットプリセット]**. 詳細ページの右上隅に設定されている&#x200B;**[!UICONTROL 「フォームを表示」]**&#x200B;は初期設定の表示です。
1. プリセットリストパネルで、「 **[!UICONTROL 追加]** をクリックして、ページの右側にある詳細パネルで定義フィールドをアクティブにします。
1. 詳細パネルの「プリセット名」フィールドにプリセットの名前を入力します。
1. 「バッチセットの種類」ドロップダウンメニューで、「**[!UICONTROL アセットセット]**」を選択します。
1. 「サブタイプ」ドロップダウンリストで、「**[!UICONTROL 多軸スピンセット]**」を選択します。
1. 展開 **[!UICONTROL アセットの命名規則]**&#x200B;を選択し、「ファイル名」ドロップダウンリストで、 **[!UICONTROL カスタム]**.
1. 「**[!UICONTROL 一致]**」およびオプションとして「**[!UICONTROL ベース名]**」の属性を使用して、グループを構成する画像アセットの命名に使用する正規表現を定義します。

   リテラルの Match 正規表現の例を次に示します。

   `(\w+)-\w+-\w+`

1. **[!UICONTROL 「行と列の位置」]**&#x200B;を展開し、2D スピンセット配列内の画像アセットの位置の名前形式を定義します。

   ファイル名内での行または列の位置は丸括弧で囲みます。

   例えば、行の正規表現の場合、次のようになります。

   `\w+-R([0-9]+)-\w+`

   または

   `\w+-(\d+)-\w+`

   列の正規表現の例を次に示します。

   `\w+-\w+-C([0-9]+)`

   または

   `\w+-\w+-C(\d+)`

   これらの式は例に過ぎません。 必要に応じて独自の正規表現を作成できます。

   >[!NOTE]
   >
   >行と列の正規表現の組み合わせで、多次元スピンセット配列内のアセットの位置を判断できない場合、そのアセットはセットに追加されず、エラーが記録されます。

1. 命名規則と作成オプションの設定では、アセットの命名規則で定義したベース名にサフィックスとプリフィックスを指定します。また、Adobe Dynamic Media Classicのフォルダー構造内で画像セットを作成する場所も定義します。

   多数の画像セットを定義する場合は、これらのセットを、アセット自体を含むフォルダーとは別に保持します。 多くの顧客は、画像セットフォルダを作成し、生成されたバッチセットを配置するためにアプリケーションをリダイレクトしています。

1. 選択 **[!UICONTROL 保存]** をクリックします。
1. スピンセットを通常通りにアップロードして公開します。「バッチセットプリセット」の「ジョブの読み込みオプション」ダイアログボックスで 2D スピンセットの名前がアクティブ化されていることを確認します。

>[!MORELIKETHIS]
>
>* [アセットのプレビュー](previewing-asset.md#previewing_an_asset)
>* [画像プリセットの設定](setting-image-presets.md#setting_up_image_presets)
>* [メタデータの表示、追加、書き出し](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
>* [ジョブファイルを確認](checking-job-files.md#checking_job_files)

