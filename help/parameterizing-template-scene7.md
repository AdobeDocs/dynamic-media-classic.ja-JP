---
title: Dynamic Media Classicでのテンプレートのパラメータ化
seo-title: Dynamic Media Classicでのテンプレートのパラメータ化
description: 'null'
seo-description: Dynamic Media Classicでテンプレートをパラメータ化する方法について説明します
uuid: 27c8c8b4-47f3-4270- a6db- d304648ba357
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/template- publishing
discoiquuid: df1a9ff5- a5ba-4480- ba0d- a19bc665f907
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Dynamic Media Classicでのテンプレートのパラメータ化{#parameterizing-a-template-in-scene}

Dynamic Media Classic FXGとして保存したIllustratorテンプレートをScene7Publishing Systemにアップロードした後、その可変要素を定義できます。これを行うには、印刷テンプレートのビルド画面およびプレビュー画面で可変要素をパラメータ化します。Dynamic Media Classicには、レイヤー上のテキストパラメータとオブジェクトパラメーターを定義し、それぞれのプロパティを定義するツールがあります。また、あるテンプレートの別のバージョンを作成することもできます。

FXG テンプレートをパラメータ化することで、テキスト、画像およびグラフィックの可変性をカスタマイズすることができます。例えば、テキスト行をパラメータ化して、エンドユーザが Web ユーザインターフェイスを使用してテキストを変更できるようにすることができます。空のテキストフィールドを可変として定義して、エンドユーザがこれらのフィールドにパーソナライズされたテキストを入力できるようにすることができます。また、Dynamic Media Classic印刷テンプレートのビルド画面で、デザイン要素の属性とプロパティをパラメータ化することもできます。

>[!NOTE]
>
>DOM操作を使用する予定の場合、Dynamic Media Classicでテンプレートをパラメータ化する必要はありません。

## FXG テンプレートでのパラメータの定義 {#defining-parameters-in-fxg-templates}

Follow these steps in Dynamic Media Classic to define parameters for an FXG template:

1. 参照ウィンドウで、FXG ファイルを選択します。
1. **「ビルド** »をクリックして?«印刷テンプレート»?を選択するか、ファイル?の«編集&#x200B;********

   印刷テンプレート画面が開きます。

1. RRCo\ FXG\ Welcome_ Summit_10（FXGファイル）を選択し、 **ビルド** / **印刷テンプレートをクリック**&#x200B;します。</p>

   ![](assets/wp_fxg_edit.png)

1. 印刷テンプレート画面のレイヤーパネルで、パラメータ化する要素が含まれたレイヤーを選択します。

   >[!NOTE]
   >
   >眼アイコンをクリックしてオンとオフを切り替え、目的のオブジェクトを選択します。

1. プロパティパネルで、「名前」列（テキストをパラメータ化する場合）または「パラメータ」列（オブジェクトをパラメータ化する場合）をクリックします。

   **テキストフィールドのテキスト** をクリックします（プロパティリストの一番下までスクロールして検索します）。パラメータダイアログボックスが表示されます。Select the text that you want to parameterize and click **Add**. テキストの異なる部分を選択してそれぞれにパラメータを追加することで、同じテキストのプロパティから複数のパラメータを作成できます。To change the name of the parameter, click it, enter a new name, and click **Close**.

   **「** パラメーター」列のボックスをクリックします。パラメータの編集ダイアログボックスが表示されます。Enter a name and click **OK**.

   複数の属性を同じ値で一度にカスタマイズするには、属性ごとに同じパラメータ名を使用します。例えば、テンプレートに長方形と星形がある場合、それぞれの「単色」色属性のパラメータ名として「`newcolor`」を入力できます。これにより、「`newcolor`」値を変更するたびに、長方形と星形の両方の色が新しい色に変更されるようになります。

1. 「値」または「データ」フィールドに属性の初期設定値を指定します。選択したオブジェクトのすべてのプロパティを設定し、目的の外観を指定します。
1. （オプション）パラメータ化するすべてのオブジェクトまたはレイヤーで手順 3～5 を繰り返します。
1. 「**保存**」または「**名前を付けて保存**」をクリックします。
1. **「プレビュー」** をクリックしてFXGプレビューウィンドウを開き、作成したパラメータをデフォルト値で表示します。

## FXG テンプレートのオブジェクトまたはレイヤーの表示/非表示 {#show-or-hide-an-object-or-layer-in-the-fxg-template}

非表示になったオブジェクトおよびレイヤーは、プレビューまたは出力結果に表示されませんが、ファイルから削除されたわけではありません。必要に応じて、再び表示することができます。表示/非表示は、変数にすることができる属性です。眼アイコンをクリックしてオンまたはオフにすると、オブジェクトまたはレイヤーの表示/非表示の初期設定値が設定されます。

1. オブジェクトパネルで、オブジェクト名またはレイヤー名の横にある眼アイコンをクリックして、ファイル内で非表示にします。
1. もう一度クリックすると、オブジェクトは表示されます。

## 様々なバージョンのテンプレートの作成 {#create-different-versions-of-a-template}

属性を編集して、用途ごとに異なるバージョンのテンプレートを作成できます。

印刷テンプレート画面で、「名前を付けて保存」をクリックして、元の FXG テンプレートを上書きせずに、新しい FXG テンプレートとしてファイルを保存します。

## ストロークテキストの使用 {#using-stroked-text}

ストロークテキストは、属性をパラメータ化する方法の一例です。ダイナミックメディアClassicは、以下のストロークテキスト機能をサポートしています。

* ストロークの幅
* 破線のストロークパターン
* 異なる結合スタイル
* 異なるキャップエンドスタイル
* ストロークのオーバープリント
* ストロークの個別カラー処理（スポットカラーサポートを含む）

以下の表は、サポートされるストロークテキストの属性を示しています。

| 属性 | 説明 |
|--- |--- |
| s7:fill `<Boolean>`(S7FXG Only) | 塗りをテキストに対して有効にするかどうかを指定する。初期設定は true。 |
| s7:stroke `<Boolean>` (S7FXG Only) | ストロークをテキストに対して有効にするかどうかを指定する。初期設定は false。 |
| s7:weight `<number>` (S7FXG Only) | テキストの線幅をポイント単位で指定する。初期設定は 1 ポイント。 |
| s7:joints `<string>` (miter, round, bevel) (S7FXG Only) | ストロークの結合タイプを指定する。初期設定は round。 |
| s7:caps `<string>` (none, round, square) (S7FXG Only) | ストロークのキャップタイプを指定する。初期設定は round。 |
| s7:miterLimit `<number>` (S7FXG Only) | 結合がストロークのマイター結合である場合のマイター制限を指定する。初期設定は 4。 |
| s7:strokeOverprint `<Boolean>` (S7FXG Only) | ストロークのオーバープリントを有効にするかどうかを指定する。初期設定は false。 |
| s7:strokeColorName（S7FXG のみ） | ストロークのカラー名を定義する以外は s7:colorName と同様。 |
| s7:strokeColorValue（S7FXG のみ） | ストロークに使用されるカラー値を定義する以外は s7:colorValue と同様。 |
| s7:strokeColorspace（S7FXG のみ） | ストロークのカラースペースを定義する以外は s7:colorspace と同様。 |
| flm:dashPattern `<array>` (S7FXG Only) | 初期設定では破線や間隔のパターンはないが、この属性でストロークの破線／間隔のパターンを定義する。最初の値でストロークの破線を指定し、2つ目の値で破線の間隔を指定する。同様に、破線と間隔の値を交互に指定することで、配列を複数の値で拡張できる。 |

## ワープテキストの使用 {#using-warped-text}

ワープテキストにより、波、旗、引き伸ばしなどの効果を追加して、テキストの外観を変更することができます。

ワープテキストは、RichText オブジェクトでサポートしています。縦書きまたは横書き、およびポイントテキスト、エリアテキスト、パス上のテキストをサポートしています。ワープテキストを適用するには、あらかじめテキストオブジェクト全体を選択する必要があります。

ワープテキストは Adobe Illustrator で作成できます。

テキストにワープを適用するときに、次の属性を設定できます。

* スタイル
* 方向
* カーブ
* 水平方向のゆがみ
* 垂直方向のゆがみ

各属性には、一連の値が含まれています。

| 属性 | 値 | 初期設定 |
|--- |--- |--- |
| スタイル7:warpStyle | nonearcarcLowerarcUpperarchbulgeshellLowershellUpperflagwavefishrisefishEyeinflatesqueezetwist | 除外 |
| 方向7:warpDirection | horizontalvertical | 横 |
| カーブ7:warpBend | -1 ～ 1 | 0.5 |
| 水平方向のゆがみ7:warpHorizontalDistortion | -1 ～ 1 | 0 |
| 垂直方向のゆがみ7:warpVerticalDistortion | -1 ～ 1 | 0 |

>[!NOTE]
>
>For `inflate` and `fishEye`, changing the `s7:warpDirection` flag between horizontal and vertical does not have any effect on the output.

ワープテキストの作成および使用方法について詳しくは、Adobe Illustrator のドキュメントを参照してください。

>[!MORELIKETHIS]
>
>* [Illustrator での初期テンプレートの作成](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)
>* [印刷テンプレート用のファイルのアップロード](upload-files-template-publishing.md#upload_files_for_template-publishing)

