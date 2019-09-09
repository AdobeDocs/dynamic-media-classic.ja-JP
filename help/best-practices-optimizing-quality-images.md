---
title: 画質を最適化するためのベストプラクティス
seo-title: 画質を最適化するためのベストプラクティス
description: 'null'
seo-description: 画像画質を最適化するためのベストプラクティスについて説明します。
uuid: 102e83fe- ee2a-443b- ba92-6ad5cc3dayef0
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/master_ files
discoiquuid: 8164466e-2520-482a-88ec-6191fdc77ea3
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 画質を最適化するためのベストプラクティス{#best-practices-for-optimizing-the-quality-of-your-images}

許容範囲内の結果のレンダリングには多数の要因が関係することから、画質の最適化に時間がかかることもあります。知覚される画質は各個人で異なるので、結果はある程度主観的なものと言えます。構造的に実験を行うことが重要です。

Dynamic Media Classicには、画像のチューニングと最適化、結果のレンダリングのための100を超える画像サービングコマンドが含まれています。重要なコマンドおよびベストプラクティスを使用して、このプロセスを効率化し、良い結果をすばやく得るために、次のガイドラインが役に立ちます。

[スマートイメージング](https://helpx.adobe.com/experience-manager/6-3/assets/using/imaging-faq.html)も参照してください。

## Best practices for image format (&amp;fmt=) {#best-practices-for-image-format-fmt}

* 良い画質および扱いやすいサイズと幅で画像を配信するには、JPG または PNG が最良の選択肢です。
* URLに形式コマンドが指定されていない場合、ダイナミックメディア画像サービングのデフォルトはJPGで配信されます。
* JPG は 10:1 の比率で圧縮され、通常は比較的小さい画像ファイルサイズになります。PNG は約 2:1 の比率で圧縮されますが、画像に白の背景が含まれるなどの一部のケースではその限りではありません。ただし、一般的に PNG ファイルのサイズは JPG ファイルよりも大きくなります。
* JPG は非可逆圧縮を使用します。この方式では、圧縮中に画像要素（ピクセル）が消失します。一方、PNG は可逆圧縮を使用します。
* JPG では、シャープなエッジとコントラストを持つ人工的な画像よりも写実的な画像の方がより忠実に圧縮されます。
* 画像に透明部分が含まれる場合は、PNG を使用します。JPG では透明化がサポートされません。

As a best practice for image format, start with the most common setting `&fmt=JPG`.

## 画像サイズのベストプラクティス {#best-practices-for-image-size}

このタスクでは、サイズを指定し、さらにオプションとして画像の縮小に使用するダウンサンプリングモードを指定します。

* For image sizing, the best and most straightforward approach is to use `&wid=<value>` and `&hei=<value>` or just `&hei=<value>`. これらのパラメーターにより、縦横比に応じて画像の幅が自動的に設定されます。
* `&resMode=<value>` は、ダウンサンプリングに使用するアルゴリズムを制御します。から始め `&resMode=sharp2`ます。この値により、最良の画質になります。While using the downsampling value `=bilin` is faster, it often results in the aliasing of artifacts.

画像サイズ調整のベストプラクティスとして、 `&wid=<value>&hei=<value>&resMode=sharp2``&hei=<value>&resMode=sharp2`

## 画像へのシャープ適用のベストプラクティス {#best-practices-for-image-sharpening}

画像へのシャープ適用は、Web サイト上の画像を管理する上で最も複雑な側面であり、ミスが多く起きるところです。次の参考リソースを参照して、Dynamic Media Classicでシャープとアンシャープマスクがどのように動作するかについての詳細を学習してください。

Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

On Adobe TV, watch [Sharpening an image with unsharp mask](https://tv.adobe.com/watch/visual-design-cs6/sharpening-an-image-with-unsharp-mask/).

Dynamic Media Classicでは、取り込み時、配信時、またはその両方に画像をシャープにすることができます。ただし、ほとんどの場合は、両方ではなくいずれかの方法のみを使用して画像にシャープを適用することをお勧めします。通常は、配信時に URL 上の画像にシャープを適用すると最良の結果を得られます。

画像へのシャープの適用に使用できる方法は次の 2 つあります。

* Simple sharpening ( `&op_sharpen`) - Similar to the sharpen filter used in Photoshop, simple sharpening applies basic sharpening to the final view of the image following dynamic resizing. ただし、この方法にはユーザーが設定できる項目はありません。The best practice is to not use `&op_sharpen` unless required.
* Unsharp masking ( `&op_USM`) - Unsharp masking is an industry standard sharpening filter. ベストプラクティスとして、次のガイドラインに従って、アンシャープマスクを使用して画像にシャープを適用します。アンシャープマスクでは、次の 3 つのパラメーターを制御できます。

   * `&op_sharpen=amount,radius,threshold`

      * `amount`（0 ～ 5、効果の強度）
      * `radius`（0 ～ 250、シャープが適用されるオブジェクト周囲に描画される「シャープ線」の幅、ピクセル単位）

         `radius` パラメーターと `amount` パラメーターは互いに反作用することに注意してください。Reducing `radius` can be compensated by increasing `amount`. `Radius` ではより細かい制御が可能であり、値を低く設定すると、端のピクセルだけがシャープになり、高く設定すると広範囲のピクセルがシャープになります。

      * `threshold` （0~255、効果の感度。）

         このパラメーターは、シャープを適用するピクセルが周囲の領域とどの程度異なれば、端のピクセルとみなされフィルターによりシャープが適用されるかを指定します。しきい値は、肌のトーンのような類似した色の領域に過度なシャープが適用されることを防ぐために使用できます。例えば、しきい値に 12 を指定すると、肌のトーンの明るさがわずかに変化しても無視され「ノイズ」が追加されません。一方、まつげと皮膚が接触する場所のようにコントラストの強い場所にはエッジのコントラストが追加されます。
      フィルターで使用するベストプラクティスを含む、これら 3 つのパラメーターの設定方法について詳しくは、次のリソースを参照してください。

      画像へのシャープの適用に関する [Dynamic Media Classicヘルプトピック](https://help.adobe.com/en_US/scene7/using/WS389B162D-2981-41e5-9253-15D22D2ECBC8.html)です。

      Best practices white paper [Sharpening images in Adobe Scene7 Publishing System and on Image Server](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf).

   * Dynamic Media Classicでは、次の4つ目のパラメーターを制御することもできます。monochrome（ `0,1`）.このパラメーターは、アンシャープマスクが各カラーコンポーネントに個別に適用されるか（値 `0` を使用）、画像の明るさ／適用度に適用されるか（値 `1` を使用）を示します。


ベストプラクティスとして、まずはアンシャープマスクの radius パラメーターを使用します。はじめに使用できる radius 設定は次のとおりです。

* Web サイト：0.2 ～ 0.3 pixel
* 写真印刷（250 ～ 300 ppi）：0.3 ～ 0.5 pixel
* オフセット印刷（266 ～ 300 ppi）：0.7 ～ 1.0 pixel
* カンバス印刷（150 ppi）：1.5 ～ 2.0 pixel

amount を 1.75 から 4 まで徐々に増やします。シャープ適用で必要な効果が得られない場合は、radius を小数単位で増やして、もう一度 amount を 1.75 ～ 4 の間で動かします。必要に応じて繰り返します。

monochrome パラメーター設定は 0 のままにします。

## JPEG 圧縮（&amp;qlt=）のベストプラクティス {#best-practices-for-jpeg-compression-qlt}

* このパラメーターは JPG エンコーディングの画質を制御します。値を高く設定すると画質は上がりますがファイルサイズが大きくなり、低く設定すると画質は下がりますがファイルサイズが小さくなります。このパラメーターの範囲は 0 ～ 100 です。
* 高画質を目的として最適化する場合にも、このパラメーターの値を 100 以外に設定してください。90 や 95 の設定と 100 の設定の違いはほぼ認識できない程度ですが、100 を設定すると画像ファイルのサイズが不必要に増加します。Therefore, to optimize for quality but avoid image files becoming too large, set the `qlt=` value to 90 or 95.
* To optimize for a small image file size but keep image quality at an acceptable level, set the `qlt=` value to 80. 70 ～ 75 以下の値に設定すると、画質が大幅に低下します。
* As a best practice, to stay in the middle, set the `qlt=` value to 85 to stay in the middle.
* `qlt=` = での chroma フラグの使用

   * `qlt=` パラメーターには、標準値 `,0` （デフォルト）を使用してRGB色度ダウンサンプリングをオンにしたり、値を使用してオフにしたりでき `,1`ます。
   * To keep it simple, start with RGB chromaticity downsampling turned off ( `,1`). この設定により通常は画質が上がります。特にシャープなエッジやコントラストを多く含む人工的な画像ではそうなります。

As a best practice for JPG compression use `&qlt=85,0`.

## Best practices for JPEG sizing (&amp;jpegSize=) {#best-practices-for-jpeg-sizing-jpegsize}

`jpegSize` は、メモリに制約のあるデバイスに配信するために画像が特定のサイズを上回らないようにする場合に便利なパラメーターです。

* This parameter is set in kilobytes ( `jpegSize=<size_in_kilobytes>`). このパラメーターには、画像配信で許可される最大サイズを定義します。
* `&jpegSize=` は、JPG圧縮パラメーターと相互に作用 `&qlt=`します。If the JPG response with the specified JPG compression parameter ( `&qlt=`) does not exceed the `jpegSize` value, the image is returned with `&qlt=` as defined. Otherwise, `&qlt=` is gradually decreased until the image fits in the maximum allowed size, or until the system determines it cannot fit and returns an error.

As a best practice, set `&jpegSize=` and add the parameter `&qlt=` if you are delivering JPG images to devices with limited memory.

## ベストプラクティスのまとめ {#best-practices-summary}

ベストプラクティスとして、高画質と小さいファイルサイズの両方を達成するために、まずは次のパラメーターの組み合わせを使用します。

`fmt=jpg&qlt=85,0&resMode=sharp2&op_usm=1.75,0.3,2,0`

この設定の組み合わせによって、ほとんどの状況で良好な結果が得られます。

画像をさらに最適化する必要がある場合は、シャープ適用（アンシャープマスク）パラメーターを徐々に微調整します。そのために、まずは radius を 0.2 または 0.3 に設定します。次に、amount を 1.75 から最大 4（Photoshop での 400% に相当）の範囲で徐々に増やします。求められる結果が得られたかを確認します。

シャープの結果にまだ満足できない場合は、radius を小数単位で増やします。小数単位で増やすたびに、もう一度 amount を 1.75 から始め、徐々に 4 まで増やします。求められる結果が得られるまで、このプロセスを繰り返します。上記の値は、制作スタジオで検証されてきたアプローチですが、他の値から始めて、別の方法に従っても問題ありません。ユーザーが満足できる結果であるかどうかは主観的な問題であるので、構造化された実験が重要になります。

実験中は、ワークフローを最適化するために次の一般的な推奨事項が役に立つでしょう。

* Dynamic Media Classic URL上で直接、または調整操作のリアルタイムプレビューを提供するScene7Publishing Systemの画像調整機能を使用して、様々なパラメーターをリアルタイムで試してテストします。
* ベストプラクティスとして、ダイナミックメディア画像サービングコマンドを画像プリセットにグループ化することができます。An image preset is basically URL command macros with custom preset names such as `$thumb_low$` and `&product_high$`. URL パス内にカスタムプリセット名を指定すると、そのプリセットが呼び出されます。この機能により、Web サイト上での様々な画像使用パターンに関するコマンドおよび画質設定を管理でき、URL 全体の長さを短縮することもできます。
* また、Dynamic Media Classicでは、画像の画質を調整するためのより高度な方法も提供されています。例えば、取り込み時に画像をシャープにすることができます。レンダリング結果をさらに微調整して最適化する高度な使用例については、アドビのプロフェッショナルサービスまでお問い合わせください。個々のお客様向けの情報とベストプラクティスを提供いたします。
