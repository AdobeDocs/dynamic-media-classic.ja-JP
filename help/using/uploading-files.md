---
title: ファイルのアップロード
description: Adobe Dynamic Media Classicにファイルをアップロードする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 8dfcfb3f-6472-4efd-bc87-d5111eee45ce
topic: Content Management
level: Intermediate
source-git-commit: 1cd516119da23f5ef4c0195273025ddd4b3fa789
workflow-type: tm+mt
source-wordcount: '3858'
ht-degree: 25%

---

# ファイルのアップロード{#uploading-files}

アセットファイルをAdobe Dynamic Media Classicにアップロードする前に、アセットファイルの名前が正しいことを確認してください。 また、フォルダー構造が思いどおりに設定および整理されていることを確認します。 Adobe Dynamic Media Classicが提供する FTP サイトから、またはコンピューターやネットワークから直接ファイルをアップロードできます。 Adobe Dynamic Media Classicには、アップロード時にファイルを最適化するためのオプションが用意されています。 Adobe Dynamic Media Classic デスクトップアプリケーションをインストールした場合は、ファイルやフォルダーをデスクトップから直接ドラッグしてアップロードできます。 詳しくは、[アプリケーションの全般設定](application-setup.md#general_settings)を参照してください。

## アップロード用のアセットとフォルダーの準備 {#preparing-your-assets-and-folders-for-uploading}

Adobe Dynamic Media Classicにアセットをアップロードする前に、適切な形式とサイズであることを確認してください。 また、アセットの命名に関するAdobe Dynamic Media Classicのルールを遵守する必要があります。 フォルダ構成とファイル構造を設定しておくと、ファイルの操作や場所の特定が容易になります。

### サポートされているアセットファイル形式 {#supported-asset-file-formats}

次の表に、Adobe Dynamic Media Classicがサポートするアセットファイル形式を示します。 サポートされるCamera Raw ファイルについては、[https://helpx.adobe.com/jp/camera-raw/using/supported-cameras.html](https://helpx.adobe.com/jp/camera-raw/using/supported-cameras.html) を参照してください。

| アセットファイル形式 | 説明 |
| --- | --- |
| オーディオ | AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 |
| カスケードスタイルシート | CSS |
| カラープロファイル | ICC、ICM |
| フォント | AFM、OTF、PFB、PFM、PhotoFont、TTC、TTF |
| FXG | FXG |
| Illustrator | AI、FXG |
| 画像 | BMP、FPX、GIF、JPEG、JPG、PNG、PICT （Windows® のみ）、TIF、TIFF |
| InDesign | INDD、INDT |
| MS® Office | DOC、PPT、RTF、XLS |
| PDF | PDF |
| Photoshop | PSD、FXG、Camera Raw |
| PostScript | EPS、PS |
| Adobe Dynamic Media Classic画像のオーサリング | VNC、VNT、VNW |
| SVG | SVG、SVGX |
| TAR | TAR |
| ビデオ | 3GP、AVI、M2P、M2T、M2TS、M2V、M4V、MOV、MP4、MPEG、MPG、MTS、OGV、TS、VOB、WMV/ASF |
| XML | XML |
| ZIP | ZIP |

TAR および ZIP のアップロードサポートには、ファイルを解凍するかどうかを選択するチェックボックスがあります。

### Dynamic Media でサポートされていない画像形式 {#unsupported-image-formats-dynamic-media}

以下のリストは、Dynamic Media でサポートされていない *サポートされていない* ラスタライズ画像ファイル形式のサブタイプに関する説明です。

* IDAT チャンクサイズが 100 MB を超える PNG ファイル。
* PSB ファイル。
* カラースペースが CMYK、RGB、グレースケールまたはビットマップ以外のPSD ファイルはサポートされていません。 DuoTone、Lab、および Indexed カラースペースはサポートされていません。
* ビット数が 16 を超えるPSD ファイル。
* 浮動小数点データを持つTIFF ファイル。
* Lab カラースペースを持つTIFF ファイル。

### アセットタイプ {#asset-types}

Adobe Dynamic Media Classic プログラムで最適な結果を得るには、必ず推奨されるファイル形式とサイズを使用してください。 次の表に、アセットタイプを示します。アセットタイプによっては、よく使用されるアセットについて、推奨の形式とファイルサイズを示しているものもあります。

| アセットタイプ | 説明／推奨 |
| --- | --- |
| オーディオ | 入力オーディオアセット形式には AAC、HE-AAC、AC3、WAV、WMA、AIFF、MP3 があります。オーディオは MP3、AAC および HE-AAC 形式にトランスコードできます。 |
| 画像（画像のサイズ変更、ズーム、画像セット、スピンセットの場合） | 画像は最長サイズで 2,000 ピクセル以上にする必要があります。一般的な画像サイズは最長サイズで 1500 ～ 2,500 ピクセルの範囲です。 推奨の形式は、TIFF ファイルや PNG ファイルのような可逆圧縮の画像形式です。JPEG 画像にする場合は、画質を最高に設定してください。GIF ファイルのアニメーションは、他の静的コンテンツと同様に処理されます。 |
| eCatalog | Adobe Acrobatで作成された高解像度のPDF ファイル、または「プレス対応」として保存されたAdobe Creative Suite アプリケーションを使用します。 PDF には、必要なすべてのフォント、画像、マスクが含まれます。 また、必要な参照グラフィック要素をすべて、単一ページ、見開きページ、複数ページ形式のいずれかで含めることができます。 英数字順にファイルに名前を付けて、ページが並ぶようにします。アップロードを簡単にするために、eCatalog のもとになる PDF をすべて同じフォルダに格納してください。アップロード時に切り抜きオプションを選択すると、切り抜きマーク、登録ターゲット、カラーバーのようなトリミング部分を PDF から削除することができます。製本版の PDF ファイルのカラースペースは、ほとんどの場合 CMYK になるため、PDF ファイルとともに使用する CMYK ICC カラープロファイルを取得しておくことが重要です。 |
| テンプレート | テキスト、画像、およびレイヤーを含めることができるレイヤー画像またはレイアウトデザイン。変数データをカスタマイズできるように、画像レイヤー、テキスト文字列、色やサイズなどの属性をパラメータ化することができます。テンプレートで使用する画像の要件は、ほかの画像の要件と同様です。Photoshop などの画像編集プログラムでグラフィックを作成し、それぞれのグラフィックを TIFF または PNG 形式の平滑化透過ファイルとして保存します。用途に対して画像解像度が適切であることを確認してください。印刷用の画像は 300 ppi です。 |
| ビデオ | Adobe Dynamic Media Classicは、OGV および MP4 形式で保存されたビデオファイルをサポートしています。 アップロード時にファイルを MP4 形式にトランスコードできます。 詳しくは、[サポートされているアセットファイル形式](#supported-static-file-formats)を参照してください。 |
| フォント | TrueType、`Type1` （Windows® のみ）、OpenType® フォント、PhotoFonts をアップロードしました。 |
| 画像 | 画像ファイルとレイヤー画像ファイル。 |
| 画像セットとスウォッチセット | ビューアで表示可能な関連性のある一連の画像。 |
| ICC プロファイル | アップロードした画像をそのソースカラースペースから別のカラースペースに変換するために使用できるカラープロファイル。 |
| ビネット | 画像オーサリングプログラムで作成された画像と関連ファイル。 |
| コンテンツファイル | Adobe InDesign、Illustrator または Photoshop コンテンツファイル。 |
| FXG ファイル | プリント、Web、電子メール、デスクトップおよびデバイス向けにカスタマイズ可能な出力用テンプレートを作成するのに使用する、解像度に依存しないグラフィック形式ファイル。 |
| SVG ファイル | 画像サービングサーバがレンダリングすることができるスケーラブルベクタグラフィックファイル。 |
| XML ファイル | パスと要求のクエリ部分を変更するのに使用する事前処理規則を定義するファイル。 |
| カスケードスタイルシートファイル | CSS スキンをアップロードしてHTML5 ビューアをカスタマイズする。 |
| JavaScript ファイル | JavaScript ファイルは、アカウント情報を保持するために、ビューアのインストルメンテーションに使用されます。 Adobe セキュリティでは、（クロスサイトスクリプティングを避けるために）配信に別のドメインを使用しているクライアントアカウントに対してのみ、このアセットタイプを使用することをお勧めします。 |

>[!NOTE]
>
>画像ファイルと PDF をAdobe Dynamic Media Classicにアップロードすると、これらのソースファイルが P-TIFF（Pyramid TIFF）ファイルに変換されます。 これらの P-TIFF は、後で Dynamic Media Image Server に公開されるファイルです。 Adobe Dynamic Media Classicでは、Adobe Dynamic Media Classic ズームビューアで表示する場合に高速ズームを可能にする様々なズーム比が含まれているので、Pyramid Tiff ファイル形式を使用しています。

### サポートされている静的ファイルの形式 {#supported-static-file-formats}

Adobe Dynamic Media Classicは、複数の静的ファイル形式をサポートしています。 静的コンテンツとは、CSS、PDF、SVG、XML など、「そのまま」公開されるアセットのことです。

次のファイルの種類を公開できます。

* アニメーション GIF
* オーディオファイル
* CSS
* JavaScript（会社が独自のドメインで構成されている場合）
* プライマリビデオ
* PDF（アップロード後にPDFが公開用にマークされると、既存の eCatalog/PDF ワークフローのすべての PDF が配信されるのを回避できます）
* PrX ビデオ
* SVG
* XML
* ZIP

Adobe Dynamic Media Classicには、静的なコンテンツのプレビュー URL を生成するオプションはありません。

### ファイル名の要件 {#filename-requirements}

ファイル名の拡張子はアップロード処理中にファイル名から取り除かれるため、システム上で同じルート名を持つファイルを共存させることはできません。Adobe Dynamic Media Classic システムでは、アセットのファイル名からファイル名拡張子を引いた名前が、アセットのアセット ID になります。 したがって、同じ名前のアセットは存在しません。

社内のすべてのユーザーが、ファイルの命名に関する次のルールを理解していることを確認します。

* 同じ名前のアセット ID はシステムで使用できません。
* アセット ID 名では大文字と小文字が区別されます。
* アセット ID にはスペースを含む名前（black jacket.tif や blue jacket.jpg など）を使用しないことをお勧めします。Adobe Dynamic Media Classicでは、アセット名を使用して URL 文字列を作成する際に、アセット名の空白文字を ASCII エンコードします。 このような ASCII コードは見づらいので、URL が読みづらくなります。
* 言語固有の文字はファイル名で使用できます。一方、次の文字はファイル名で使用できません。

  `\ ; / ? : @ & = + $ , &#42; " &lt; > | ' { } %`

  ファイル名に上記の文字が 1 つ以上含まれている場合、その文字はアップロード時にファイル名から削除されます。

通常、アセットのファイル名は、次に示すように、項目番号、製品 SKU またはその他の名前と同じにできます。

| 項目 | ファイル名 | アセット ID |
| --- | --- | --- |
| 896649 | 896649.jpg | 896649 |
| 48A3_2X | 48A3_2X.tif | 48A3_2X |

### フォルダの整理と構造 {#folder-organization-and-structure}

コンテンツをシステムにアップロードする前に、Adobe Dynamic Media Classicでコンテンツのフォルダーとサブフォルダーを整理し構造化します。 この作業を事前に計画しておくと、2 つの大きな利点があります。

* FTP 経由でコンテンツをAdobe Dynamic Media Classicにアップロードする場合、アップロード中にフォルダー構造をレプリケートするようにシステムに指示できます。 これにより、コンテンツは、コンピューターまたはネットワーク上と同じAdobe Dynamic Media Classic内のフォルダーとサブフォルダーに整理されます。 （フォルダー構造をAdobe Dynamic Media Classicにレプリケートするには、FTP 経由でアセットをアップロードする際に「サブフォルダーを含める」オプションをオンにします）。
* ファイルのアップロード後にシステムのフォルダ構成を変更するのは、最初からフォルダ構造を慎重に検討した場合に比べて、はるかに難しくなります。

Adobe Dynamic Media Classicにコンテンツを保存するためのフォルダーの命名アプローチと構造は、組織のニーズに応じて選択します。 フォルダ構成の例を以下に示します。

**SKU ベース**：フォルダーには、SKU または項目番号に従って名前が付けられます。 例えば、0 個、20 個、30 個のすべての数値系列に対して個別のフォルダーが作成されます。

**ブランドベース**：複数のブランドラインを持つメーカーや、他のブランドを他社に販売する小売業者の場合、ファイルを異なるブランドのという名前の製品フォルダーに分割します。

**プロジェクトベース**：フォルダーは、ロールアウト/ドロップ日またはプロジェクト名に従って整理されます。 eCatalog の作成を主に行うクライアントには、このフォルダ構成が適しています。

**Web サイトのフォルダー階層のミラー**：このフォルダー構造は、web サイトのフォルダー構造を反映しています。フォルダーの名前は、製品カテゴリなどの名前が付いています。

## ファイルのアップロードについて {#uploading-your-files}

デスクトップから個々のファイルをアップロードすることも、FTP を使用してフォルダーをアップロードすることもできます。 100 MB を超えるファイルをアップロードする場合、またはフォルダーとサブフォルダー全体をアップロードする場合は、「**FTP 経由**」タブを選択します。

Adobe Dynamic Media Classicから、アップロードジョブの開始と終了を確認し、問題が発生した場合は通知するメールメッセージが送信されます。

大きなアップロードジョブの実行中（または直後）に、一部の新しい項目に「画像がまだ最適化されていません」というメッセージが表示される場合があります。 このメッセージが表示される理由は、ファイルがまだ完全に処理されず、Adobe Dynamic Media Classicに追加されていないためです。 後でこれらのファイルを最適化することができます[ ファイルの最適化 ](application-setup.md#optimize_files) を参照してください。

### 「デスクトップから」タブを使用したファイルのアップロード {#upload-files-using-sps-desktop-application}

Adobe Dynamic Media Classic デスクトップアプリケーションでは、ファイルとフォルダーをドラッグしてアップロードできます。

1. Adobe Dynamic Media Classic Desktop アプリケーションのグローバルナビゲーションバーで「**[!UICONTROL アップロード]**」を選択します。
1. アップロード ページで、「**[!UICONTROL デスクトップから]**」タブを選択します。
1. アップロードページの左側の「**[!UICONTROL アップロードするファイルを選択]**」領域で「**[!UICONTROL 参照]**」を選択してアップロードするファイルまたはフォルダーを選択し、「**[!UICONTROL 開く]**」を選択します。
1. アップロードページの右側の選択した **フォルダーの宛先** 領域で、アップロードしたファイルまたはフォルダーを追加する宛先フォルダーに移動します。
1. （オプション）アップロードページ下部付近の「ジョブ名」テキストフィールドに、アップロードジョブの新しい名前を入力します。 または、Adobe Dynamic Media Classicで提供されるデフォルトのシステム生成名を使用してもかまいません。 アップロードジョブと公開ジョブはジョブページに記録されます。ここでジョブのステータスを確認できます。 詳しくは、[ジョブファイルの確認](checking-job-files.md#checking_job_files)を参照してください。
1. （オプション）アップロードページの下部付近にある **[!UICONTROL アップロード後に公開]** を選択して、アップロードしたアセットを自動的に公開します。
ファイルを公開すると、ファイルがライブサーバーに送信されます。その後、これらのファイルの URL を外部の Web サイトやアプリケーションで使用することができます。この同じオプションは、[ ジョブ オプション ] ダイアログ ボックスでも使用できます。
1. （オプション）アップロードするファイルで既存のファイルを同じ名前に置き換える場合は、アップロードページの下部付近で、「**[!UICONTROL 任意のフォルダーでベース名が同じファイルを上書き]** を選択します。 この同じオプションは、[ ジョブ オプション ] ダイアログ ボックスでも使用できます。
このオプションの名前は、**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 一般設定]**/**[!UICONTROL アプリケーションにアップロード]**/**[!UICONTROL 画像を上書き]** の設定に応じて異なる場合があります。
1. アップロードページの右下隅付近にある **[!UICONTROL ジョブオプション]** を選択し、必要なオプションを指定します。

   詳しくは、[ アップロードオプション](uploading-files.md#upload_options)を参照してください。

1. アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL 保存]**」を選択します。
1. アップロードページの右下隅で「**[!UICONTROL アップロードを送信]**」を選択します。
アップロードの進行状況を確認するには、グローバルナビゲーションバーの **[!UICONTROL ジョブ]** を選択します。 Adobe Dynamic Media Classicで引き続き作業できます。 いつでもジョブ ページに戻って進行中のジョブを確認できます。 進行中のアップロードジョブをキャンセルするには、期間の横にある「**[!UICONTROL キャンセル]**」を選択します。

### 「FTP を使用」タブを使用したファイルのアップロード {#upload-files-using-via-ftp}

1. 特定のリージョンに固有のAdobe Dynamic Media Classic FTP サイトにログオンします。 管理者から入手した FTP のユーザ名とパスワードを使用してください。
1. Adobe Dynamic Media Classicのグローバルナビゲーションバーで「**[!UICONTROL アップロード]**」を選択します。
1. アップロード ページで、「**[!UICONTROL FTP を使用]**」タブを選択します。
1. アップロード ページの左側の **[!UICONTROL アップロード用に FTP フォルダーを選択]** 領域で、ファイルのアップロード元となる FTP フォルダーを選択します。
1. アップロード ページの右側の **[!UICONTROL Adobe Dynamic Media フォルダーの宛先を選択]** 領域で、Adobe Dynamic Media Classicの宛先フォルダーを選択します。
1. （オプション）アップロードページ下部付近の「ジョブ名」テキストフィールドに、アップロードジョブの新しい名前を入力します。 または、Adobe Dynamic Media Classicで提供されるデフォルトのシステム生成名を使用してもかまいません。 アップロードジョブと公開ジョブはジョブページに記録されます。ここでジョブのステータスを確認できます。
詳しくは、[ジョブファイルの確認](checking-job-files.md#checking_job_files)を参照してください。
1. （オプション）アップロードページの下部付近にある **[!UICONTROL アップロード後に公開]** を選択して、アップロードしたアセットを自動的に公開します。
ファイルを公開すると、ファイルがライブサーバーに送信されます。その後、これらのファイルの URL を外部の Web サイトやアプリケーションで使用することができます。この同じオプションは、[ ジョブ オプション ] ダイアログ ボックスでも使用できます。
1. （オプション）アップロードするファイルで既存のファイルを同じ名前に置き換える場合は、アップロードページの下部付近で、「**[!UICONTROL 任意のフォルダーでベース名が同じファイルを上書き]** を選択します。 この同じオプションは、[ ジョブ オプション ] ダイアログ ボックスでも使用できます。
このオプションの名前は、**[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 一般設定]**/**[!UICONTROL アプリケーションにアップロード]**/**[!UICONTROL 画像を上書き]** の設定に応じて異なる場合があります。
1. オプション。「**[!UICONTROL FTP 経由]**」タブを選択した場合にのみ使用できます。 アップロードページの下部付近にある「**[!UICONTROL アップロード時に Zip ファイルまたは Tar ファイルを解凍]**」を選択すると、アップロードした ZIP ファイルまたは TAR ファイルからすべてのファイルを自動的に抽出できます。 この同じオプションは、[ ジョブ オプション ] ダイアログ ボックスでも使用できます。
1. アップロードページの右下隅付近にある **[!UICONTROL ジョブオプション]** を選択し、必要なオプションを指定します。

   詳しくは、[ アップロードオプション](uploading-files.md#upload_options)を参照してください。

1. アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL 保存]**」を選択します。
1. アップロードページの右下隅で「**[!UICONTROL アップロードを送信]**」を選択します。

   アップロードの進行状況を確認するには、グローバルナビゲーションバーで「**[!UICONTROL ジョブ]**」を選択します。 ジョブページにアップロードの進行状況が表示されます。Adobe Dynamic Media Classicで引き続き作業できます。 いつでもジョブ ページに戻って進行中のジョブを確認できます。

進行中のアップロードジョブをキャンセルするには、期間の横にある「**[!UICONTROL キャンセル]**」を選択します。

## アップロードジョブオプション ダイアログボックス {#upload-options}

ファイルのアップロード時に、アップロードジョブオプション ダイアログボックスで次のオプションから選択できます。

* **ジョブ**: **[!UICONTROL ジョブ]** を選択して、アップロードジョブ全体に影響を与えるオプションを選択します。

  また、一般設定の *デフォルトアップロードオプション* ダイアログボックスを使用して、ジョブをアップロードするための **[!UICONTROL デフォルト]** オプションを選択することもできます。 **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 一般設定]**/**[!UICONTROL デフォルトのアップロードオプション]** に移動し、必要なデフォルトのオプションを設定します。

   * **[!UICONTROL 条件]**：このオプションを使用できるのは、「**[!UICONTROL FTP 経由]**」タブを選択した場合のみです。
      * **[!UICONTROL 1 回限り]**:1 回実行されるアップロードジョブを指定します。 次のようなオプションがあります。
         * **[!UICONTROL 今すぐ]**:「アップロードジョブオプション」ダイアログボックスで **[!UICONTROL 保存]** を選択した直後に、アップロードジョブを実行します。次に、アップロードページで **[!UICONTROL アップロードを送信]** を選択します。
         * **[!UICONTROL 後で実行するようにスケジュール]**：アップロードジョブを実行する年、月、日および時間（15 分単位）を選択します。
      * **[!UICONTROL 繰り返し]**：毎日、毎週、または毎月実行されるアップロードジョブを指定します。 または、アップロードジョブを独自の仕様にカスタマイズします。
         * **[!UICONTROL 毎日]**：ジョブを毎日実行する時間を設定します。 ジョブを月曜日から金曜日のみに実行する場合は、「**[!UICONTROL 平日のみ]**」を選択します。
         * **[!UICONTROL 毎週]**：ジョブを実行する特定の曜日と時間を選択します。
         * **[!UICONTROL 毎月]**：ジョブを実行する月の特定の日または曜日（開始時刻も含む）を選択します。
         * **[!UICONTROL カスタム]**：アップロードまたは公開ジョブの時間間隔を独自の指定にカスタマイズします。 [ カスタムアップロードまたは公開ジョブの時間間隔の作成 ](checking-job-files.md#creating-a-custom-upload-or-publish-job-time-interval) を参照してください。

   * **[!UICONTROL アップロード後に公開]**:「**[!UICONTROL デスクトップから]**」タブまたは「**[!UICONTROL FTP 経由]**」タブのいずれかを選択した場合に使用できます。 このオプションを選択すると、アップロードしたアセットを自動的に公開できます。 ファイルを公開すると、ファイルがライブサーバーに送信されます。その後、これらのファイルの URL を外部の Web サイトやアプリケーションで使用することができます。このオプションは、アップロードページにもあります。

   * **[!UICONTROL 任意のフォルダーでベースアセット名が同じファイルを上書き]**:**[!UICONTROL FROM DESKTOP]** タブまたは **[!UICONTROL VIA FTP]** タブのいずれかを選択した場合に使用できます。 アップロードするファイルで同じ名前の既存のファイルを置き換える場合は、このオプションを選択します。このオプションは、アップロードページにもあります。このオプションの名前は、**[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 一般設定]**/**[!UICONTROL アプリケーションにアップロード]**/**[!UICONTROL 画像を上書き]** の設定に応じて異なる場合があります。

   * **[!UICONTROL アップロード時に Zip または Tar ファイルを解凍]**:「**[!UICONTROL デスクトップから]**」タブまたは「**[!UICONTROL FTP 経由]**」タブを選択した場合に使用できます。
このオプションを選択すると、アップロードした ZIP ファイルまたは TAR ファイルからすべてのファイルを自動的に抽出できます。 この同じオプションは、[ ジョブ オプション ] ダイアログ ボックスでも使用できます。

   * **[!UICONTROL サブフォルダーを含める]**:「**[!UICONTROL FTP を使用]**」タブを選択した場合にのみ使用できます。
アップロードするフォルダのサブフォルダもアップロードする場合は、このオプションを選択します。アップロードするフォルダーとそのサブフォルダーの名前はAdobe Dynamic Media Classicに自動的に登録されます。

   * **[!UICONTROL メタデータファイルを処理]**:「**[!UICONTROL FTP を使用]**」タブのいずれかを選択した場合にのみ使用できます。 タブ区切りまたは XML ファイルをアップロードしてメタデータを複数のアセットに追加する場合は、このオプションを選択します。
詳しくは、[メタデータの読み込み（FTP 経由）](viewing-adding-exporting-metadata.md#import-metadata)を参照してください。

* **切り抜きオプション**：画像からホワイトスペースのピクセルを自動的に切り抜きます。 **[!UICONTROL 切り抜き]** メニューを開き、「**[!UICONTROL 手動]**」を選択し、「上」、「右」、「下」、「左」テキストフィールドに、各辺から切り抜くピクセル数を入力します。 また、切り抜きメニューで「**[!UICONTROL トリミング]**」を選択し、以下のオプションを選択することもできます。

   * **[!UICONTROL トリミング対象]**：カラーと透明度のどちらで切り抜くかを選択します。
      * **[!UICONTROL カラー]**:「カラー」オプションを選択します。 次に、隅メニューを選択し、切り抜きたいホワイトスペースの色を最も表現している色の画像の隅を選択します。
カラーに基づくトリミング：0 を指定すると、画像の隅で選択した色と完全に一致するピクセルのみが切り抜かれます。 設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。
      * **[!UICONTROL 透明度]**: 「**[!UICONTROL 透明度]**」オプションを選択します。
透明度に基づくトリミング：切り抜くピクセルが透明な場合のみ、0 を指定してください。1 に近い数値を指定すると、透明度が高くなります。
      * **[!UICONTROL 公差]**: スライダーをドラッグして、0 ～ 1 の公差を指定します。

* **カラープロファイルオプション**:Adobe Dynamic Media Classicの動的配信に使用するために最適化されたファイルを作成する場合は、カラー変換を選択します。

   * **[!UICONTROL デフォルトのカラー保持]**：画像にカラースペース情報が含まれる場合は常にソース画像のカラーを保持します。カラー変換はありません。 今日ではほぼすべての画像に、既に適切なカラープロファイルが埋め込まれています。ただし、CMYK ソース画像に埋め込みのカラープロファイルが含まれていない場合は、sRGB（標準の赤、緑、青）カラースペースへのカラー変換が実行されます。sRGB は、web ページに画像を表示するための推奨カラースペースです。
   * **[!UICONTROL 元のカラースペースを維持]**:Adobe Dynamic Media Classicに取り込まれた時点で、カラーが変換されずに元の色を保持します。 カラープロファイルが埋め込まれていない画像の場合、画像のリクエストを処理するために必要なカラー変換は、公開設定で設定されたデフォルトのカラープロファイルを使用して行われます。 これらのカラープロファイルは、このオプションで作成されたファイル内の色と常に一致するとは限りません。 そのため、「デフォルトの色保存」オプションを使用することをお勧めします。
   * **[!UICONTROL カスタム開始]**/**[!UICONTROL 終了]**：メニューが開き、「**[!UICONTROL 変換開始]**」および「**[!UICONTROL 変換先]** カラースペースを選択できます。 この詳細オプションは、ソースファイルに埋め込まれたカラー情報よりも優先されます。送信するすべての画像のカラープロファイルデータが正しくないか不足している場合にのみ、このオプションを選択します。

* **画像編集オプション**：画像内のクリッピングマスク &lt;> を保持し、カラープロファイルを選択できます。
[ アップロード時の画像の微調整オプション ](image-editing-options-upload.md#image-editing-options-at-upload) を参照してください。

* **PostScript®のオプション**: PostScript® ファイルのラスタライズ、ファイルの切り抜き、透明背景の維持、解像度の選択、カラースペースの選択を行うことができます。
[PostScriptおよびIllustrator ファイルの操作 ](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files) を参照してください。

* **Photoshopのオプション**: Adobe® Photoshop® ファイルからのテンプレートの作成、レイヤーの管理、レイヤーの命名方法の指定、テキストの抽出、テンプレートへの画像のアンカー方法の指定を行うことができます。
詳しくは、[PSD アップロードオプション](psd-files.md#psd_upload_options)を参照してください。

* **PDFのオプション**: ファイルのラスタライズ、検索単語とリンクの抽出、eCatalog の自動生成、解像度の設定、カラースペースの選択を行うことができます。
詳しくは、[PDF アップロードオプション](pdfs.md#pdf_upload_options)を参照してください。

* **Illustratorのオプション**: Adobe Illustrator® ファイルのラスタライズ、透明背景の維持、解像度の選択、カラースペースの選択を行うことができます。
[PostScriptおよびIllustrator ファイルの操作 ](postscript-illustrator-files.md#working_with_postscript_and_illustrator_files) を参照してください。

* **EVIDEO オプション**：ビデオプリセットを選択することで、ビデオファイルをトランスコードできます。
[ ビデオエンコーディングプリセットの操作 ](uploading-encoding-videos.md#working_with_video_encoding_presets) を参照してください。

* **その他のメタデータ**：アップロードするファイルを説明するキーワードを入力します。 キーワードはカンマで区切ります。キーワードを使用すると、アセットの検索が容易になります。
[ 詳細検索の実行 ](searching-assets.md#conducting_an_advanced_search) を参照してください。
[ キーワードのアップロード ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/548_upload-keywords_converted%20renamed_Done-AVS) トレーニングビデオも参照してください。

* **バッチセットプリセット**：アップロードしたファイルから画像セット、スピンセット、スウォッチセットを作成するには、使用するプリセットの「**[!UICONTROL アクティブ]**」列を選択します。 複数のプリセットを選択できます。プリセットは、アプリケーション設定/バッチセットプリセット ページで作成できます。
詳しくは、[バッチセットプリセット](application-setup.md#batch_set_presets)を参照してください。

* **詳細**:[ 別のジョブでアップロードをフォロー ](uploading-files.md#follow-an-upload-with-another-job) を参照してください。

## アップロード後に別のジョブを実行 {#follow-an-upload-with-another-job}

FTP を使用して項目をアップロードする場合、アップロードの完了時に開始するように後続のジョブをスケジュールできます。 他のジョブの開始がスケジュールされている場合、ここでスケジュールしたジョブはキューに入れられます。

新しいジョブは、指定したアドレスに通知を送信し、その場所のコードをトリガーできるようにします。 この継続される公開ジョブの名前は、アップロードジョブと同じ名前になりますが、先頭に Pub_ が付きます。**

**別のジョブでアップロードを追跡するには：**

1. 「**[!UICONTROL アップロード]**」を選択したあと、「**[!UICONTROL FTP 使用]**」タブを選択します。
1. アップロードページの右下隅の「**[!UICONTROL ジョブオプション]**」を選択します。
1. アップロードジョブオプション ダイアログボックスで、「**[!UICONTROL 詳細]**」セクションを展開します。
1. **[!UICONTROL 別のジョブでアップロードをフォロー]** ドロップダウンリストから次のいずれかを選択します。

   * なし
   * HTTP 要求
   * 画像サービング公開
   * 画像レンダリング公開
   * ビデオ公開

1. HTTP アドレスを指定します。
1. ファイルがアップロードされた場合にのみ実行するかどうかを指定します。
1. このジョブが完了するたびに、またはファイルが公開されていた場合のみ、この要求を実行するかどうかを指定します。

   >[!NOTE]
   >
   >定期的にスケジュールされたジョブでは、ファイルが公開されないことがあります。

>[!MORELIKETHIS]
>
>* [ アセットフォルダーの操作 ](asset-folders.md#working_with_asset_folders)
>* [ 繰り返し発生するアップロードジョブと公開ジョブの処理 ](checking-job-files.md#handling_recurring_upload_and_publish_jobs)
>* [ アップロードジョブまたは公開ジョブをトリガーとして使用 ](checking-job-files.md#using_an_upload_or_publish_job_as_a_trigger)
