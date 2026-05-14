---
title: PSD ファイルの操作
description: Adobe Dynamic Media ClassicでPSD ファイルを操作する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: e3b8c4b9-e9c4-4d7f-84de-2efb456755a1
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T20:08:12.325Z'
TQID: 'https://experienceleague.adobe.com/DkWNVywchW9Lpxgg-u56TlLEmryKxrxc1zKIno8KgfU'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 1029
ht-degree: 22%

---

# PSD ファイルの操作{#working-with-psd-files}

<!--   USED TO BE AN OPTION UNDER COLOR PROFILE OPTIONS * **Convert To sRGB (default)**: Converts to sRGB (Standard Red Green Blue). sRGB is the recommended color space for displaying images on Web pages. -->

PSD（Photoshop ドキュメントファイル）は、Adobe Dynamic Media Classicでテンプレートの作成に最もよく使用されます。 PSD ファイルをアップロードすると、ファイルからAdobe Dynamic Media Classic テンプレートを自動的に作成できます（アップロード画面で「テンプレートを作成」オプションを選択します）。

Adobe Dynamic Media Classicでは、テンプレートを作成するためにファイルを使用する場合、レイヤーを含むPSD ファイルから複数の画像が作成されます。レイヤーごとに1つの画像が作成されます。

## PSD アップロードオプション {#psd-upload-options}

PSD ファイルをアップロードするオプションは、アップロードジョブオプションダイアログボックスのPhotoshop オプションの下にあります。 これらのオプションでは、ファイルを切り抜き、そのファイルのカラープロファイルを作成し、それを使用してテンプレートを作成し、アンカーを選択できます。

これらのオプションは、PSD ファイルのアップロード時に利用できます。

* **切り抜きオプション**: **[!UICONTROL 切り抜きオプション]**&#x200B;の下にあります。 「**[!UICONTROL トリミング]**」を選択すると、PSD ファイルのエッジから余白を自動的にトリミングできます。 「**[!UICONTROL 手動]**」を選択して、PSD ファイルの側面を切り抜きます。

   * **[!UICONTROL トリミング]**:「**に基づいてアウェイをトリミング」メニューを選択し、**&#x200B;[!UICONTROL &#x200B; カラー&#x200B;]&#x200B;**または**&#x200B;[!UICONTROL &#x200B;透明度&#x200B;]&#x200B;**を選択します。**

  「**[!UICONTROL カラー]**」オプションを選択した場合は、「コーナー」メニューを選択し、切り抜くホワイトスペースのカラーを最も的確に表現したカラーを持つPSDのコーナーを選択します。

  スライダをドラッグして、許容値を 0 ～ 1 の範囲で指定します。 色に基づいてトリミングする場合、0 に設定すると、PSD の隅で選択した色と正確に一致するピクセルのみが切り抜かれます。 設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。 透明度に基づいてトリミングするには、ピクセルが透明な場合にのみ切り抜きピクセルに0を指定します。1に近い数値を指定すると、透明度が高くなります。

   * **[!UICONTROL 手動]**：画像の任意の辺または各辺から切り抜くピクセル数を入力します。 画像から切り抜かれる長さは、画像ファイルの ppi（ピクセル/インチ）設定によって異なります。 例えば、画像に150 ppiが表示されているとします。 次に、「上」、「右」、「下」、「左」テキストボックスに「75」と入力します。 画像の各辺が0.5 インチで切り抜かれます。

* **カラープロファイルオプション**: **[!UICONTROL カラープロファイルオプション]**&#x200B;の下にあります。

   * **[!UICONTROL 既定の色保持]**

   * **[!UICONTROL 元のカラースペースを保持]**：画像の元のカラースペースを保持します。

   * **[!UICONTROL カスタム送信元]** > **[!UICONTROL 送信先]**: メニューを開いて、「変換元」と「変換先」カラースペースを選択できるようにします。 標準のPhotoshop カラースペースまたはAdobe Dynamic Media Classicにアップロードしたカラースペースを選択できます。 詳しくは、[ICC プロファイル](/help/using/icc-profiles.md)を参照してください。

