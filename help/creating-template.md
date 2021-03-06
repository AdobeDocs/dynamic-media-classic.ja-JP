---
title: テンプレートの作成
description: Adobe Dynamic Media Classicでテンプレートを作成する方法を説明します。
uuid: c762224b-7c6c-4434-bada-c26570079645
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: 8f7093da-d215-4337-ac95-69f0a5bf8648
feature: Dynamic Media Classic
role: User
exl-id: 23ac1a0f-c90b-4250-ae36-93702fb5ebd9
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '3466'
ht-degree: 44%

---

# テンプレートの作成 {#creating-a-template}

テンプレートを作成するには、**[!UICONTROL ビルド]** / **[!UICONTROL テンプレートの基本]** に移動します。 「デザイナー」または「開発者」を選択します。このページで、画像とテキストレイヤーを追加できます。また、レイヤーの順序を変更したり、レイヤーのサイズや位置を変更したり、画像やテキストにシャドウ効果と光彩効果を適用することもできます。

[ テンプレートの基本 ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) トレーニングビデオも参照してください。

>[!NOTE]
>
>以前のバージョンのAdobe Dynamic Media Classicで作成したテンプレートを編集する場合、「キャンバスレイヤーを追加しますか？」を保存すると、プロンプトが表示されます。 ベースレイヤを追加しない場合は、**[!UICONTROL No]** を選択します。 誤って「**[!UICONTROL はい]**」を選択した場合は、URL 内の `&allowCanvasPrompt` 修飾子と `&layer=0` 修飾子を削除して、**[!UICONTROL Enter]** キーまたは **[!UICONTROL Return]** キーを押します。

## 最初のテンプレートの作成 {#creating-the-initial-template}

テンプレートセットを作成する際には、「**[!UICONTROL 保存後に公開]**」オプションがセットおよびセットメンバーに対して次のように影響します。

| **[!UICONTROL 保存前に「保存後に]** 公開」オプションが選択されているか | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

既存のテンプレートからテンプレートを作成できます。テンプレートを開き、「**[!UICONTROL 名前を付けて保存]**」を選択し、名前を付けて保存ダイアログボックスに新しい名前を入力します。

**最初のテンプレートを作成するには：**

1. 初期テンプレートを作成するには、次のいずれかの方法を使用します。

   * **最初にPSDーを選択します**  — 参照パネルで、テンプレートに必要なPSDファイルを 1 つ以上選択し、ビル **[!UICONTROL ド]** / **[!UICONTROL 基本テンプレート]**&#x200B;に移動します。

   * **テンプレート画面から開始します**  — ビル **[!UICONTROL ド]** / **[!UICONTROL テンプレートの基本]**&#x200B;に移動します。「デザイナー」または「開発者」を選択します。

1. カンバスサイズを入力ダイアログボックスで、テンプレートの幅と高さを入力します。
1. アセットライブラリでフォルダを選択して、テンプレートにする PSD ファイルまたは画像をテンプレート画面にドラッグします。
1. 操作が完了したら、ページ右下付近にある「**[!UICONTROL 保存後に公開]**」が選択済み（初期設定）であることを確認します。
1. 「**[!UICONTROL 保存]**」を選択します。
1. テンプレートを保存するフォルダーを選択し、テンプレートの名前を入力して、「**[!UICONTROL 送信]**」を選択します。

   Adobe Dynamic Media Classicは、必要に応じて画像を縮小し、キャンバス（テンプレートを定義するためのテンプレート画面の領域）に合わせます。

## テンプレートセットの編集 {#editing-a-template-set}

公開済みのセットと非公開のテンプレートセットのどちらを編集する場合でも、「**[!UICONTROL 保存後に公開]**」オプションは、セットおよびセットメンバーに対して次の方法で影響を与えます。

| セットが既に公開されているか？ | **[!UICONTROL 編集を保存する前]** に「保存後に公開する」オプションを選択した場合 | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーの公開状態が維持される。編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**テンプレートセットを編集するには：**

1. グリッドビューで、テンプレートセットを参照し、イメージの下の [**[!UICONTROL 編集]**] を選択します。
1. 必要に応じてテンプレートを変更します。
1. 編集が完了したら、ページ右下付近にある「**[!UICONTROL 保存後に公開]**」が選択済み（初期設定）であることを確認します。
1. 「**[!UICONTROL 保存]**」を選択し、保存フォルダーを選択し、セットの名前を入力して、「**[!UICONTROL 保存]**」を選択します。

