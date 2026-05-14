---
title: eCatalog画像マップの作成
description: Adobe Dynamic Media ClassicでeCatalog Image Mapsを作成する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Viewers,eCatalog
role: User
exl-id: 5e7f39a5-36a6-40df-8752-064a582c9346
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T17:43:26.837Z'
TQID: 'https://experienceleague.adobe.com/E1qnvzD2WIqVHt0UAtIq7bZfYlPZbfG9Ye6F9ntX5Q4'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 1505
ht-degree: 26%

---

# eCatalog画像マップの作成{#creating-ecatalog-image-maps}

Image Mapは、eCatalog ページ上のリージョンで、マウスを使用してロールオーバーしたり、さまざまな種類のトリガー操作を選択したりできます。 例えば、画像マップの上にポインターを移動すると、アイテムのロールオーバーテキストの説明が表示されます。 画像マップを選択すると、別のアクションが開始されます。 例えば、Web ページを開いて、閲覧者がアイテムについて詳しく知ったり購入したりできるようにしたり、ビデオを起動して使用中のアイテムを表示したりできます。

## eCatalog画像マップの描画 {#drawing-ecatalog-image-maps}

eCatalog では、eCatalog 画面の「ページをマップ」タブで画像マップを描画します。 この画面は、eCatalog のページを表示する画像マップ領域と、右側に表示される画像マップリストから構成されます。 画像マップを作成すると、その名前は画像マップリストに入力されます。

1. eCatalogのロールオーバー&#x200B;**[!UICONTROL 編集]** ボタンを選択します。
1. **[!UICONTROL ページをマップ]**&#x200B;を選択します。
1. ページをマップ画面の左側で、必要なページを選択します。
1. 以下の手順に従って、長方形または多角形の画像マップを画像マップ領域で描画します。

   * **長方形マップ**：長方形画像マップツールを選択し、ページ上でドラッグして長方形を作成します。

   * **多角形マップ**：多角形の画像マップツールを選択し、画像の周囲を必要な回数だけ選択します。 選択すると、Adobe Dynamic Media Classicは画像マップの境界線を描画します。

     画像マップを描画すると、Adobe Dynamic Media Classicは画像マップリストに名前を割り当てます。 名前を作成するために、Adobe Dynamic Media Classicは、作業しているeCatalog ページの名前に連続番号を追加します。

1. （オプション）画像マップリストの[!UICONTROL 名前]列に、画像マップの新しい名前を入力できます。 名前を入力するときは、空白を入力しないでください。
1. ビューアが画像マップを選択すると、新しいWeb ページを開くことができます。 画像マッピングリストパネルで、「URL」列にWeb ページのURLを入力します。

   URL （Href テンプレート）の入力を簡単にするには、**[!UICONTROL 編集]**&#x200B;を選択してテンプレートを入力します。