* **Photoshop オプション**

   * **[!UICONTROL レイヤーを維持]**: PSD内のレイヤーがある場合は、個々のアセットにリッピングします。 アセットのレイヤーと PSD との関連付けはそのまま保持されます。 ディテールビューでPSD ファイルを開き、レイヤーパネルを選択すると、これらのファイルを表示できます。 詳しくは、PSD ファイルでのレイヤーの表示と編集を参照してください。

   * **[!UICONTROL テンプレートを作成]**: PSD ファイルのレイヤーからテンプレートを作成します。

   * **[!UICONTROL テキストを抽出]**：ユーザーがビューア内のテキストを検索できるように、テキストを抽出します。

   * **[!UICONTROL レイヤーを背景サイズに拡張]**: リッピングされた画像レイヤーのサイズを背景レイヤーのサイズに拡張します。

   * **[!UICONTROL レイヤーの命名]**: PSD ファイルのレイヤーが別々の画像としてアップロードされます。 Adobe Dynamic Media Classicでこれらの画像に名前を付けるには、次のオプションから選択します。

      * **[!UICONTROL レイヤー名]**:PSD ファイル内のレイヤー名の後に画像の名前を付けます。 例えば、元の PSD ファイルで Price Tag という名前のレイヤーは、Price Tag という名前の画像になります。 ただし、PSD ファイル内のレイヤー名がデフォルトのPhotoshop レイヤー名（背景、レイヤー1、レイヤー2など）の場合、PSD ファイル内のレイヤー番号にちなんで名前が付けられます。<!-- not their default layer names -->

      * **[!UICONTROL Photoshopとレイヤー番号]**：元のレイヤー名を無視して、PSD ファイル内のレイヤー番号の後に画像を指定します。 画像には、Photoshop ファイル名の後にレイヤー番号を付加した名前が付けられます。 例えば、`Spring Ad.psd`という名前のファイルの2番目のレイヤーは、Photoshopにデフォルト以外の名前が付いていても`Spring Ad_2`という名前になります。

      * **[!UICONTROL Photoshopとレイヤー名]**: PSD ファイルの後にレイヤー名またはレイヤー番号を付けて画像に名前を付けます。 PSD ファイルのレイヤー名が、初期設定の Photoshop レイヤー名の場合は、レイヤー番号が使用されます。 例えば、`SpringAd`という名前のPSD ファイル内の`Price Tag`という名前のレイヤーは`Spring Ad_Price Tag`という名前です。 既定の名前がLayer 2のレイヤーは`Spring Ad_2`と呼ばれます。

   * **[!UICONTROL Anchor]**: PSD ファイルから生成されたレイヤー構成から生成されたテンプレートで、画像をどのようにアンカーするかを指定します。 初期設定で、アンカーは中央に配置されます。 中央アンカーを使用すると、置き換え画像の縦横比にかかわらず、同じスペースに最適な置き換え画像を作成できます。 この画像を置き換える画像の縦横比が異なる場合も、テンプレートを参照し、パラメータの代入を使用すれば、同じスペースを適切に埋められます。 使用しているアプリケーションが、テンプレートに割り当てられたスペースを置換画像が埋めることを必要とする場合は、別の設定に変更します。

## PSD ファイルでのレイヤーの表示と編集 {#viewing-and-editing-layers-in-a-psd-file}

PSDをアップロードするときに「**[!UICONTROL レイヤーを維持]**」オプションを選択した場合、Adobe Dynamic Media Classicは個々のレイヤーをアセットに取り込みました。 PSD ファイルに属するアセットレイヤーを表示および編集するには、詳細表示の参照パネルでファイルを開きます。

>[!NOTE]
>
>Adobe Dynamic Media Classicは、ネストされたレイヤーグループで最大5つのレベルをサポートします。

1. 参照パネルでPSD ファイル全体をダブルクリックします。 ファイルが詳細ビューで開きます。

   >[!NOTE]
   >
   >PSD レイヤーのいずれかを開くのではなく、アセット全体を開いてください。

1. **[!UICONTROL レイヤー]**&#x200B;を選択します。 すべてのレイヤーが別個の画像としてレイヤーパネルに表示されます。
1. レイヤーをダブルクリックし、次のいずれかの操作を行います。

   * レイヤーに画像マップを作成するには、**[!UICONTROL 画像マップ]** アイコンを選択します。 （[画像マップの作成](creating-image-maps.md#creating_image_maps)を参照）。
   * レイヤーにズームターゲットを作成するには、**[!UICONTROL ズームターゲット]** アイコンを選択します。 （[&#x200B; ガイド付きズームのズームターゲットの作成](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)を参照）。
   * レイヤーを切り抜くには、**[!UICONTROL 切り抜き]** アイコンを選択します。 （[画像の切り抜き](cropping-image.md#cropping_an_image)を参照）。
   * レイヤーをシャープにするには、**[!UICONTROL シャープ]**&#x200B;を選択します。 （[画像をシャープにする](sharpening-image.md#sharpening_an_image)を参照）。
   * レイヤーを調整するには、**[!UICONTROL 調整]**&#x200B;を選択します。 （[画像の調整](adjusting-image.md#adjusting_an_image)を参照）。

1. **[!UICONTROL 保存]**&#x200B;または&#x200B;**[!UICONTROL 別名で保存]**&#x200B;を選択します。
1. 別のレイヤーを表示または編集するには、レイヤープレビューの下部にある矢印を選択します。
1. レイヤーの詳細ビューを終了するには、**[!UICONTROL グリッド表示]** アイコンを選択します。
