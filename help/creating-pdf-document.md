---
title: PDF ドキュメントの作成
seo-title: PDF ドキュメントの作成
description: 'null'
seo-description: Dynamic Media ClassicのWeb- to- Printプロセスを使用してPDFドキュメントを作成する方法について説明します。
uuid: 274fb06b-320b-40fa-8b61- c224d8aaa1
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/template- publishing
discoiquuid: 87e91e8e-10a2-4fba-87c7- aad2bd798146
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# PDF ドキュメントの作成 {#creating-a-pdf-document}

Web-to-Print プロセスの最後の段階は、カスタマイズされた PDF の生成です。用意された Web アプリケーションを使用してテンプレートをパーソナライズしたエンドユーザは、最終 PDF ドキュメントを作成できます。一般に、この最終 PDF はプリントサービスプロバイダに送稿され、プロ仕様でプリントされます。最終 PDF が意図したとおりにプリントされるようにするため、開発側は正しい joboptions ファイルを使用し、フォント、プリンタマーク、カラーを適切に設定します。

## PDF プリセットの設定 {#setting-up-pdf-presets}

PDFの互換性レベルとプリンターの設定を指定するには、PDF joboptionsファイルを作成してダイナミックメディアクラシックサーバーにアップロードします。例えば、PDF/X-4 互換 PDF 出力を選択することができます（PDF プリント印刷ワークフローの推奨）。joboptions ファイルは、オーサリングソフトウェア（Adobe Illustrator など）または Acrobat で作成できます。印刷業者に必ず連絡をとり、印刷ジョブの適切なジョブオプション設定について助言を受けてください。

joboptions ファイルの作成および Acrobat での joboptions ファイルの作成について詳しくは、Adobe Acrobat ヘルプを参照してください。

joboptions ファイルを Illustrator で作成するには、次の手順に従います。

1. 編集／Adobe PDF プリセットを選択します。
1. ダイアログボックスで、使用するプリセットを選択します。

   Dynamic Media Classicでは、以下のジョブオプション設定がサポートされています。

   | ジョブオプション | 説明 |
   |--- |--- |
   | 一般 | <ul><li>互換性のある形式 </li><li>オブジェクトレベルの圧縮</li><li>サムネールを埋め込み</li><li>Web 表示用に最適化</li></ul> |
   | 画像 | <ul><li>ダウンサンプル</li><li>解像度</li><li>しきい値</li><li>カラー画像、グレースケール画像、白黒画像の圧縮</li></ul> |
   | フォント | <ul><li>すべてのフォントを埋め込む（フォントは初期設定で埋め込まれます）</li><li>OpenType フォントを埋め込む</li><li>使用している文字の割合が次より少ない場合サブセットフォントにする：</li><li>常に埋め込むフォントのリスト</li><li>常に埋め込まないフォントのリスト</li></ul> |
   | カラー | <ul><li>Color Strategy（画像だけタグ付けはすべてタグ付けとして扱われます）</li><li>文書レンダリングインテント</li><li>4.2.5 では以下の作業用スペースのみサポートされています。4.3 では、IPS にアップロードされた任意のカスタマ提供プロファイルを使用できます。</li><li>回避策として、会社の初期設定カラープロファイルを使用して、アートワークの変換先となるカラースペースを指定できます。</li></ul> |
   | RGB | <ul><li>e-sRGB </li><li>scRGB with encoding range [-4.0, 4.0]</li><li>Lab D50</li><li>PCS XYZ</li><li>Flat XYZ</li><li>Linear ROMM-RGB</li><li>ROMM-RGB</li><li>sYCC 8-bit</li><li>e-sYCC 8-bit</li></ul> |
   | グレー | <ul><li>Gray Gamma 1.8</li><li>Gray Gamma 2.2</li><li>Dot Gain 10%</li><li>Dot Gain 15%</li><li>Dot Gain 20%</li><li>Dot Gain 25%</li><li>Dot Gain 30%</li><li>sGray</li></ul> |
   | キャリブレーションされた CMYK カラースペースの CMYK を維持 |  |
   | 詳細設定 | 「OPI コメントを保存」は常にオン |
   | 規格 | 準拠する規格 |

   >[!NOTE]
   >
   >joboptionsファイルのプリンタマーク設定は、Dynamic Media Classicでは無視されます。プリンタマークは、ダイナミックMedia Classic URLコマンドを使用して設定されます。

