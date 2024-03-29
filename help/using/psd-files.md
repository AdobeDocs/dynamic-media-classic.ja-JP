---
title: PSDファイルの操作
description: Adobe Dynamic Media ClassicでPSDファイルを操作する方法を説明します。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '1015'
ht-degree: 24%

---

# PSDファイルの操作{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD(Photoshopドキュメントファイル ) は、テンプレートを作成するためにAdobe Dynamic Media Classicで最もよく使用されます。 PSDファイルをアップロードする際、ファイルからAdobe Dynamic Media Classicテンプレートを自動的に作成できます（アップロード画面の「テンプレートを作成」オプションを選択します）。

Adobe Dynamic Media Classicでは、PSDファイルを使用してテンプレートを作成すると、レイヤーを持つテンプレートファイルから複数の画像が作成されます。テンプレートを使用すると、各レイヤーに対して 1 つの画像が作成されます。

## PSD アップロードオプション {#psd-upload-options}

PSDファイルをアップロードするためのオプションは、アップロードオプションを設定ダイアログボックスの「Photoshopオプション」の下にあります。 これらのオプションでは、ファイルを切り抜き、そのファイルのカラープロファイルを作成し、それを使用してテンプレートを作成し、アンカーを選択できます。

これらのオプションは、PSD ファイルのアップロード時に利用できます。

* **切り抜きオプション**  — 次の場所にあります。 **[!UICONTROL 切り抜きオプション]**. 選択 **[!UICONTROL トリミング]** PSD・ファイルの端から自動的に空白を切り抜くには、「 」を選択します。 **[!UICONTROL 手動]** PSD・ファイルの端を切り抜くには：

   * **[!UICONTROL トリミング]**  — を選択します。 **[!UICONTROL トリミングする対象：]** メニューで、「 」を選択します。 **[!UICONTROL カラー]** または **[!UICONTROL 透明]**.

  次を選択した場合、 **[!UICONTROL カラー]** 」オプションを選択し、切り抜く白いスペースの色を最もよく表す色を持つPSDの隅を選択します。

  スライダをドラッグして、許容値を 0 ～ 1 の範囲で指定します。色に基づいてトリミングする場合、0 に設定すると、PSD の隅で選択した色と正確に一致するピクセルのみが切り抜かれます。設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。透明度に基づいてトリミングする場合は、透明なピクセルのみを切り抜く場合は 0 を指定し、1 に近い数を指定すると透明度が高くなります。

   * **[!UICONTROL 手動]**  — 画像の任意の辺または各辺から切り抜くピクセル数を入力します。 画像から切り抜かれる長さは、画像ファイルの ppi（ピクセル/インチ）設定によって異なります。例えば、画像が 150 ppi と表示され、「上」、「右」、「下」、「左」の各テキストボックスに 75 と入力した場合、「0.5 in」と入力します。 は、画像の両側から切り抜かれます。

* **カラープロファイルオプション**  — 次の場所にあります。 **[!UICONTROL カラープロファイルオプション]**.

   * **[!UICONTROL 初期設定の色の保持]**

   * **[!UICONTROL 元のカラースペースを保持]**  — 画像の元のカラースペースを保持します。

   * **[!UICONTROL カスタム送信元]** > **[!UICONTROL 宛先]** - 「変換元」と「変換先」のカラースペースを選択できるメニューを開きます。 Adobe Dynamic Media Classicにアップロードした標準のPhotoshopカラースペースまたはカラースペースを選択できます。 詳しくは、[ICC プロファイル](/help/using/icc-profiles.md)を参照してください。

