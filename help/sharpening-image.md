---
title: 画像へのシャープの適用
seo-title: 画像へのシャープの適用
description: 'null'
seo-description: 画像にシャープを適用する方法について説明します。
uuid: d86af74a-89c5-4f2b-96ba- f2e7da600bca
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/master_ files
discoiquuid: 11cd5362- d90a-4c1e- bfbd-46a65a554409
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 画像へのシャープの適用 {#sharpening-an-image}

シャープとは、デジタル画像のアウトラインを鮮明に表示するための画像操作方法です。シャープの適用によって、エッジのピクセル間のコントラストが大きくなり、領域の明暗が強調されます。また、局所的なコントラストも大きくなるので、微細な部分がはっきりと表示されます。すべての画像に正しくシャープを適用できる決まった方法はありません。シャープが足りなければ、ぼやけた画像になりますが、過剰なシャープは、ハロー、アーチファクトおよびノイズの原因になります。

Dynamic Media Classicでは、すべての画像に画像プリセットを使用することを強くお勧めします。これにより、画像プリセットで呼び出された画像に対して均等サイズとシャープの適用が実行されます。さらに、画像プリセットのシャープ適用パラメータの編集と変更が非常に簡単になります。次回に公開する際、そのプリセットで呼び出されたすべての画像には新しい値が与えられます。

また、Dynamic Media Classicでは、ビューアプリセットにシャープを追加してから、そのプリセットを使用してビューアを呼び出すことをお勧めします。これにより、ビューア内の画像が鮮明で魅力的になります。

ただし、画像プリセットやビューアプリセット、またはシャープの適用の代替方法のいずれかを使用するかどうかに関係なく、画像をよりシャープにすることが重要です。そうしないと、画像（および Web サイト）がぼやけて、曖昧に見えます。

>[!NOTE]
>
>「シャープ」コマンドは、シャープ効果を含めた画像プリセット設定を上書きします。画像プリセットは、ダイナミックメディアImage Serverから配信される画像のサイズと形式を制御します。Dynamic Media Classicでは、画像プリセットを使用してすべての画像を配信し、画像が均一のサイズとシャープで配信されることを確認することを強くお勧めします。ただし、いったん個別の画像にシャープを設定すると、その後、画像プリセットのシャープ設定が画像に適用されなくなります。このような画像は、画像プリセットのシャープ設定を適用せずに配信されます。

多くの場合、画像にシャープを適用する必要があります。ダイナミックメディアクラシックSPSおよび画像サーバには、シャープの適用オプションがいくつか用意されています。シャープの適用が画像に与える影響や、シャープの適用がどの程度必要であるか理解することが重要です。ほとんどの画像にシャープを適用する必要がありますが、要求される程度は画像によって異なります。

画像にシャープを適用すると、ピクセルのコントラストが増加し、エッジの強調効果が出ます。人間は、この強調されたエッジのコントラストをシャープとして認識します。画像にシャープフィルタを適用して、画像を強調することは簡単ですが、画像にシャープを適用しすぎることも多くなります。

画像にシャープを適用しすぎると、光輪効果または境界線のバンディングが発生します。

Scene7Publishing SystemおよびDynamic Media Image Serverで画像のシャープを最適化するために実行できるベストプラクティスがあります。

Scene7Publishing [SystemおよびDynamic Media Image Serverで画像をシャープにするためのベストプラクティス](https://marketing.adobe.com/resources/help/en_US/s7/sharpening/s7_sharpening_images.pdf)を参照してください。

**画像にシャープを適用する方法**

To sharpen an image, click its rollover **Edit** button and choose Sharpen, or open it in the Browse Panel in Detail view, then click **Sharpen**. シャープエディタ画面が開き、シャープの各コマンドが表示されます。コマンドを選択し、 **「保存**」をクリックします。

>[!NOTE]
>
>画像にシャープを適用する前に、プリセットを適用メニューを選択し、画像プリセットを選択して、そのシャープ効果を確認します。画像プリセットのシャープ効果が、対象の画像に適している場合もあります。プリセットを適用メニューは、シャープエディタ画面の下部にあります。

**シャープオプション**

以下の表には、Image Server の「シャープの適用」オプションが示されています。

| 名前 | URL プロトコル | 値 | 例 |
|--- |--- |--- |--- |
| 単純なシャープの適用 | op_sharpen | `0 | 1` | op_sharpen=1 |
| 再サンプルモード | resMode | `bilin | bicub | sharp2 | trilin`<br><br>bilin：標準的なバイリニア補間を選択します。最も高速な再サンプル法です。ただし、いくつかのエイリアシングアーチファクトが多少目に付きます。<br>bicub：バイキュービック補間を選択します。bilin よりも CPU 使用率が増えますが、エイリアシングアーチファクトが少ないシャープな画像になります。<br><br>sharp2：修正ランチョス窓関数を補間アルゴリズムとして選択します。バイキュービック法よりも多少シャープな結果になりますが、CPU 使用率はさらに高くなります。<br><br>trilin：修正トリリニア補間を選択し、可能な場合は、高い解像度と低い解像度の両方を使用します。エイリアシングが問題となっている場合にのみ使用することをお勧めします。周波数の高いデータが削減されることから、JPEG のサイズが小さくなります。 | resMode=sharp2 |
| アンシャープマスク | op_usm | amount、radius、threshold、monochuamount<br><br>:フィルター強度係数（実数0…5）<br><br>半径:フィルターカーネル半径（実数0…250） <br><br>しきい値:フィルタしきい値レベル（int0…255）<br><br>モノクロ:各カラーコンポーネントを個別にアンシャープマスクするには0に設定し、画像の明るさ（適用度）にアンシャープマスクを適用するには、1に設定します。 | op_usm=1,1,10,0 |

シャープメニューを選択し、オプションを選択します。

**なし** シャープを無効にします。

**シャープ** :ファイルのサイズを変更した後、ファイル上の単純なシャープを実行します。これは Photoshop の「シャープの適用」フィルタと類似しており、あらゆるユーザパラメータをサポートします。通常は、このフィルタまたはアンシャープマスクを使用しますが、両方を使用することはありません。ベストプラクティスとしてこの方法が推奨されることはありませんが、ボケの補正に役立ちます。（URL： op_sharpen）

**アンシャープマスク** 最終的なダウンサンプリング画像に対してシャープフィルタ効果を微調整できます。効果の適用度、効果の半径（ピクセルで測定）、および無視されるコントラストのしきい値を制御できます。この効果は、Photoshop の「アンシャープマスク」フィルタと同じオプションを使用します。（URL: op_usm）

アンシャープマスクでシャープの適用を微調整するには、これらのオプションを選択します。

**適用量** 端のピクセルに適用するコントラストの量を制御します。初期設定値は 0.0 です。高解像度画像では、この値を 5.0 まで高めることができます。適用量は、フィルタ強度の度合いと考えることができます。Dynamic Media Classicの適用量の設定は、Photoshopの適用量と同じでないことに注意してください。Photoshopでは1%~500%の範囲で適用されますが、ダイナミックMedia Classicでは0.0~5.0の範囲で拡大縮小されます。（例えば、Photoshop では 5.0 は約 500％に相当し、0.9 は 90％に相当します）。

**半径** シャープに影響を与える端のピクセルを囲むピクセル数を指定します。この効果は、画像内のすべてのピクセル上で実行され、全方向に放射されます。

最善の半径値は、画像のサイズに依存します。この値を小さく設定すると、端のピクセルのみにシャープが適用されます。大きい値に設定すると、広い範囲のピクセルにシャープが適用されます。

例えば、2000 x 2000 pixel  の画像と 500 x 500 pixel  の画像において類似したシャープの適用効果を得るには、2000 x 2000 pixel の画像で 2 pixel の半径値を設定します。次に、500 x 500 pixel の画像で 1 pixel の半径値を設定します（値が高いほど、画像のピクセルが多くなります）。

**Threshold** Determines the range of contrast to ignore when the unsharp mask filter is applied. このオプションは、シャープを適用するピクセルが周囲の領域とどの程度異なれば、端のピクセルとみなされシャープが適用されるかを指定します。

しきい値には 0～255 を使用します。これはグレースケール画像における明るさのステップ数です。0 = 黒、128 = 50％グレー、および 255 = 白。例えば、しきい値に 12 を指定すると、肌のトーンの明るさがわずかに変化しても無視され「ノイズ」が追加されません。一方、まつげと皮膚が接触する場所のようにコントラストの強い場所にはエッジのコントラストが追加されます。

例として、ある人物の顔写真があるとします。アンシャープマスクを適用すると、画像の中でコントラストの大きな部分に加えて滑らかな肌自体も影響を受けます。滑らかな肌でも、明るさの値によって微妙な変化を示します。しきい値を使用しない場合、フィルタによって肌のピクセルの微妙な変化が強調され、ノイズの多い効果（おそらく望ましくない）が発生する一方、まつげのコントラストが増加し、シャープさが強調されます（おそらく望ましい）。これを防ぐには、しきい値を使用して、滑らかな肌のようにコントラストが急激に変化しないピクセルは無視するフィルターとなるようにします。ノイズやポスタリゼーションの発生を避けるために——肌トーンを持つ画像の場合、——2~20のしきい値を試してみてください。デフォルトのしきい値を0にすると、画像内のすべてのピクセルがシャープになります。

**「各カラーを** 選択」に適用して、各カラーコンポーネントに個別にシャープを適用します。「明るさ」を選択すると、画像の明るさ領域にシャープが適用されます。

**再サンプリング**

再サンプリングメニューを選択してオプションを選択します。これらのオプションは、ダウンサンプリングした画像をシャープにします。

**なし** 再サンプリングをオフにします。

**バイリニア** 法最も高速な再サンプリング方法一部のエイリアシングアーチファクトは顕著です。

**バイキュービック法** - Image ServerでCPU使用率が増えますが、エイリアシングアーチファクトが少ないシャープな画像になります。

**シャープ2** 「バイキュービック法」オプションよりも多少シャープな結果になりますが、Image ServerのCPUコストはさらに高くなります。

**トリリニア** :可能な場合は、高い解像度と低い解像度の両方を使用します。エイリアシングが問題である場合にのみ推奨されます。この方法では、周波数の高いデータが削減されるため JPEG のサイズが小さくなります。

**シャープの適用と画像プリセット**

最終的な結果を達成するため、3 つのシャープの適用効果をすべて混合できます。ただし、この操作は推奨されません。Dynamic Media Classicでは、シャープ効果を画像プリセットの一部として保存することをお勧めします。画像プリセットを使用すると、小さなテキスト文字列で動的にサイズ変更された画像を作成するために、最も頻繁に使用される画像修飾子をパッケージ化できます。画像プリセットには、ファイル形式（通常は Web 用の JPEG）の値、ピクセル数、および画像へのシャープの適用が含まれます。特定のタイプの画像サイズを作成する必要のある各画像の修飾子を URL に追加する代わりに、「サムネール」などの指定された画像プリセットを作成し、適切なサイズ、ファイル形式およびシャープの適用オプションでサムネールの画像プリセットを設定してから、画像プリセット名を使用して画像を呼び出します。画像プリセットを使用すると、全体的な URL の長さが短縮されます。以下の 2 つの URL は、シャープを適用した、同じ 350 x 350 の JPEG 画像を生成します。

* `https://sample.scene7.com/is/image/S7train/Backpack_A?wid=350&hei=350&fmt=jpeg&qlt=85,0&resMode=sharp2&op_usm=0.9,1.0,8,0`
* `https://sample.scene7.com/is/image/S7train/Backpack_A?$!_s7product$`

画像プリセットは、いつでも変更または更新することができます。画像プリセットに加えた変更の結果は、公開した後、および URL のキャッシュを消去した後に確認できます。

あるサイズカテゴリにおいて、各画像に対して 1 つのプリセットを使用する場合、会社管理者は Web コードを変更せずに、その画像プリセットの定義を更新し、再公開し、その形式を使用して各画像に影響を与えることができます。ベストプラクティスとして、サイト上でユニークなサイズあたりに 1 つの画像プリセットを使用します。画像プリセットを追加するには、設定／アプリケーション設定／画像プリセットに移動します。次に、既存のプリセットを追加または編集します。プリセットの名前自体が、唯一の必須フィールドです。ただし、各プリセットにある程度のシャープを適用する必要があります。

**JPG 画質**

「JPG 画質」オプションは、JPG の圧縮レベルを制御します。

**JPG画質** 圧縮レベルとクロミナンスダウンサンプリングを制御する場合は、このオプションを選択します。

**スライダ** JPG圧縮レベルを指定します。この設定は、ファイルサイズと画質の両方に影響を与えます。JPG画質のスケールは1~100です。

**JPGクロミナンスダウンサンプリング** を有効にすると、周波数の高さよりも周波数の高いカラー情報に目が不透明になるので、JPEG画像は画像情報を輝度とカラーコンポーネントに分割します。JPEG 画像を圧縮すると、輝度成分は最大解像度が維持され、色成分はピクセルのグループの平均化によりダウンサンプリングされます。ダウンサンプリングにより、知覚される品質にほとんど影響を与えることなく、データ量が 1/2 から 1/3 に削減されます。ダウンサンプリングは、グレースケール画像では使用できません。この方法は、コントラストが高い画像（テキストがオーバーレイされた画像など）で圧縮の量を低減させるのに役立ちます。

**全社規模のシャープの適用オプションの設定**

画像プリセットを使用しない場合、または URL 文字列と一緒に具体的な Image Server のシャープの適用プロトコルを渡さない場合、ダウンサンプル時に画像にシャープは適用されません。ただし、これが起こる場合、デフォルトのシャープの適用値を設定すると、すべての画像に対して、常にある程度のシャープが適用されます。

会社のデフォルトのシャープの適用オプションを設定するには、設定／アプリケーション設定／公開設定／Image Server に移動します。デフォルトの再サンプリングモードをシャープ 2 に設定する場合、ダウンサンプル時に常に画像にシャープが適用されます。

**ビューアプリセットへのシャープの追加**

画像へのシャープ修飾子をプリセットに追加しない限り、初期の小さな読み込み画像がぼやけて見えます。これは、シャープを適用せずに、ビューアウィンドウに適合するようダウンサンプルされるためです。

SPS で（画像プリセットのような）ビューアプリセットを使用すると、肌の選択やビューアオプションを含む（印刷ボタンの挿入や、ズームアニメーションの速度制御など）、多数のオプションを一箇所に集中できます。ビューアプリセットは、設定／アプリケーション設定／ビューアプリセットの下にある、画像プリセットと同じセクションに表示されます。

修飾子オプションは、すべての eCatalog、回転、カスタムズームビューアプリセットのコア設定セクションの下に表示されます。修飾子ボックスに URL シャープの適用コマンドを追加することにより、ビューアプリセットを使用してビューアが呼び出されるたびにシャープが追加されます。

ビューアプリセットを呼び出すには、ビューア URL で config= command を使用します。ここに、ビューアプリセット（FantasticoZoom2009）を使用して画像セット（靴）を呼び出す例を示します。

`https://s7d9.scene7.com/s7viewers/html5/ZoomViewer.html?asset=Scene7SharedAssets/ImageSet-Views-Sample&config=S7train/FantasticoZoom2009`

ここに示すプリセットは、ビューアのデフォルトのスキンにシャープを適用し、変更します。

**画像に特有のオーバーライドの作成**

あまり推奨されないシャープの適用方法として、画像ごとにシャープのオーバーライドを作成する方法が挙げられます。この場合、画像プリセットに適用されたシャープが、独自の具体的な値でオーバーライドされます。ただし、この方法は、あらゆるサイズに対して他のすべてのシャープの適用方法をオーバーライドします。画像の解像度があまり高くない場合、およびこれらの小さな画像にとって、画像プリセットの値が高すぎる場合、この方法が最適の使用例になります。この場合、画像ごとにシャープを適用することが必要になる場合があります。

SPS で任意の画像を選択して、詳細ビューに移動し（詳細ビューボタンをダブルクリックするか、押します）、「シャープ」をクリックします。パラメータを変更して、「保存」をクリックします。これにより、シャープの適用修飾子または画像プリセットなど、URL で呼び出すコマンドの代わりに、これらのシャープの適用パラメータを使用するよう Image Server に指示が与えられます。変更を反映させるには、公開する必要があります。