1. 「書き出し」をクリックし、名前と場所を指定し、「保存」をクリックします。
1. joboptions ファイルをアセットとして Scene7 Publishing System にアップロードします。

   これを URL で参照することで、公開したテンプレートで使用します。以下に例を挙げます。

   `https://yourpublishserver.scene7.com/is/agm/SiliconPublishing/PetNews?&fmt=pdf,cmyk&joboption=SPSfilenameid`

## 印刷用 PDF の準備 {#preparing-the-pdf-for-print}

印刷用 PDF を最終出力する前に、このセクションのガイドラインに従っていることを確認してください。

**画像**

公開ジョブ内のすべての画像がダイナミックMedia Classic Serverにアップロードされ、公開されていることを確認してください。

**フォント**

公開ジョブ内のすべてのフォントがダイナミックMedia Classic Serverにアップロードされ、公開されていることを確認してください。フォントの変更をエンドユーザに許可する予定の場合は、フォントをホストする法的権利を持っていることを確認します。

**画像解像度（ピクセル/インチ）**

ビットマップ画像の解像度は、生成された印刷用PDFのDynamic Media Classicサーバーによって保持されます。Dynamic Media Classicでは、必要に応じて画像解像度がアップ調整されます。最適な結果を得るには、Web でのプレビュー時の解像度を初期設定値（通常は 72 dpi）のままにします。会社のすべての画像の初期設定解像度は、公開設定の Image Server ウィンドウの「初期設定のプリント解像度」セクションで設定されています。高めの解像度（300 dpi など）の場合は処理時間が長くなることがあるので、印刷用 PDF だけに適用します。PDF ジョブの初期設定解像度を手動で上書きするには、imageRes= コマンドを URL で使用します。

**カラーマネジメント**

ドキュメントや画像にはグレースケール、CMYK、名前付きスポットカラー、RGB または Lab カラーモデルを使用できます。どれも、未キャリブレーションでも、ICC カラープロファイルを採用したキャリブレーション済みでもかまいません。最適な結果を得るには、生成される印刷用 PDF にプロファイルを埋め込みます。デフォルトでは、Dynamic Media Classicサーバーはこれを実行します。必要なすべてのカラープロファイルがDynamic Media Classicプラットフォームにアップロードされていることを確認してください。デザインアプリケーションに設定されているカラーマネジメントオプションが、Dynamic Media Classic Serverで設定されているものと一致していることを確認してください。

**デザインアプリケーションのカラーマネジメント設定：**&#x200B;オーサリングアプリケーション（Adobe Illustrator など）のカラー設定で、作業用スペースの RGB および CMYK カラープロファイルを指定します。

**Dynamic Media Classicカラーマネジメントの設定:** 通常、デザインアプリケーションのカラーマネジメント設定は、Dynamic Media Classicサーバーのデフォルトのカラープロファイルと一致する必要があります。設定は公開設定の Image Server ウィンドウで確認できます。

## プリンタマークの表示 {#displaying-printer-marks}

次のいずれかに対して PDF を作成することが考えられます。

* 完成ドキュメント
* フィルムやプレートなど、印刷業者に製作用として入稿する可能性がある中間ドキュメント

中間ドキュメントには、裁ち落としマージンやプリンタマークなど、ほかにも製作コンテンツが含まれている可能性があります。こうしたコンテンツは通常、完成ページの境界外に表示されます。

Acrobat のプリンタマークの追加画面で使用できるすべてのマークを使用できます。プリンタマークは、`printerMark` パラメータを使用して制御されます。The syntax is `&printerMark=trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed`.