* **Photoshop Options**

   * **[!UICONTROL レイヤーを維持]**  — レイヤーがある場合はPSD内のレイヤーを個々のアセットにリッピングします。 アセットのレイヤーと PSD との関連付けはそのまま保持されます。詳細ビューでPSDファイルを開き、画層パネルを選択すると、画層を表示できます。 詳しくは、レイヤーファイルの表示とPSDを参照してください。

   * **[!UICONTROL テンプレートを作成]**  — テンプレートファイル内のレイヤーからPSDを作成します。

   * **[!UICONTROL テキストを抽出]**  — ユーザーがビューアでテキストを検索できるように、テキストを抽出します。

   * **[!UICONTROL レイヤーを背景サイズに拡大]**  — リッピングされた画像レイヤーのサイズを背景レイヤーのサイズに拡大します。

   * **[!UICONTROL レイヤーの命名]** :PSDファイル内のレイヤーは、別々の画像としてアップロードされます。 Adobe Dynamic Media Classicでこれらの画像に名前を付けるには、次のオプションから選択します。

      * **[!UICONTROL レイヤー名]**  — イメージファイル内のレイヤー名の後にPSDの名前を付けます。 例えば、元の PSD ファイルで Price Tag という名前のレイヤーは、Price Tag という名前の画像になります。ただし、PSDファイル内のレイヤー名がデフォルトのPhotoshopレイヤー名（背景、レイヤー 1、レイヤー 2 など）の場合、PSDファイル内のレイヤー番号に基づいてイメージの名前が付けられます。 <!-- not their default layer names -->

      * **[!UICONTROL Photoshopとレイヤー番号]**  — イメージファイルのレイヤ番号に従ってPSDに名前を付けます。元のレイヤ名は無視されます。 画像には、Photoshop ファイル名の後にレイヤー番号を付加した名前が付けられます。例えば、という名前のファイルの 2 番目のレイヤー `Spring Ad.psd` がという名前 `Spring Ad_2` (Photoshopでデフォルト以外の名前が付いていた場合でも )。

      * **[!UICONTROL Photoshopと画層名]**  — イメージファイルの後にPSDの名前を付け、その後にレイヤ名またはレイヤ番号を付けます。 PSD ファイルのレイヤー名が、初期設定の Photoshop レイヤー名の場合は、レイヤー番号が使用されます。例えば、という名前のレイヤー `Price Tag` という名前のPSDファイルに `SpringAd` がという名前 `Spring Ad_Price Tag`. 既定の名前が Layer 2 の画層が呼び出されます。 `Spring Ad_2`.

   * **[!UICONTROL アンカー]**  — 画像ファイルから作成されたレイヤー構成から生成されたテンプレートに画像をアンカーする方法をPSDします。 初期設定で、アンカーは中央に配置されます。中央にアンカーを配置することによって、置換画像は、その縦横比に関係なく、同じスペースを最も適切に埋めることができます。この画像を置き換える画像の縦横比が異なる場合も、テンプレートを参照し、パラメータの代入を使用すれば、同じスペースを適切に埋められます。使用しているアプリケーションが、テンプレートに割り当てられたスペースを置換画像が埋めることを必要とする場合は、別の設定に変更します。

## レイヤーファイル内のPSDの表示と編集 {#viewing-and-editing-layers-in-a-psd-file}

PSDをアップロードする際に「レイヤーを維持」オプションを選択した場合、Adobe Dynamic Media Classicは個々のレイヤーをアセットにリッピングしました。 詳細ビューの参照パネルでファイルを開くと、PSDファイルに属するアセットレイヤを表示および編集できます。

>[!NOTE]
>
>Adobe Dynamic Media Classicは、ネストされた画層グループで最大 5 つのレベルをサポートします。

1. [ 参照 ] パネルでPSDファイル全体をダブルクリックします。 ファイルが詳細ビューで開きます。

   >[!NOTE]
   >
   >PSD レイヤーのいずれかを開くのではなく、アセット全体を開いてください。

1. 選択 **[!UICONTROL レイヤー]**. すべてのレイヤーが別個の画像としてレイヤーパネルに表示されます。
1. 画層をダブルクリックして、次のいずれかの操作を行います。

   * 画層上にイメージマップを作成するには、を選択します。 **[!UICONTROL 画像マップ]** アイコン。 ( 詳しくは、 [画像マップを作成](creating-image-maps.md#creating_image_maps).)
   * レイヤー上にズームターゲットを作成するには、 **[!UICONTROL ズームターゲット]** アイコン。 ( 詳しくは、 [ガイドズーム用のズームターゲットの作成](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom).)
   * レイヤーを切り抜くには、 **[!UICONTROL 切り抜き]** アイコン。 ( 詳しくは、 [画像の切り抜き](cropping-image.md#cropping_an_image).)
   * レイヤーにシャープを適用するには、 **[!UICONTROL シャープ]**. ( 詳しくは、 [画像にシャープを適用](sharpening-image.md#sharpening_an_image).)
   * 画層を調整するには、 **[!UICONTROL 調整]**. ( 詳しくは、 [画像の調整](adjusting-image.md#adjusting_an_image).)

1. 選択 **[!UICONTROL 保存]** または **[!UICONTROL 名前を付けて保存]**.
1. 別の画層を表示または編集するには、画層プレビューの下部にある矢印を選択します。
1. 画層の詳細ビューを終了するには、 **[!UICONTROL グリッド表示]** アイコン。
