---
title: ICC （International Color Consortium）プロファイル
description: Adobe Dynamic Media Classicの ICC プロファイルについて説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 50%

---

# ICC プロファイル［ICC ぷろふぁいる］{#icc-profiles}

ICC（International Color Consortium）プロファイルは、画像ファイルのカラースペースを正しく変換する方法が記述されたファイルです。ICC プロファイルにより、画像の正しい色を得ることができます。例えば、コンピュータのモニタに出力するように設計された画像を正しく表示するには、ICC プロファイルを選択します。このプロファイルは、画像を異なるカラースペースに変換し、オンラインで正確に色が表示されるようにします。

Adobe Dynamic Media Classicでは、画像をアップロードする際に画像を別のカラースペースに変換する ICC プロファイルを選択できます。 すべての標準Photoshop ICC プロファイルは、デフォルトでAdobe Dynamic Media Classicで使用できます。 アップロード画面でカラープロファイル名を表示するには、カラープロファイルメニューを選択します。次に、「カスタム開始/終了」を選択し、「変換元」および「変換先」メニューで ICC プロファイル名を選択します。

参照： [アップロード時の画像編集オプション](image-editing-options-upload.md#image-editing-options-at-upload).

デフォルトの ICC プロファイルを使用する以外にも、他の ICC プロファイルをAdobe Dynamic Media Classicにアップロードして、カラースペースの変換に使用できるようにします。 参照パネルの詳細表示に切り替えて、ICC プロファイルのプロファイルクラス、カラースペースタイプ、PCS タイプを調べます。

## ICC プロファイルをアップロード {#uploading-icc-profiles}

ICC プロファイルのアップロードは、ファイルをアップロードするのと同じ方法で行います。ICC プロファイルは任意のAdobe Dynamic Media Classic フォルダーに保存できます。

参照： [ファイルをアップロード](uploading-files.md#uploading_your_files).

## ICC プロファイルの調査 {#examining-an-icc-profile}

ICC プロファイルを調べるには、参照パネルで ICC プロファイルを選択し、詳細ビューで表示します。 詳細ビューには、ICC プロファイルに関する次の情報が表示されます。

* **[!UICONTROL プロファイルクラス]** - ICC （International Color Consortium）は、1 種類のアプリケーションに対応する各クラスを定義しています。 例えば、入力プロファイルはデジタルカメラやスキャナなどに対応し、出力プロファイルはプリンタに対応しています。

* **[!UICONTROL カラースペースタイプ]**  – この数値は、ICC で定義されているプロファイルの「入力」カラースペースです。 カラースペースの種類は、カラースペースの構成要素数とそれらの構成要素の解釈を定義します。例えば、RGB は、赤、緑、青の 3 つの構成要素のあるカラースペースです。カラースペースの種類は、スペースの特定の色特性は定義しません（例えば、原色の色度）。

* **[!UICONTROL PCS タイプ]**  – この PCS タイプは、プロファイルの「出力」カラースペース（プロファイル接続スペース）です。 例えば、カラープロファイルは RGB から PCS に変換して、その後 CMYK に変換することができます。

色や画像のタグ付けに使用する入力、表示または出力プロファイルでは、PCS の種類は XYZ または Lab です。このプロファイルを、ICC 仕様に定義されている対応する特定のカラースペースとして解釈します。