* trim marks = 0|1
* bleed marks = 0|1
* registration marks = 0|1
* color bars = 0|1
* page information = 0|1
* style = Illustrator | IllustratorJ | QuarkXPress
* line weight = 0.125 | 0.25 | 0.50
* layer embed = 0|1

印刷製作用にドキュメントを準備する場合は、プリンタマークが必要になります。印刷会社は、このプリンタマークを使用して、校正刷り用の分離フィルムの位置を決め、校正やインク密度を正確に判断するためにフィルムを測定し、サイズに合わせてフィルムをトリミングするなど、様々な作業を行います。プリンタマークは、トリムボックスや裁ち落としボックスなどのドキュメントボックスの境界を示します。製作関連のコンテンツには次のものがあります。

**メディアボックス** ページが印刷される物理媒体の境界。メディアサイズの外側のコンテンツは安全に破棄でき、ファイルの内容に影響を与えません。

**裁ち落としサイズ**&#x200B;裁ち落としサイズには、切断、折りおよびトリミング機器の物理的な限界を反映させるための領域が含まれる場合もあります。初期設定値はページのトリミングサイズです。

**仕上がりサイズ** トリミング後の仕上げページの寸法。仕上がりサイズには、印刷指示、裁断マーク、カラーバーなどの製作関連のコンテンツが含まれるため、メディアサイズより小さくなる場合があります。初期設定値はページのトリミングサイズです。

**アートボックス** ページの作成者が意図するページの意味のあるコンテンツ（余白を含む）の範囲。初期設定値はページのトリミングサイズです。

この表の修飾子を使用すると、Adobe Illustrator、InDesign および Acrobat で利用できるプリンタマークを複製できます。

| 修飾子／値 | 説明 |
|--- |--- |
| bleedMargin=top,left,bottom,right | Acrobat のページボックスを設定ダイアログボックスのオプションで指定されます。「裁ち落としサイズ」を選択し、「余白の制御」で余白を指定します。<br><br>値は、アートワーク（メディアサイズ）の上下左右の端から内側に対する距離を示します。値（0~1000）はポイント単位です。<br><br>New height= original height-（top+ bottom）<br><br>新しいwidth= original width-（left+ right） |
| mediaMargin=top,left,bottom,right | Acrobat のページボックスを設定ダイアログボックスのオプションで指定されます。「ページサイズを変更」の「Custom Page Size」を変更します。<br><br>値は、アートワーク（メディアサイズ）の上下左右の端から外側に対する距離を示します。値（0~1000）はポイント単位です。<br><br>New height= top+ bottom+ original heightNew<br><br>width= top+ bottom+ original widgets<br><br>新しい高さと新しい幅の値によって、生成されるPDFの新しいページサイズが決まります。<br><br>新しいメディアサイズが定義されると、トリムマージンと裁ち落としマージンに関するすべての計算で、新しいメディアサイズをアートワークの端として考慮する必要があります。 |
| trimMargin=top,left,bottom,right | Acrobat のページボックスを設定ダイアログボックスのオプションで指定されます。「仕上がりサイズ」を選択し、「余白の制御」で余白を指定します。<br><br>値は、アートワーク（メディアサイズ）の上下左右の端から内側に対する距離を示します。値（0~1000）はポイント単位です。<br><br>New height= original height-（top+ bottom）<br><br>新しいwidth= original width-（left+ right） |
| printerMark= trim marks, bleed marks, registration marks, color bars, page information, style, line weight, layer embed | 値は次のとおりです。<br><br>trim marks=0,1（初期設定:0）<br><br>bleed marks=0,1（初期設定は0）<br><br>registration marks=0,1（初期設定は0<br><br>）<br><br>page information=0,1（default is0）<br><br>style= Default， InDesignJ1， InDesignJ2， Illustrator， IllustratorJ， QuarkXPress（default is Default） line weight=0.1（default is Default）<br><br>line weight=0.1（初期設定はデフォルトです）25-0.2（初期設定では0.25）<br><br>のどちらの値もレイヤーembed=0，1で、すべてのプリンタマークを含む新しいレイヤーを作成します（初期設定は1）<br><br>。このマークは、使用するスタイルに応じて変わり、マークとカラーバーは異なる、および対応するスタイルと一致しますAcrobat. |

