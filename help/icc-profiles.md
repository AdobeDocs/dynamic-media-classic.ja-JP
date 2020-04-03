---
title: ICC プロファイル
seo-title: ICC プロファイル［ICC ぷろふぁいる］
description: 'null'
seo-description: ICCの機能についてプロファイルします。
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# ICC プロファイル［ICC ぷろふぁいる］{#icc-profiles}

ICC（International Color Consortium）プロファイルは、画像ファイルのカラースペースを正しく変換する方法が記述されたファイルです。ICC プロファイルにより、画像の正しい色を得ることができます。例えば、コンピュータのモニタに出力するように設計された画像を正しく表示するには、ICC プロファイルを選択します。このプロファイルは、画像を異なるカラースペースに変換し、オンラインで正確に色が表示されるようにします。

Scene7 Publishing System では、画像をアップロードするときに ICC プロファイルを選択して、画像を異なるカラースペースに変換することができます。Photoshop のすべての標準的な ICC プロファイルは、Scene7 Publishing System で初期設定で使用することができます。アップロード画面でカラープロファイル名を表示するには、カラープロファイルメニューを選択します。そして、「カスタム アップロード元 > アップロード先」を選択して、変換前メニューと変換後メニューで ICC プロファイル名を選択します。詳しくは、[アップロード時の画像編集オプション](image-editing-options-upload.md#image-editing-options-at-upload)を参照してください。

初期設定の ICC プロファイルに加え、他の ICC プロファイルを Scene7 Publishing System にアップロードして、それらをカラースペースの変換に使用することができます。参照パネルで詳細ビューに切り替えて、ICC プロファイルのプロファイルクラス、カラースペースの種類、PCS タイプを調べます。

## ICC プロファイルのアップロード {#uploading-icc-profiles}

ICC プロファイルのアップロードは、ファイルをアップロードするのと同じ方法で行います。ICC プロファイルは Scene7 Publishing System のあらゆるフォルダに格納できます。詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## ICC プロファイルの確認 {#examining-an-icc-profile}

ICC プロファイルを確認するには、参照パネルで ICC プロファイルを選択して、詳細ビューで表示します。詳細ビューに、ICC プロファイルに関する次の情報が表示されます。

**プロファイルクラス** ICC(International Color Consortium)は、各クラスを定義して、アプリケーションの種類をカバーします。 例えば、入力プロファイルはデジタルカメラやスキャナなどに対応し、出力プロファイルはプリンタに対応しています。

**Color Space Type** ：この数値は、ICCで定義されるプロファイルの「入力」カラースペースです。 カラースペースの種類は、カラースペースの構成要素数とそれらの構成要素の解釈を定義します。例えば、RGB は、赤、緑、青の 3 つの構成要素のあるカラースペースです。カラースペースの種類は、スペースの特定の色特性は定義しません（例えば、原色の色度）。

**PCS Type** ：このPCSの種類は、プロファイルの「出力」カラースペース、つまりプロファイル接続スペースです。 例えば、カラープロファイルは RGB から PCS に変換して、その後 CMYK に変換することができます。

色や画像のタグ付けに使用する入力、表示または出力プロファイルでは、PCS の種類は XYZ または Lab です。このプロファイルを、ICC 仕様に定義されている対応する特定のカラースペースとして解釈します。
