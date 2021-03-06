---
title: アップロード時の画像の微調整オプション
description: AdobeDynamic Media Classicのアップロード時に使用できる画像の微調整オプションについて説明します。
uuid: 0912ae6f-41c9-41b5-94d1-e266face782e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: d3f21cdf-2cb3-46e8-955a-b8daf0b233bc
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 2d9fc6d8-973f-4aaa-bc2c-b49cda2cde58
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '1166'
ht-degree: 51%

---

# アップロード時の画像の微調整オプション{#image-editing-options-at-upload}

AI、EPS、PSD ファイルなどの画像ファイルをアップロードする際、アップロードオプションを設定ダイアログボックスで次の編集操作を実行できます。

* 画像の端からの余白の切り抜き
* 手動での画像の端の切り抜き
* カラープロファイルの選択
* クリッピングパスからのマスクの作成
* アンシャープマスクオプションによる画像へのシャープの適用
* 背景のノックアウト

これらのオプションは、アップロードページの「 **[!UICONTROL 画像編集オプション]** 」見出しの下にあります。

## 画像の空白の切り抜き

画像の空白ピクセルを自動的に切り抜くには、アップロードオプションを設定ダイアログボックスで「**[!UICONTROL 切り抜きオプション]**」を選択します。 **[!UICONTROL 切り抜き]**&#x200B;ドロップダウンリストで、「**[!UICONTROL トリミング]**」を選択します。 次のオプションを選択します。

* **[!UICONTROL トリミングする部分を選択]**  — このドロップダウンリストから、色と透明度のどちらに基づいて切り抜くかを選択します。

   * **[!UICONTROL カラー]**  - 「色」オプションを選 **** 択します。次に、「**[!UICONTROL コーナー]**」ドロップダウンリストから、切り抜く白のスペースの色を最も表す色の画像の隅を選択します。

   * **[!UICONTROL 透明度]**  - 「透明度」オプションを選択します。

* **[!UICONTROL 許容値]**  — スライダをドラッグして、許容値を0 ～ 1の範囲で指定します。

   * **色に基づくトリミング**  — 画像の隅で選択した色と完全に一致するピクセルのみを切り抜く場合は、0を指定します。設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。

   * **透明度に基づくトリミング**  — 透明なピクセルのみを切り抜く場合は0を指定します。1に近い値を指定すると、透明度が高くなります。

## 画像の側面からの手動切り抜き

画像の端を手動で切り抜くには、切り抜きメニューを選択し、「手動」を選択します。次に、画像の一部または全部の辺から切り抜くピクセル数を入力します。画像から切り抜かれる長さは、画像ファイルの ppi（ピクセル/インチ）設定によって異なります。例えば、画像の解像度が 150 ppi で、「上」、「右」、「下」、「左」の各テキストボックスすべてに 75 を入力した場合、各辺から 1/2 インチずつ切り抜かれます。

## カラープロファイルを選択

画像のカラースペースを選択するには、「カラープロファイル」オプションを選択します。

* **[!UICONTROL sRGBに変換]**  - sRGB（標準の赤緑青）に変換します。Web ページに画像を表示する場合のカラースペースには sRGB が推奨されます。

* **[!UICONTROL 元のカラースペースを保持]**  — 元のカラースペースを保持します。

* **[!UICONTROL カスタムの変換元]** / **[!UICONTROL 変換先]**  - 「変換元」と「変換先」のカラースペースを選択できるメニューを開きます。標準のPhotoshopカラースペースまたはDynamic Media ClassicにアップロードしたAdobeのカラースペースを選択できます。

