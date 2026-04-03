---
title: ICC （International Color Consortium）プロファイル
description: Adobe Dynamic Media ClassicのICC プロファイルについて説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
source-git-commit: 2893110e9629ef72a0e919b47abc94c916e132e9
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 31%

---

# ICC プロファイル［ICC ぷろふぁいる］{#icc-profiles}

ICC （International Color Consortium）プロファイルは、あるカラースペースから別のカラースペースに画像ファイルを正しく変換する方法を説明するファイルです。 ICC プロファイルにより、画像の正しい色を得ることができます。 たとえば、コンピュータモニターに印刷するように設計された画像を正しく表示するには、ICC プロファイルを選択できます。 このプロファイルは、画像を異なるカラースペースに変換し、オンラインで正確に色が表示されるようにします。

Adobe Dynamic Media Classicでは、ICC プロファイルを選択して、画像をアップロードするときに画像を別のカラースペースに変換できます。 すべての標準Photoshop ICC プロファイルは、Adobe Dynamic Media Classicでデフォルトで使用できます。 アップロード画面でカラープロファイル名を表示するには、カラープロファイルメニューを選択します。 そして、「カスタム アップロード元 > アップロード先」を選択して、変換前メニューと変換後メニューで ICC プロファイル名を選択します。

アップロード ](image-editing-options-upload.md#image-editing-options-at-upload)の[画像編集オプションを参照してください。

デフォルトのICC プロファイルを使用するだけでなく、他のICC プロファイルをAdobe Dynamic Media Classicにアップロードして、カラースペースの変換に利用できるようにすることもできます。 参照パネルの詳細表示に切り替えて、ICC プロファイルのプロファイルクラス、カラースペースタイプ、およびPCS タイプを調べます。

要約すると、ICC プロファイルの重要なポイントは次のとおりです。

* ICC プロファイルを使用すると、画像ファイルの異なるカラースペース間で正しいカラー変換が可能になります。
* Adobe Dynamic Media Classicには、堅牢な画像変換を実現する、あらゆる標準のPhotoshop ICC プロファイルが組み込まれています。
* カスタム ICC プロファイルにより、高度なカラースペース変換ニーズに対応する柔軟性が向上しました。
* プロファイルクラスやPCS タイプなどの詳細を詳細ビューで表示すると、ICC設定の管理に役立ちます。
* ICC プロファイルのアップロードは簡単で、Dynamic Media Classicのフォルダー間でアクセスできます。


## ICC プロファイルのアップロード {#uploading-icc-profiles}

ICC プロファイルのアップロードは、ファイルをアップロードするのと同じ方法で行います。 ICC プロファイルは、任意のAdobe Dynamic Media Classic フォルダーに保存できます。

[ ファイルのアップロード ](uploading-files.md#uploading_your_files)を参照してください。

## ICC プロファイルを調べる {#examining-an-icc-profile}

ICC プロファイルを調べるには、参照パネルで選択し、詳細ビューに表示します。 詳細ビューには、ICC プロファイルに関する次の情報が表示されます。

* **[!UICONTROL プロファイルクラス]**: ICCは、アプリケーションの種類をカバーする各クラスを定義します。 例えば、入力プロファイルは、デジタルカメラやスキャナーなどのデバイスに適用されます。 出力プロファイルはプリンターに適用されます。

* **[!UICONTROL 色空間タイプ]**：この数値は、ICCで定義されているプロファイルの「入力」色空間です。 カラースペースの種類は、カラースペースの構成要素数とそれらの構成要素の解釈を定義します。 例えば、RGB は、赤、緑、青の 3 つの構成要素のあるカラースペースです。 カラースペースの種類は、スペースの特定の色特性は定義しません（例えば、原色の色度）。

* **[!UICONTROL PCS タイプ]**：このPCS タイプは、プロファイルの「出力」カラースペース（プロファイル接続スペース）です。 例えば、カラープロファイルは RGB から PCS に変換して、その後 CMYK に変換することができます。

カラーや画像のタグ付けに便利な入力、表示、または出力プロファイルの場合、PCS タイプはXYZまたはLabです。 このプロファイルを、ICC 仕様に定義されている対応する特定のカラースペースとして解釈します。