## テンプレートの削除 {#deleting-a-template}

テンプレートセットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（「子」）は影響を受けず、それらの既存の公開または非公開の状態が維持されます。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**テンプレートを削除するには:**

1. グリッドビュー、リストビューまたは詳細ビューで、1 つ以上のテンプレートを選択します。
1. グローバルナビゲーションバーで、**[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **[!UICONTROL 削除]** に移動します。

## テンプレート画面について {#understanding-the-template-screen}

テンプレート画面には、レイヤーを操作したり、パラメータ化するためのツールがあります。

テンプレート画面で次のツールを使用して、テンプレートを作成できます。

* **[!UICONTROL パン]**  — レイヤーを選択したり、カンバス上でレイヤーを移動したり、サイズを変更したり、回転したりできます。

* **[!UICONTROL テキスト]**  — テキストレイヤーを作成します。カンバス上をドラッグしてテキストレイヤーを作成し、レイヤーにテキストを入力します。[ テキストレイヤーの作成 ](#creating-a-text-layer) を参照してください。

* **[!UICONTROL プレビュー]**  — プレビュー画面を開き、テンプレートをズームビューアで表示します。Web サイトまたはアプリケーション上で、テンプレートがどのように表示されるかを確認できます。

* **[!UICONTROL パラメ]** ータ概要パラメータの概要画面を開きます。テンプレート内の各レイヤーの名前と、各レイヤー上のアクティブにしたパラメータの名前が表示されます。

* **[!UICONTROL テキストエディタ v4.3 およびテキストエディタ v4.2]**  — 最新で最も機能が充実したテキストエディタ、テキストエディタ v4.3、または以前のテキストエディタ v4.2 を使用できます。テンプレートを作成すると、テキストエディタ v4.3 がデフォルトで選択されます。以前のテンプレートを編集する場合は、テキストエディタ v4.2 が初期設定で選択されます。現在、テキストエディタ v4.3 ではワードラップをサポートしていないため、ワードラップを使用している以前のテンプレートを編集する場合は、テキストエディタ v4.2 を使用するとテンプレートを完全な状態で保持することができます。古いテンプレートで折り返しを使用しない場合は、テキストエディタ v4.3 を選択して、提供される多くの新機能を利用できます。 例えば、余白を増やし、余白を減らし、すべて大文字でテキストを設定し、「文字に合わせてコピー」などです。

   >[!NOTE]
   >
   >Adobe Dynamic Media Classicでは、テキストエディター v4.2 がオプションとして削除される予定なので、可能であれば、テキストエディター 4.3 を使用することをお勧めします。 **[!UICONTROL 折り返し]** オプションは、今後のリリースのテキストエディターに組み込まれる予定です。

* **[!UICONTROL デザイナーと開発者]**  — 自分の役割に最も適したオプションを選択します。

* **[!UICONTROL キャンバス]**  — テンプレートを定義するための使用可能な領域の合計をピクセル単位で定義します。初期設定のサイズは、300 x 300 pixel です。レイヤーは、カンバス上に配置されます。

* **[!UICONTROL 「レイヤーリスト」(Layers list]** ) — テンプレート内のレイヤーの名前をリストします。レイヤーを選択するには、「レイヤー」リストで名前を選択します。「レイヤー」リストには、レイヤーに効果を追加したり、レイヤーを削除したり、レイヤーの順序を変更したり、レイヤーをパラメータ化するためのツールがあります。[ レイヤーの操作 ](#working-with-layers) を参照してください。

* **[!UICONTROL レイヤーのプロパティ領域]**  — レイヤーの背景色、不透明度、サイズ、位置、および背景色、不透明度、カンバスのサイズを変更するためのツールを提供します。また、シャドウ効果と光彩効果を調整することもできます。[ レイヤーの操作 ](#working-with-layers) を参照してください。

## 画像レイヤーの作成 {#creating-image-layers}

1. アセットライブラリからカンバスに画像をドラッグします。

   画像の ID 名が「レイヤー」リストに表示されます。

   >[!NOTE]
   >
   >必要に応じて、Adobe Dynamic Media Classicでは、画像レイヤーを作成する際に、画像がキャンバスに収まるように画像が縮小されます。

## テキストレイヤーの作成 {#creating-a-text-layer}

1. **[!UICONTROL テキスト]** ツールを選択します。
1. ドラッグして、カンバスまたは画像にテキストボックスを作成します。
1. 表示されたテキスト画面の「プレビュー」タブで、次のいずれかの操作を行ってテキストを追加します。

   * テキストボックスにテキストを入力します。「テキストフィールドにフィット」を選択してテキストボックスにテキストを合わせます。
   * クリップボードからテキストボックスにテキストをペーストします。

1. 「**[!UICONTROL 適用]**」を選択し、テキスト画面を閉じます。

### テキストの書式設定 {#format-text}

テキストレイヤーのテキストの書式を設定するには、次の操作を行います。

1. 「レイヤー」リストで、編集するテキストのテキストボックス名をダブルクリックします。テキストエディタが表示されます。
1. テキストエディタのテキストボックスで、書式を設定するテキストを選択します。 すべてのテキスト、テキストの一部、または個々の文字を選択できます。
1. 次の書式設定オプションを指定し、**[!UICONTROL 適用]** を選択します。

   * **[!UICONTROL フォント]**  — フォントメニューでフォントを選択します。目的のフォントがメニューに表示されない場合は、Adobe Dynamic Media Classicにアップロードできます。 詳しくは、フォントを参照してください。

   * **[!UICONTROL フォントサイズ]**  — メニューからフォントサイズを選択するか、ボックスに特定のサイズを入力するか、上向き矢印を選択してサイズを 2 ポイントずつ増減しま ****  **** す。

   * **[!UICONTROL 色]**  — テキストの色を選択します。

   * **[!UICONTROL 太字]**、 **[!UICONTROL 斜体]**、または下線 ****  — テキストを選択し、テキストに適用する書式設定の種類のアイコンを選択します。

   * **[!UICONTROL すべて大文字]**、 **[!UICONTROL 上付き文字]**、または下付き文字 ****  — テキストを選択し、テキストに適用する書式の種類のアイコンを選択します。

   * **[!UICONTROL 整列]**  — テキストレイヤー内のテキストを左揃え、中央揃えまたは右揃えにする整列ボタンを選択します。

   * **[!UICONTROL トラッキング]**  — 単語間のスペースの量を調整する数値を入力または選択します。

   * **[!UICONTROL カーニング]**  — 文字間のスペースを調整する数値を入力または選択します。

   * **[!UICONTROL 行間]**  — 行間のスペースを調整する数値を入力または選択します。

   * **[!UICONTROL ベースラインシフト]**  — 選択した文字を周囲のテキストのベースラインを基準に上下に移動する数値を入力または選択します。このオプションは、分数を手動で設定したり、インライングラフィックの位置を調整したりする場合に使用します。

>[!NOTE]
>
>最後の操作を元に戻す場合は、「**[!UICONTROL 元に戻す]**」を選択します。 「**[!UICONTROL 元に戻す]**」を選択した後で、操作のやり直しについて考えを変える場合は、「**[!UICONTROL やり直し]**」を選択します。

### 段落の書式設定 {#format-paragraphs}

1. 「レイヤー」リストで、編集するテキストのテキストボックス名をダブルクリックします。テキストエディタが表示されます。
1. 書式を設定する段落を選択します。
1. 次の書式設定オプションを指定し、**[!UICONTROL 適用]** を選択します。

   * **[!UICONTROL 線形]**  — 線形のタイプを指定する場合に選択します。左揃え、中央揃え、右揃え、または均等揃え。

   * **[!UICONTROL 段落の末尾の位置揃え]**  — 段落の最後の行の位置揃えのタイプを指定する場合に選択します。最後の行は左揃え最後の行は中央揃え最後の行は右揃えになります。

   * **[!UICONTROL 行間]**  — 段落内のすべての行の間隔を調整する数値を入力または選択します。

   * **[!UICONTROL すべてインデント]**  — テキストのインデント幅を増やす場合に選択します。

   * **[!UICONTROL インデントを削除]**  — テキストのインデント量を減らします。

   * **[!UICONTROL 1 行目のインデント]**  — テキストの 1 行目のインデント幅を指定します。

   * **[!UICONTROL 段落前のスペース]**  — 段落の最初の行のテキストの上に表示するスペースの量を指定します。

   * **[!UICONTROL 段落後の空白]**  — 段落の最後の行のテキストの下に表示する空白の量を指定します。

   * **[!UICONTROL 垂直方向の整列]**  — テキストボックス内でテキストを垂直方向に表示する位置を選択します。上、中央、下。

   * **[!UICONTROL テキストの方向]**  — テキストを表示する方向を選択します。右から左、または左から右。

### テキストレイヤーのプロパティの調整 {#adjust-text-layer-properties}

1. 基本テンプレート画面で、調整するテキストボックスを選択します。
1. レイヤーのプロパティパネルで、必要に応じて、次のオプションを選択します。

   * **[!UICONTROL テキストを縮小（テキストエディタ v4.2 のみ）]**  — テキストボックス内に収めるには、「 」を選択してテキストを縮小します。

   * **[!UICONTROL 折り返し（テキストエディタ v4.2 のみ）]**  — テキストを折り返すかどうかを指定するには、折り返しオプションを選択します。

   * **[!UICONTROL 折り返し]**  — テキストを折り返して、横に小さすぎるテキストボックスに収めます。

   * **[!UICONTROL 折り返しなし]**  — テキストボックスが小さすぎる場合に、テキストを折り返さず、代わりにテキストの一部を切り捨てます。

   * **[!UICONTROL 改行なしの折り返し]**  — テキストボックスに収まるようにテキストを折り返し、単語を区切りません。

   * **[!UICONTROL 位置]**  — キャンバス上のテキストボックスの位置を指定します。

   * **[!UICONTROL パディング]**  — 余白を追加するか、レイヤーの長方形を切り抜きます。「左」、「上」、「下」、「右」に対して、追加または削除するピクセル数を指定します。 切り抜く余白または負の数を追加する場合は、正の数を入力します。

### テキストソースコードの表示と編集 {#view-and-edit-text-source-code}

テキストエディタの「ソース」タブに表示される情報は、参照用です。ソースコードの編集に精通している場合にのみ、テキストを編集してください。

1. 「レイヤー」リストで、編集するテキストのテキストボックス名をダブルクリックします。テキストエディタが表示されます。
1. テキストエディタで、テキストのソースコードを表示するには、テキストエディタの「**[!UICONTROL ソース]**」タブを選択します。
1. 必要に応じて、テキストを確認または編集します。

   プレビュー表示とソース表示を切り替えても、変更は反映されないままです。

1. **[!UICONTROL Apply]** を選択して編集内容をレンダリングします。

## レイヤーの操作 {#working-with-layers}

「レイヤー」リストと「レイヤーのプロパティ」領域を使用して、レイヤーを操作します。レイヤー重なり順を変更したり、サイズと位置を変更したり、レイヤーを回転させたり、レイヤーの背景色、前景色、不透明度および描画モードを指定することができます。

また、カンバスのサイズを変更したり、背景色を選択したり、不透明度設定を変更することもできます。

### レイヤーの並べ替え {#reordering-layers}

レイヤーの順序を変更すると、特に透明度やオーバープリントが関係する場合に、外観に影響を与える可能性があります。 変更を確定する前に、必ず結果をプレビューしてください。

1. テンプレート内のレイヤーの順序を変更するには、次の手順のいずれかに従います。

   * 「レイヤー」リストで、レイヤーを選択します。次に、「**[!UICONTROL 上]**」または「**[!UICONTROL 下]**」を必要な回数だけ選択して、リスト内の正しい位置に配置します。
   * 「レイヤー」リストで、レイヤーを上または下にドラッグします。

### レイヤーとキャンバスのサイズと位置の変更 {#changing-the-size-and-position-of-layers-and-the-canvas}

レイヤーは、カンバスに収まるサイズでなければなりません。レイヤーまたはカンバスのサイズは、手動またはサイズ値を入力して変更することができます。レイヤーの位置は、手動またはオフセット値を入力して変更することができます。また、レイヤーを回転させることもできます。

>[!NOTE]
>
>Adobe Dynamic Media Classicでは、テンプレートと同じサイズの画像プリセットを作成することをお勧めします。 画像プリセットのサイズをテンプレートのサイズと同じにすることで、テンプレートの最終出力サイズとシャープオプションが正しく設定されます。画像プリセットの作成後は、テンプレートのプレビュー画面のプリセットを適用メニューからこれを選択することができます。画面には、画像がサーバから配信されたときにどのように表示されるかが示されます。[ 画像プリセットの設定 ](setting-image-presets.md#setting_up_image_presets) を参照してください。

* **レイヤーのサイズの変更**  — レイヤーまたはキャンバスのサイズを変更するには、「レイヤー」リストでレイヤーまたはキャンバスを選択し、次のいずれかの方法を使用します。

* **手動でサイズを変更する**  — レイヤーまたはキャンバスの隅を選択してドラッグします。テキストレイヤーでは、レイヤーの辺をドラッグすることもできます。縦横比（形状）を維持しながらサイズを変更するには、Shift キーを押しながらドラッグします。

* **レイヤーサイズの測定値の入力**  - 「レイヤーのプロパティ」領域の「W」（幅）および「H」（高さ）テキストボックスに、ピクセル値を入力します。

レイヤーのサイズを変更できるとともに、パディングすることもできます。パディングするには、「レイヤーのプロパティ」領域の「左」、「右」、「上」、「下」ボックスにパディング値を入力します。パディングにより、ベースレイヤーの周囲からオフセットさせるためのマージンが現在のレイヤーに追加されます。パディングは、ドロップシャドウや光彩（外側）効果を追加し、これらの効果を目立たせたい場合に便利です。パディングにより、レイヤーのサイズが増加し、拡張されたパディング領域に背景色が表示されます。ベースレイヤーは、レイヤーの新しいサイズを基準に自動的に再配置されます。例えば、現在のレイヤーがベースレイヤーの中央にある場合、レイヤーの左側を広げると、レイヤーはベースレイヤーの右方向へ移動します。

* **レイヤーの位置の変更**  — キャンバス上のレイヤーの位置を変更するには、「レイヤー」リストでレイヤーの名前を選択し、次のいずれかの方法を使用します。

* **位置を手動で変更する**  — レイヤー境界の上ではなく、近くにポインターを移動し、4 方向の矢印カーソルが表示されたら、選択してドラッグを開始します。

* **位置オフセットの測定値の入力**  - X および Y テキストボックスに X および Y オフセットの測定値を入力します。これらの値は、アンカーポイントの x および y オフセット（ピクセル単位）を表します。

* **レイヤーの回転**  - 「回転」(Rotate) ボックスに、レイヤーの回転角度が表示されます。レイヤーを回転させるには、「レイヤー」リストでレイヤーの名前を選択して、次のいずれかの手順に従います。

* **手動で回転**  — レイヤーのコーナーの上ではなく、近くにカーソルを移動します。カーソルが回転カーソルに変わったら、レイヤーの隅をドラッグします。15°単位で回転させるには、Shift キーを押しながらドラッグします。

* **度数の入力**  — 画層を回転する度数を入力します。正の角度値を指定すると時計回りに回転します。反時計回りに回転させるには、負の値を指定します。

**レイヤーまたはレイヤー効果を非表示にする：**

レイヤー名またはレイヤー効果の名前の横にある目のアイコンを選択して、レイヤーまたはレイヤー効果を非表示にすることができます。 非表示になったレイヤーは、プレビューまたは出力で表示されません。レイヤー情報は URL から削除されません。代わりに、URL に `hide=1` が追加され、レイヤーが非表示になっていることに注意してください。 例：

`layer=5&src=is{PortalCo/title}&pos=274,192&effect=-1&.effect=Drop Shadow&blendmode`

`layer=5&src=is{PortalCo/title}&pos=274,192&hide=1&effect=-1&.effect=Drop Shadow&blendmode`

### 背景色、不透明度、および描画モードを指定 {#determining-the-background-color-opacity-and-blend-mode}

レイヤーまたはカンバスの背景色、不透明度、および描画モードを選択するには、レイヤーまたはカンバスを選択して、次のいずれかの手順に従います。

* **前景色**  - 「前景色 **[!UICONTROL 」]** を選択し、カラースウォッチを選択して、シャドウまたは光彩のカラーを変更します。また、ボックスにカラー値パラメータを入力することもできます。背景色は、透明化の設定が有効なレイヤーにのみ適用されます。例えば、値札の部分的に透明なレイヤーや、テキストフィールドの背景に適用されます。透明化の設定がオンになっている PSD、TIFF または PNG 画像で構成されるレイヤーは、背景を透明にすることができます。

* **背景色**  - 「背景色」 **[!UICONTROL を選]** 択し、カラースウォッチを選択して、パディングされた領域の色を変更します。

* **不透明度**  — 不透明度スライダをドラッグして、レイヤーを半透明にし、基になる画像の一部が透けて見えるようにします。100 %の設定は不透明です。0 は透明です。

* **描画モード**  - Photoshopで使用可能な描画モードの 1 つをシミュレートするには、オプションを選択します。標準、ディザ合成、明るく、暗く、乗算、スクリーンのいずれかのオプションを選択します。これらのオプションは、カンバスではなく、レイヤーで利用できます。

## レイヤーにシャドウ効果と光彩効果を使用する {#using-shadow-and-glow-effects-on-layers}

レイヤーにシャドウまたは光彩を適用することができます。シャドウまたは光彩は、レイヤーの周囲に適用され、内側または外側に広がります。どちらに広がるかは、選択したシャドウまたは光彩オプションによって異なります。テンプレートがシャドウ効果とグロー効果を持つPSDファイルで作成された場合は、Adobe Dynamic Media Classicでこれらの効果を調整できます。

シャドウ効果または光彩効果を適用した後に、テンプレート画面の「レイヤーのプロパティ」領域でサイズ、色、不透明度および位置を調整できます。

### レイヤーに影や光彩効果を適用する {#applying-a-shadow-or-glow-effect-to-a-layer}

1. 「レイヤー」リストで、レイヤーを選択します。
1. 効果を追加メニューを選択して、オプションを選択します。

   * **[!UICONTROL ドロップシャドウ]**  — レイヤーの右下にシャドウを適用します。

   * **[!UICONTROL シャドウ（内側）]**  — レイヤーのすべてのエッジの内側にシャドウ効果を適用します。

   * **[!UICONTROL 外光彩]**  — レイヤーのすべてのエッジの周りに光彩効果を適用します。

   * **[!UICONTROL [ 内側光彩]** ] — レイヤーのすべてのエッジ内に光彩効果を適用します。

効果を適用すると、効果名が「レイヤー」リストに表示されます。エフェクトを削除するには、[ レイヤ ] リストで名前を選択し、[**[!UICONTROL 削除]**] を選択します。

>[!NOTE]
>
>基になるレイヤが表示するほど大きくない場合、ドロップシャドウや外側の光彩の効果が見えないことがあります。 シャドウや光彩が見えない場合は、レイヤーにパディング値を追加するか、レイヤーの順序を変更することを検討してください。 詳しくは、[レイヤーとカンバスのサイズと位置の変更](creating-template.md#changing_the_size_and_position_of_layers_and_the_canvas)および[レイヤーの順序の変更](creating-template.md#reordering_layers)を参照してください。

### シャドウ効果またはグロー効果の調整 {#adjusting-a-shadow-or-glow-effect}

シャドウ効果と光彩効果を調整するには、まず「レイヤー」リストで名前を選択します。そして、テンプレート画面の「レイヤーのプロパティ」領域で設定を変更します。

* **[!UICONTROL カラー]**  — カラーボタンを選択し、カラースウォッチを選択して、シャドウまたは光彩のカラーを変更します。また、ボックスにカラー値パラメータを入力することもできます。

* **[!UICONTROL 不透明度]**  — スライダーをドラッグして、効果の強さを指定します。不透明度の低い効果のほうが透明度が高くなります。

* **[!UICONTROL 描画モード]**  - Photoshopで使用可能な描画モードの 1 つをシミュレートするには、オプションを選択します。標準、ディザ合成、明るく、暗く、乗算、スクリーンのいずれかのオプションを選択します。

* **[!UICONTROL サイズ]**  - [X と Y] ボックスに値を入力し、影の効果を拡大または縮小します。サイズオプションは、内側のシャドウとドロップシャドウでのみ利用できます。

* **[!UICONTROL 拡大]**  — スライダーをドラッグして、効果を内側または外側に広げます。

* **[!UICONTROL ぼかし]**  — スライダをドラッグして、効果の端のぼかしを制御します。ぼかしが強い効果のほうが、ぼかし量が多くなります。

## レイヤーのマスク {#masking-layers}

「レイヤー」リストには、レイヤーのマスクまたはアルファチャンネルの使用方法を指定するマスクボタンがあります。マスクボタンを使用して、背景レイヤーの効果を、テンプレート内の特定のレイヤーまたは親レイヤー全体に適用することができます。「レイヤー」リストでレイヤーを選択し、「**[!UICONTROL マスク]**」を選択して次の状態を順に切り替えます。

* レイヤーの背景を不透明にする。
* レイヤーの内容を反転して、レイヤーの背景を黒一色で塗りつぶす。
* レイヤーの背景を黒一色で塗りつぶす。