詳しくは、[ICC プロファイル](icc-profiles.md#icc_profiles)を参照してください。

## クリッピングパスからのマスクの作成

クリッピングパス情報に基づいて画像のマスクを作成するには、「**[!UICONTROL クリッピングパスからマスクを作成]**」を選択します。 このオプションは、画像編集アプリケーションで作成される際に、クリッピングパスが作成された画像に適用されます。

## アンシャープマスクを使用した画像のシャープ

このフィルターを使用すると、ダウンサンプリングされた最終的な画像に対するシャープフィルター効果を微調整できます。 効果の強さ、効果の半径（ピクセル単位）、無視されるコントラストのしきい値を制御できます。

この効果は、Photoshop の「アンシャープマスク」フィルターと同じオプションを使用します。その名称とは異なり、アンシャープマスクはシャープ適用フィルターの一種です。

「アンシャープマスク」で、目的のオプションを設定します。次の表に、設定オプションについて示します。

| アンシャープマスクのオプション | 説明 |
| --- | --- |
| 適用量 | 端のピクセルに適用されるコントラストの量を制御します。<br><br>このオプションは効果の適用度と考えてください。AdobeDynamic Media Classicのアンシャープマスクの量の値とAdobe Photoshopの量の値の主な違いは、Photoshopの量の範囲が1%～500%である点です。 一方、AdobeDynamic Media Classicでは、値の範囲は0.0 ～ 5.0です。AdobeDynamic Media Classicでは、5.0の値はPhotoshopでは500%と大体同じ値です。値が0.9の場合は、90%と等しくなります。 |
| 半径 | 効果の半径を制御します。<br><br>値の範囲は 0 ～ 250 です。この効果は、画像内のすべてのピクセル上で実行され、すべてのピクセルから全方向に放射されます。半径の単位はピクセルです。例えば、2000 x 2000ピクセルの画像と500 x 500ピクセルの画像に対して同様のシャープニング効果を得るには、2000 x 2000ピクセルの画像に2ピクセルの半径を設定します。 次に、500 x 500ピクセルの画像の1ピクセルの半径値を設定します。 ピクセル数の多い画像ほど大きい値が使用されます。 |
| しきい値 | しきい値は、アンシャープマスクフィルターが適用されたときに無視されるコントラストの範囲です。この効果は、このフィルタを使用する際に画像に「ノイズ」が入り込まないように、重要です。 値の範囲は 0 ～ 255 です。これはグレースケール画像における明るさのステップ数です。0 = 黒、128 = 50% グレーおよび 255 = 白。<br><br>例えば、しきい値に 12 を指定すると、肌のトーンの明るさがわずかに変化しても無視されノイズが追加されません。しかし、まつげと皮膚が接触する場所のようにコントラストの強い場所にはエッジのコントラストが追加されます。<br><br>例えば、誰かの顔の写真がある場合、「アンシャープマスク」は画像のコントラストの強い部分に影響します。例えば、まつげと皮膚が交わり、明らかなコントラストの領域を作り出し、滑らかな皮膚自体を作り出す場合です。 滑らかな肌でも、明るさの値によって微妙な変化を示します。しきい値を使用しない場合、このフィルターによって肌のピクセル内の微妙な変化が強調されます。そのため、ノイズの多い望ましくない効果となる一方、まつげのコントラストが増加し、シャープさが強調されます。<br><br>これを防ぐには、しきい値を導入して、滑らかな肌のようにコントラストが急激に変化しないピクセルは無視するフィルターとなるようにします。<br><br>以前に示したファスナーのグラフィックで、ファスナーの横のテクスチャを見てください。しきい値が小さすぎてノイズを抑えることができず、画像のノイズが現れています。 |
| モノクロ | 画像の明るさ（適用度）にアンシャープマスクを適用する場合は選択します。<br><br>各カラーコンポーネントに対して個別にアンシャープマスクを適用する場合は選択解除します。 |

[画像のシャープ](sharpening-image.md#sharpening_an_image)も参照してください。

[AdobeDynamic MediaおよびImage Serverでの画像のシャープ](/help/assets/s7_sharpening_images.pdf)も参照してください。

## ノックアウトの背景

ノックアウトの背景を使用すれば、画像をアップロードしたときにその背景を自動的に削除できます。このテクニックは、特定のオブジェクトへの注意を引き、煩雑な背景から際立たせるために便利です。

| ノックアウトの背景のオプション | 説明 |
| --- | --- |
| ノックアウトの背景 | 選択すると、ノックアウトの背景機能およびオプションが有効または「オン」になります。 |
| 隅 | 必須。<br>ノックアウトする背景色を定義するために使用する画像の隅です。<br>「<b>左上」、「左下」、「右上」または「右下</b>」から選択できます。 |
| Fill メソッド | 必須。<br>設定した「隅」の場所からのピクセル透明化の方法を制御します。<br>次の塗り方から選択できます。<br> ・  <b>Flood Fill</b>  — 指定した隅と一致し、接続されているすべてのピクセルを透明にします。<br>・  <b>ピクセルを一致</b>  — 画像上の位置に関係なく、一致するすべてのピクセルを透明にします。 |
| 許容値 | （オプション）<br>設定した「隅」の場所に基づいて一致するピクセルカラーの許容されるバリエーション量を制御します。<br>値 0.0 を使用すると、完全に一致するピクセルカラーが対象になります。値 1.0 を使用する場合は、最大のバリエーションが許容されます。 |

>[!MORELIKETHIS]
>
>* [画像の切り抜き](cropping-image.md#cropping_an_image)

