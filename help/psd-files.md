---
title: PSDファイルの操作
description: Dynamic Media ClassicでのPSDファイルの操作方法をAdobeします。
uuid: 5836b660-6bca-46e7-ab39-1a31d1e0cff2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 4086e3db-5aca-41a0-8f15-302afbf67ddb
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
source-git-commit: ad5270545be502d3aaabba574353787622ab0445
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 29%

---

# PSDファイルの操作{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)** - Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on web pages. -->

PSD(Photoshop Documentファイル)は、AdobeDynamic Media Classicでテンプレートを作成する際に最もよく使用されます。 PSDファイルをアップロードする際に、ファイルからAdobeDynamic Media Classicテンプレートを自動的に作成できます（アップロード画面の「テンプレートを作成」オプションを選択します）。

AdobeDynamic Media Classicは、PSDファイルを使用してテンプレートを作成する場合、レイヤーを持つPSDファイルから複数の画像を作成します。各レイヤーに対して1つのイメージが作成されます。

## PSD アップロードオプション {#psd-upload-options}

PSDファイルのアップロードに関するオプションは、アップロードオプションを設定ダイアログボックスの「Photoshopオプション」にあります。 これらのオプションでは、ファイルを切り抜き、そのファイルのカラープロファイルを作成し、それを使用してテンプレートを作成し、アンカーを選択できます。

これらのオプションは、PSD ファイルのアップロード時に利用できます。

* **切り抜きオプション**  - 「切り抜きオプション」 **[!UICONTROL の下にあります]**。**[!UICONTROL トリミング]**&#x200B;を選択すると、PSDファイルの端から空白が自動的に切り抜かれます。**[!UICONTROL 手動]**&#x200B;を選択して、PSDファイルの側面を切り抜きます。

   * **[!UICONTROL トリミング]**  — トリミン **[!UICONTROL グする部分を選択し]** て、「カラー透 **** 明度」を **[!UICONTROL 選択します]**。

      「**[!UICONTROL カラー]**」オプションを選択した場合は、「コーナー」メニューを選択し、切り抜く白のスペースの色を最も表す色のPSDの隅を選択します。

      スライダをドラッグして、許容値を 0 ～ 1 の範囲で指定します。色に基づいてトリミングする場合、0 に設定すると、PSD の隅で選択した色と正確に一致するピクセルのみが切り抜かれます。設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。透明度に基づいてトリミングする場合は、0を指定すると、ピクセルが透明な場合にのみ切り抜かれます。1に近い値を指定すると、透明度が高くなります。

   * **[!UICONTROL 手動]**  — 画像の任意の辺または各辺から切り抜くピクセル数を入力します。画像から切り抜かれる長さは、画像ファイルの ppi（ピクセル/インチ）設定によって異なります。例えば、画像の解像度が 150 ppi で、「上」、「右」、「下」、「左」の各テキストボックスすべてに 75 を入力した場合、画像の各辺から 1/2 インチずつ切り抜かれます。

* **カラープロファイルオプション**  — カラープロファ **[!UICONTROL イルオプション]**&#x200B;の下にあります。

   * **[!UICONTROL デフォルトの色保存]**

   * **[!UICONTROL 元のカラースペースを保持]**  — 画像の元のカラースペースを保持します。

   * **[!UICONTROL カスタムの変換元]** / **[!UICONTROL 変換先]**  - 「変換元」と「変換先」のカラースペースを選択できるメニューを開きます。標準のPhotoshopカラースペースまたはDynamic Media ClassicにアップロードしたAdobeのカラースペースを選択できます。 詳しくは、[ICC プロファイル](/help/icc-profiles.md)を参照してください。

