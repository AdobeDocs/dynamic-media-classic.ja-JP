---
title: ICC プロファイル［ICC ぷろふぁいる］
description: ICCプロファイルについて説明します。
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
translation-type: tm+mt
source-git-commit: ca12c96d3a76cfa52fd930d190476cb6fc4f4ac7
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 71%

---


# ICC プロファイル［ICC ぷろふぁいる］{#icc-profiles}

ICC（International Color Consortium）プロファイルは、画像ファイルのカラースペースを正しく変換する方法が記述されたファイルです。ICC プロファイルにより、画像の正しい色を得ることができます。例えば、コンピュータのモニタに出力するように設計された画像を正しく表示するには、ICC プロファイルを選択します。このプロファイルは、画像を異なるカラースペースに変換し、オンラインで正確に色が表示されるようにします。

Dynamic Mediaクラシックでは、画像をアップロードするときに、ICCプロファイルを選択して、画像を別のカラースペースに変換できます。 標準的なPhotoshopICCプロファイルはすべて、Dynamic Mediaクラシックでは初期設定で使用できます。 アップロード画面でカラープロファイル名を表示するには、カラープロファイルメニューを選択します。そして、「カスタム アップロード元 > アップロード先」を選択して、変換前メニューと変換後メニューで ICC プロファイル名を選択します。詳しくは、[アップロード時の画像編集オプション](image-editing-options-upload.md#image-editing-options-at-upload)を参照してください。

初期設定のICCプロファイルを使用するだけでなく、他のICCプロファイルをDynamic Mediaクラシックにアップロードして、カラースペースの変換に使用することもできます。 参照パネルで詳細ビューに切り替えて、ICC プロファイルのプロファイルクラス、カラースペースの種類、PCS タイプを調べます。

## ICC プロファイルのアップロード  {#uploading-icc-profiles}

ICC プロファイルのアップロードは、ファイルをアップロードするのと同じ方法で行います。ICCプロファイルは、任意のDynamic Mediaクラシックフォルダに保存できます。 詳しくは、[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## ICC プロファイルの確認  {#examining-an-icc-profile}

ICC プロファイルを確認するには、参照パネルで ICC プロファイルを選択して、詳細ビューで表示します。詳細ビューに、ICC プロファイルに関する次の情報が表示されます。

**プロファイル** クラスICC(International Color Consortium)は、各クラスを定義して、特定の種類のアプリケーションを対象とします。例えば、入力プロファイルはデジタルカメラやスキャナなどに対応し、出力プロファイルはプリンタに対応しています。

**Color Space** Typeこの値は、ICCで定義されているプロファイルの「入力」カラースペースです。カラースペースの種類は、カラースペースの構成要素数とそれらの構成要素の解釈を定義します。例えば、RGB は、赤、緑、青の 3 つの構成要素のあるカラースペースです。カラースペースの種類は、スペースの特定の色特性は定義しません（例えば、原色の色度）。

**PCSの** 種類このPCSの種類は、プロファイルの「出力」カラースペースです。プロファイル接続スペースです。例えば、カラープロファイルは RGB から PCS に変換して、その後 CMYK に変換することができます。

色や画像のタグ付けに使用する入力、表示または出力プロファイルでは、PCS の種類は XYZ または Lab です。このプロファイルを、ICC 仕様に定義されている対応する特定のカラースペースとして解釈します。
