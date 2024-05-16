---
title: PSDファイルの操作
description: Adobe Dynamic Media ClassicでPSDファイルを使用する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 22%

---

# PSDファイルの操作{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

PSD（Photoshop ドキュメントファイル）は、テンプレートを作成するためにAdobe Dynamic Media Classicで最もよく使用されます。 PSDファイルをアップロードするときは、ファイルからAdobe Dynamic Media Classic テンプレートを自動的に作成できます（アップロード画面のテンプレートを作成オプションを選択します）。

Adobe Dynamic Media Classicでは、レイヤーを含むPSDのファイルを使用してテンプレートを作成すると、そのファイルから複数の画像が作成されます。レイヤーごとに 1 つの画像が作成されます。

## PSD アップロードオプション {#psd-upload-options}

PSDファイルをアップロードするためのオプションは、「アップロードジョブオプション」ダイアログボックスの「Photoshopオプション」にあります。 これらのオプションでは、ファイルを切り抜き、そのファイルのカラープロファイルを作成し、それを使用してテンプレートを作成し、アンカーを選択できます。

これらのオプションは、PSD ファイルのアップロード時に利用できます。

* **切り抜きオプション**：の下にあります **[!UICONTROL 切り抜きオプション]**. を選択 **[!UICONTROL Trim]** したがって、PSDファイルの端から空白を自動的に切り抜くことができます。 を選択 **[!UICONTROL 手動]** PSDファイルの各辺を切り抜くには：

   * **[!UICONTROL Trim]**：を選択します **[!UICONTROL トリミング対象カラー]** メニューから選択します。 **[!UICONTROL カラー]** または **[!UICONTROL 透明度]**.

  を選択した場合 **[!UICONTROL カラー]** 隅メニューを選択し、切り抜きたいホワイトスペースの色を最も表現している色のPSDの隅を選択します。

  スライダをドラッグして、許容値を 0 ～ 1 の範囲で指定します。色に基づいてトリミングする場合、0 に設定すると、PSD の隅で選択した色と正確に一致するピクセルのみが切り抜かれます。設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。透明度に基づいてトリミングするには、切り抜くピクセルが透明な場合のみ、0 を指定します。1 に近い数値を指定すると、透明度が高くなります。

   * **[!UICONTROL 手動]**：画像の任意の辺または四辺から切り抜くピクセル数を入力します。 画像から切り抜かれる長さは、画像ファイルの ppi（ピクセル/インチ）設定によって異なります。例えば、画像に 150 ppi と表示されるとします。 次に、[ 上 ]、[ 右 ]、[ 下 ]、[ 左 ] の各テキスト ボックスに 75 と入力します。 画像の各辺が 0.5 インチで切り抜かれます。

* **カラープロファイルオプション**：の下にあります **[!UICONTROL カラープロファイルオプション]**.

   * **[!UICONTROL デフォルトのカラー保持]**

   * **[!UICONTROL 元のカラースペースを維持]**：画像の元のカラースペースを保持します。

   * **[!UICONTROL カスタムの送信元]** > **[!UICONTROL 終了]**：メニューが開き、「変換元」と「変換先」のカラースペースを選択できます。 標準のPhotoshop カラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。 詳しくは、[ICC プロファイル](/help/using/icc-profiles.md)を参照してください。