[ テンプレートを使用してJavaScriptとURLを入力する](creating-image-maps.md#using_a_template_to_enter_javascript_and_urls)を参照してください。

1. （オプション）表示ドロップダウンリストで「**[!UICONTROL テキストをロールオーバー]**」を選択し、ユーザーが画像マップ上にポインターを移動したときに画面に表示するテキストを入力します。
1. （オプション）表示ドロップダウンリストで「**[!UICONTROL その他のアクション]**」を選択し、ユーザーが画像マップ上でポインターを動かしたときに、ぼかしまたはフォーカスアクションをトリガーする属性を入力します。

   画像マップ ](creating-image-maps.md#defining_other_actions_for_image_maps)に対する他のアクションの定義を参照してください。[

1. **[!UICONTROL 保存]**&#x200B;を選択します。
1. （オプション）「**[!UICONTROL プレビュー]**」を選択して、デフォルトのeCatalog ビューアプリセットでeCatalogを表示します。

画像マップを削除するには、画像マップリストでその名前を選択し、**[!UICONTROL 削除]**&#x200B;を選択します。 画像マップを削除せずに、ページ上の画像マップを一時的に無効にすることができます。 画像マップリストパネルで、「画像マップのオン」オプションを選択します。

## eCatalogへのリッチメディアの埋め込み {#embedding-rich-media-in-an-ecatalog}

eCatalogのリッチメディアオプションを使用して、eCatalogに追加した画像マップにMP4形式またはスピンセットのビデオを追加できます。 ユーザーがeCatalogの画像マップ領域を選択すると、関連するスピンセットまたはビデオが表示されます。 この機能は、顧客に使用中のアイテムを表示したい場合や、異なる角度や展望からアイテムを表示したい場合に特に役に立ちます。

また、オプションとして、お客様が画像マップ上にポインターを移動したときにツールチップのテキストを表示して、お客様が何を選択しているかを把握することもできます。

**リッチメディアをe カタログに埋め込むには：**

1. eCatalog 画像マップを描画します。

   [ カタログ画像マップを描画](creating-ecatalog-image-maps.md#drawing_ecatalog_image_maps)を参照してください。

1. 表示ドロップダウンリストで、**[!UICONTROL リッチメディア]**&#x200B;を選択します。
1. 左側の「Assetsを追加」パネルで、埋め込むスピンセットまたはビデオ（MP4形式）アセットを含むフォルダーに移動します。
1. アセットを画像マップにドラッグします。
1. （オプション）画像マップリストパネルの&#x200B;**[!UICONTROL ツールヒント]**&#x200B;列ヘッダーの下に、画像マップ上にポインターを移動したときに画面に表示するテキストを入力します。
1. **[!UICONTROL 保存]**&#x200B;を選択します。

## eCatalog 画像マップの編集 {#editing-ecatalog-image-maps}

eCatalog 画面の「ページをマップ」タブを選択し、以下の手順に従って、eCatalog の画像マップを編集できます。

* **位置を調整**: パンツールを選択し、ポインターをマップの境界線の近くではなく上に移動します。 ポインターに4方向の矢印が表示されたら、画像マップ全体を新しい場所にドラッグします。

  [画像マップの位置、形状、サイズを調整する](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)を参照してください。

* **シェイプとサイズを変更**：長方形の画像マップのサイズを変更するには、パン ツールを選択します。 左右の境界線または角の部分にポインタを合わせ、ポインタが 2 方向の矢印アイコンに変わったら、ドラッグします。 多角形の画像マップのサイズを変更する場合は、正方形の選択ハンドルをドラッグします。 選択ハンドルを作成するには、画像マップの境界線を選択してドラッグします。

  [画像マップの位置、形状、サイズを調整する](creating-image-maps.md#adjusting_the_position_shape_and_size_of_image_maps)を参照してください。

* **画像マップの削除**: パンツールを選択し、画像マップを選択して選択してから、**[!UICONTROL 削除]**&#x200B;を選択します。

  eCatalogからすべての画像マップを削除するには、「**[!UICONTROL ページを注文]**」タブを選択し、「**[!UICONTROL マップをクリア]**」を選択します。

* **重なる画像マップの処理**: ドラッグして、画像マップリスト上の画像マップの順序を変更します。

  [重複する画像マップの処理](creating-image-maps.md#handling_overlapping_image_maps)を参照してください。

* **画像マップを他のページにコピー**:「**[!UICONTROL マップをコピー]**」を選択します（「ページをマップ」タブに表示していることを確認してください）。 画像を選択画面で、画像マップをコピーするページを選択し、**[!UICONTROL 選択]**&#x200B;を選択します。

  [画像マップを他の画像にコピー](creating-image-maps.md#copying_image_maps)を参照してください。

>[!NOTE]
>
>eCatalog内の別のページに画像マップをコピーする場合、eCatalog内のすべての画像マップを別のeCatalogにコピーできます。 [他の電子カタログの中から画像マップをコピー](creating-ecatalog-image-maps.md#copying_image_maps_between_ecatalogs)を参照してください。

## 画像マップデータのレビューと読み込み {#reviewing-and-importing-image-map-data}

マップの概要画面を開くと、eCatalog のメタデータが表示されます。 また、この画面から、eCatalog の画像マップデータをバッチ読み込みすることもできます。 この方式で画像マップデータを読み込むようにすると、画像マップの URL やロールオーバーテキストを簡単に入力できるようになります。

マップの概要画面を表示するには、eCatalog画面の「マップページ」タブで、「**[!UICONTROL 概要]**」を選択します。

### 画像マップのデータ概要の確認 {#review-image-map-data-summary}

1. マップ ページ画面で、**[!UICONTROL 概要]**&#x200B;を選択します。

   マップの概要画面には、eCatalogに含まれる画像マップ、URL、ロールオーバーテキストの説明およびその他のアクションの数が表示されます。

1. ロールオーバーキーエラーがある場合は、**[!UICONTROL Rollover_Key Error]**&#x200B;列のエラーを選択して、エラーを修正するためにスプレッドシートで何を変更する必要があるかを確認します。 このメッセージのテキストを選択し、コピーしてスプレッドシートにペーストできます。
1. eCatalog Viewerでページを調べることができるように、**[!UICONTROL プレビュー]**&#x200B;を選択します。 「X」を選択して概要画面を閉じてページをマップ画面に戻るか、「**[!UICONTROL 閉じる]**」を選択して「参照」に戻ります。

### 画像マップデータの読み込み {#import-image-map-data}

ページごとに画像マップデータを入力する方法もありますが、eCatalog 全体のデータをマップの概要画面で読み込むこともできます。 イメージマップデータは、タブ区切りファイルまたは XML DTD 形式で読み込みます。 ファイルのフィールドの並び順は、マップの概要画面の表示順と同じにする必要があります。名前、TOC ラベル、マップ、URL、ロールオーバーテキスト、その他のアクション、検索文字列の順に並ぶようにしてください。 画像マップデータを読み込むと、各画像マップを作成する際に、画像マップリストにデータを入力する手間が軽減されます。

>[!NOTE]
>
>画像マップデータを読み込む場合、対応する画像マップが既に作成されている必要があります。

マップの概要画面を開き、以下の手順のいずれかに従って、作成した画像マップに対応する画像マップデータを読み込みます。

1. **[!UICONTROL マップデータの読み込み]**&#x200B;を選択します。
1. メタデータの読み込みダイアログボックスで、**[!UICONTROL 参照]**&#x200B;を選択し、タブ区切りまたはXML DTD ファイルを選択します。
1. ファイルの拡張子を変更しないように注意しながら、「ジョブ名」フィールドにファイルの名前を入力します。
1. 「**[!UICONTROL アップロード]**」を選択します。

## 画像マップを他のeCatalogsとコピーする {#copying-image-maps-between-ecatalogs}

eCatalog 内のすべての画像マップを別の eCatalog にコピーできます。 画像マップのコピーというこの方法により、同じ eCatalog の各国語版で容易に画像マップをコピーすることができます。 コピーを成功させるには、Adobe Dynamic Media Classicでは、同じページ数と同じ画像のe カタログ間でコピーすることをお勧めします。

>[!NOTE]
>
>画像マップのコピー先の eCatalog に既に画像マップが含まれている場合、コピー時にそれらの画像マップは削除されます。

1つのeCatalog内のすべての画像マップを別のeCatalogにコピーするには、次の操作を行います。

1. コピーする画像マップが含まれているeCatalogを選択し、eCatalogのロールオーバー&#x200B;**[!UICONTROL 編集]** ボタンを選択します。
1. 「注文ページ」タブで、「**[!UICONTROL マップをコピー]**」を選択します。
1. アセットを選択ダイアログボックスで、画像マップをコピーするeCatalogを選択し、**[!UICONTROL Select]**&#x200B;を選択します。

画像マップをコピーする対象のeCatalogのページ数や画像サイズが異なる場合、Adobe Dynamic Media Classicに警告メッセージが表示されます。 警告にもかかわらず、画像マップをコピーするには、**[!UICONTROL 続行]**&#x200B;を選択します。