プリンタマークについては、次の点に注意してください。

* プリンタマークを指定するときは、URL 呼び出しを使用して裁ち落としマージン、トリムマージン、メディアマージンを指定します。これらのマージンを指定せずにプリンタマークを指定すると、生成された PDF の表示領域の外側にマークが表示されます。また、トリムマークと裁ち落としマークが重なる場合もあります。
* トリムマージンと裁ち落としマージンに同じマージン値を指定すると、`&printerMark` でこれらのフラグが 1 に設定されている場合に、トリムマークと裁ち落としマークが重なります。
* URL 呼び出しで fmt=swf/image 形式を指定すると、プリンタマークやマージンなしで出力される可能性があります。これは PDF 出力固有の機能です。
* Specifying `&printerMark=`through the URL results in default values being used for all parameters. Specifying `&printerMark=1` results in trim marks being set to 1 and default values for other parameters. ただし、nth 要素を ON に設定するには、すべての（n-1）パラメータを URL 経由で指定する必要があります。
* Specifying only one value for `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in that value being applied to all the top, bottom, left, and right margins of the original artwork.
* Specifying only the top and left values through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the top value being assigned to the bottom value and the left value being equal to the right.
* Not specifying the right value through `&trimMargin`, `&bleedMargin`, and `&mediaMargin` results in the left value being assigned to the right.
* 複数のページがある PDF の場合は、プリンタマーク／マージンがすべてのページに適用されます（Acrobat では、プリンタマーク／マージンのページ範囲を選択できます）。
* プリンタマーク／マージンを有効にした状態で PDF を出力すると、特に指定しない限り、Acrobat X とまったく同じ内容になります。

PDF/X-4 準拠の PDF ファイルを URL で &amp;joboption 修飾子を使用して作成する場合は、PDF ファイル ISO_15930-7-2008.pdf に記述されているプリンタマークに関連する制限事項に注意してください。

* PDF ファイルの各 Page オブジェクトには MediaBox が含まれます。PDF/X-4 準拠ファイルの各 Page オブジェクトには、TrimBox と ArtBox の両方ではなくどちらかが含まれている必要があります。MediaBox は継承によって含まれていることがあります。
* BleedBox が存在する場合は、ArtBox または TrimBox が BleedBox の境界を越えないようにする必要があります。CropBox が存在する場合は、ArtBox、TrimBox、BleedBox のどれもが CropBox の境界を越えないようにする必要があります。
* ArtBox、TrimBox、CropBox、BleedBox のどれもが MediaBox の境界を越えないようにする必要があります。
* 業界によっては BleedBox の使用を必須とする慣行もあります。適切な業務慣行に従ってください。
* ArtBox の使用より TrimBox の使用をお勧めします。
* TrapNet および PrinterMark 注釈以外のすべての注釈には、BleedBox（BleedBox が存在しない場合は TrimBox または ArtBox）の完全に外側となる Rect 値が必要です。すべての PrinterMark 注釈には、TrimBox または ArtBox の完全に外側となる Rect 値が必要です。PDF/X-4 準拠リーダーは、PDF TrapNet 以外の注釈を完全に無視する可能性があります。
* Rect がバウンディングボックスの完全に外側と見なされるのは、Rect のすべての座標がバウンディングボックスの外側または境界上にあり、この 2 つの四角形に交点がない場合です。
* ViewerPreferences ディクショナリに ViewArea、ViewClip、PrintArea、PrintClip のいずれかのキーが含まれている場合、それぞれのキーが MediaBox 値または（BleedBox がファイルのすべてのページオブジェクトに存在する場合は）BleedBox 値を持っている必要があります。