* **Photoshopのオプション**

   * **[!UICONTROL レイヤーを維持]**:PSD内のレイヤーが存在する場合は、個々のアセットにリッピングされます。 アセットのレイヤーと PSD との関連付けはそのまま保持されます。詳細ビューでPSDファイルを開き、レイヤーパネルを選択すると、これらを表示できます。 詳しくは、PSDファイルでのレイヤーの表示と編集を参照してください。

   * **[!UICONTROL テンプレートを作成]**：テンプレートファイル内のレイヤーからPSDを作成します。

   * **[!UICONTROL テキストを抽出]**：テキストを抽出して、ユーザーがビューアでテキストを検索できるようにします。

   * **[!UICONTROL レイヤーを背景サイズに拡大]**：取り込んだ画像レイヤーのサイズを、背景レイヤーのサイズに拡張します。

   * **[!UICONTROL レイヤーの名前]**:PSDファイル内のレイヤーが別々の画像としてアップロードされます。 Adobe Dynamic Media Classicのこれらの画像に名前を付けるには、次のいずれかのオプションを選択します。

      * **[!UICONTROL レイヤー名]**:PSDファイル内のレイヤー名に従って画像に名前を付けます。 例えば、元の PSD ファイルで Price Tag という名前のレイヤーは、Price Tag という名前の画像になります。ただし、PSDファイル内のレイヤー名がデフォルトのPhotoshop レイヤー名（背景、レイヤー 1、レイヤー 2 など）である場合、画像の名前はPSDファイル内のレイヤー番号に従って付けられます。 <!-- not their default layer names -->

      * **[!UICONTROL Photoshopとレイヤー番号]**：元のレイヤー名を無視して、PSDファイル内のレイヤー番号に従って画像に名前を付けます。 画像には、Photoshop ファイル名の後にレイヤー番号を付加した名前が付けられます。例えば、というファイルの 2 番目のレイヤーです。 `Spring Ad.psd` という名前です `Spring Ad_2` Photoshopにデフォルト以外の名前がある場合でも同様です。

      * **[!UICONTROL Photoshopとレイヤー名]**：画像は、PSDファイルの後に、レイヤー名またはレイヤー番号を付けた名前になります。 PSD ファイルのレイヤー名が、初期設定の Photoshop レイヤー名の場合は、レイヤー番号が使用されます。例えば、という名前のレイヤー `Price Tag` という名前のPSDファイル内 `SpringAd` という名前です `Spring Ad_Price Tag`. レイヤ 2 というデフォルト名のレイヤは、 `Spring Ad_2`.

   * **[!UICONTROL アンカー]**:PSDファイルから生成されたレイヤー化されたコンポジションから生成されたテンプレートで、画像をアンカーする方法を指定します。 初期設定で、アンカーは中央に配置されます。中央アンカーを使用すると、置き換え画像の縦横比に関係なく、同じスペースを最もよく埋めることができる置き換え画像を使用できます。 この画像を置き換える画像の縦横比が異なる場合も、テンプレートを参照し、パラメータの代入を使用すれば、同じスペースを適切に埋められます。使用しているアプリケーションが、テンプレートに割り当てられたスペースを置換画像が埋めることを必要とする場合は、別の設定に変更します。

## PSDファイル内のレイヤーの表示と編集 {#viewing-and-editing-layers-in-a-psd-file}

このオプションを選択した場合 **[!UICONTROL レイヤーを維持]** PSDをアップロードすると、Adobe Dynamic Media Classicによって個々のレイヤーがアセットに取り込まれました。 PSDファイルに属するアセットレイヤーを表示して編集するには、詳細ビューの参照パネルでファイルを開きます。

>[!NOTE]
>
>Adobe Dynamic Media Classicは、ネストされたレイヤーグループで最大 5 レベルをサポートします。

1. 参照パネルでフルPSDファイルをダブルクリックします。 ファイルが詳細表示で開きます。

   >[!NOTE]
   >
   >PSD レイヤーのいずれかを開くのではなく、アセット全体を開いてください。

1. を選択 **[!UICONTROL レイヤー]**. すべてのレイヤーが別個の画像としてレイヤーパネルに表示されます。
1. レイヤーをダブルクリックし、次のいずれかの操作を行います。

   * レイヤにイメージ マップを作成するには、 **[!UICONTROL 画像マップ]** アイコン。 （詳しくは、 [画像マップの作成](creating-image-maps.md#creating_image_maps).）
   * レイヤー上にズームターゲットを作成するには、 **[!UICONTROL ズームターゲット]** アイコン。 （詳しくは、 [ガイド付きズームのズームターゲットの作成](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).）
   * レイヤーを切り抜くには、 **[!UICONTROL 切り抜き]** アイコン。 （詳しくは、 [画像の切り抜き](cropping-image.md#cropping_an_image).）
   * レイヤーをシャープにするには、を選択します。 **[!UICONTROL シャープ]**. （詳しくは、 [画像のシャープニング](sharpening-image.md#sharpening_an_image).）
   * レイヤーを調整するには、を選択します **[!UICONTROL 調整]**. （詳しくは、 [画像の調整](adjusting-image.md#adjusting_an_image).）

1. を選択 **[!UICONTROL 保存]** または **[!UICONTROL 名前を付けて保存]**.
1. 別のレイヤーを表示または編集するには、レイヤープレビューの下部にある矢印を選択します。
1. レイヤの詳細ビューを終了するには、 **[!UICONTROL グリッド表示]** アイコン。