* **Photoshop オプション**

   * **[!UICONTROL レイヤーを維持]**  - PSD内のレイヤーがある場合は個々のアセットにリップします。アセットのレイヤーと PSD との関連付けはそのまま保持されます。詳細ビューでPSDファイルを開き、レイヤーパネルを選択すると、これらを表示できます。 詳しくは、PSD ファイル内のレイヤーの表示と編集を参照してください。

   * **[!UICONTROL テンプレートを作成]**  - PSDファイル内のレイヤーからテンプレートを作成します。

   * **[!UICONTROL テキストを抽出]**  — ユーザーがビューアでテキストを検索できるように、テキストを抽出します。

   * **[!UICONTROL レイヤーを背景サイズに拡張]**  — 切り取った画像レイヤーのサイズを背景レイヤーのサイズに拡張します。

   * **[!UICONTROL レイヤーの命名]**  - PSDファイル内のレイヤーは別々の画像としてアップロードされます。Dynamic Media Classicでこれらの画像に名前を付けるには、次のオプションから選択します。

      * **[!UICONTROL レイヤー名]**  - PSDファイル内のレイヤー名に従って画像に名前を付けます。例えば、元の PSD ファイルで Price Tag という名前のレイヤーは、Price Tag という名前の画像になります。ただし、PSDファイル内のレイヤー名がデフォルトのPhotoshopレイヤー名（背景、レイヤー1、レイヤー2など）の場合、画像の名前はPSDファイル内のレイヤー番号に従って付けられます。<!-- not their default layer names -->

      * **[!UICONTROL Photoshopとレイヤー番号]**  - PSDファイル内のレイヤー番号に従って画像に名前を付け、元のレイヤー名は無視します。画像には、Photoshop ファイル名の後にレイヤー番号を付加した名前が付けられます。例えば、`Spring Ad.psd`というファイルの2番目のレイヤーの名前は、Photoshopでデフォルト以外の名前が付けられていても`Spring Ad_2`になります。

      * **[!UICONTROL Photoshopとレイヤー名]**  - PSDファイルの後にレイヤー名またはレイヤー番号が続く名前を画像に付けます。PSD ファイルのレイヤー名が、初期設定の Photoshop レイヤー名の場合は、レイヤー番号が使用されます。例えば、`SpringAd`という名前のPSDファイル内の`Price Tag`という名前のレイヤーは、`Spring Ad_Price Tag`という名前になります。 レイヤ2という名前の既定のレイヤは、`Spring Ad_2`と呼ばれます。
   * **[!UICONTROL アンカー]**  - PSDファイルから作成されたレイヤーコンポジションから生成されたテンプレートに画像をアンカーする方法を指定します。初期設定で、アンカーは中央に配置されます。中央にアンカーを配置することによって、置換画像は、その縦横比に関係なく、同じスペースを最も適切に埋めることができます。この画像を置き換える画像の縦横比が異なる場合も、テンプレートを参照し、パラメータの代入を使用すれば、同じスペースを適切に埋められます。使用しているアプリケーションが、テンプレートに割り当てられたスペースを置換画像が埋めることを必要とする場合は、別の設定に変更します。


## PSDファイル内のレイヤーの表示と編集 {#viewing-and-editing-layers-in-a-psd-file}

PSDをアップロードしたときに「レイヤーを維持」オプションを選択した場合、AdobeDynamic Media Classicは個々のレイヤーをアセットに切り離します。 詳細ビューの参照パネルでファイルを開くと、PSDファイルに属するアセットレイヤーを表示および編集できます。

1. 参照パネルで完全なPSDファイルをダブルクリックします。 詳細ビューでファイルが開きます。

   >[!NOTE]
   >
   >PSD レイヤーのいずれかを開くのではなく、アセット全体を開いてください。

1. 「**[!UICONTROL レイヤー]**」を選択します。 すべてのレイヤーが別個の画像としてレイヤーパネルに表示されます。
1. 画層をダブルクリックし、次のいずれかの操作を行います。

   * レイヤー上に画像マップを作成するには、**[!UICONTROL 画像マップ]**&#x200B;アイコンを選択します。 （[画像マップの作成](creating-image-maps.md#creating_image_maps)を参照）。
   * レイヤー上にズームターゲットを作成するには、**[!UICONTROL ズームターゲット]**&#x200B;アイコンを選択します。 （[ガイドズーム用のズームターゲットの作成](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)を参照）。
   * レイヤーを切り抜くには、**[!UICONTROL 切り抜き]**&#x200B;アイコンを選択します。 （[画像の切り抜き](cropping-image.md#cropping_an_image)を参照）。
   * レイヤーをシャープにするには、「**[!UICONTROL シャープ]**」を選択します。 （[画像のシャープ](sharpening-image.md#sharpening_an_image)を参照）。
   * レイヤーを調整するには、**[!UICONTROL 調整]**&#x200B;を選択します。 （[画像の調整](adjusting-image.md#adjusting_an_image)を参照）。

1. 「**[!UICONTROL 保存]**」または「**[!UICONTROL 名前を付けて保存]**」を選択します。
1. 別のレイヤーを表示または編集するには、レイヤープレビューの下部にある矢印を選択します。
1. 画層の詳細ビューを終了するには、**[!UICONTROL グリッドビュー]**&#x200B;アイコンを選択します。
