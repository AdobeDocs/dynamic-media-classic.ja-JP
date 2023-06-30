---
title: ICC(International Color Consortium) プロファイル
description: Adobe Dynamic Media Classicの ICC プロファイルについて学びます。
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
topic: Administration, Content Management
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 54%

---

# ICC プロファイル［ICC ぷろふぁいる］{#icc-profiles}

ICC（International Color Consortium）プロファイルは、画像ファイルのカラースペースを正しく変換する方法が記述されたファイルです。ICC プロファイルにより、画像の正しい色を得ることができます。例えば、コンピュータのモニタに出力するように設計された画像を正しく表示するには、ICC プロファイルを選択します。このプロファイルは、画像を異なるカラースペースに変換し、オンラインで正確に色が表示されるようにします。

Adobe Dynamic Media Classicでは、ICC プロファイルを選択して、画像をアップロードする際に画像を別のカラースペースに変換できます。 すべての標準のPhotoshop ICC プロファイルは、デフォルトでAdobe Dynamic Media Classicで使用できます。 アップロード画面でカラープロファイル名を表示するには、カラープロファイルメニューを選択します。そして、「カスタム アップロード元 > アップロード先」を選択して、変換前メニューと変換後メニューで ICC プロファイル名を選択します。

詳しくは、 [アップロード時の画像編集オプション](image-editing-options-upload.md#image-editing-options-at-upload).

初期設定の ICC プロファイルを使用する以外に、他の ICC プロファイルをAdobe Dynamic Media Classicにアップロードして、カラースペース変換に使用できるようにすることができます。 参照パネルの詳細表示に切り替えて、ICC プロファイルのプロファイルクラス、カラースペースの種類、PCS の種類を調べます。

## ICC プロファイルをアップロード {#uploading-icc-profiles}

ICC プロファイルのアップロードは、ファイルをアップロードするのと同じ方法で行います。ICC プロファイルは、任意のAdobe Dynamic Media Classicフォルダーに保存できます。

詳しくは、 [ファイルをアップロード](uploading-files.md#uploading_your_files).

## ICC プロファイルを調べる {#examining-an-icc-profile}

ICC プロファイルを確認するには、参照パネルで ICC プロファイルを選択して、詳細ビューで表示します。 詳細表示は、ICC プロファイルに関する次の情報を提供します。

* **[!UICONTROL プロファイルクラス]** - ICC(International Color Consortium) は、アプリケーションのタイプをカバーする各クラスを定義します。 例えば、入力プロファイルはデジタルカメラやスキャナなどに対応し、出力プロファイルはプリンタに対応しています。

* **[!UICONTROL カラースペースの種類]**  — この数は、ICC で定義されているプロファイルの「入力」カラースペースです。 カラースペースの種類は、カラースペースの構成要素数とそれらの構成要素の解釈を定義します。例えば、RGB は、赤、緑、青の 3 つの構成要素のあるカラースペースです。カラースペースの種類は、スペースの特定の色特性は定義しません（例えば、原色の色度）。

* **[!UICONTROL PCS の種類]**  — この PCS タイプは、プロファイルの「出力」カラースペースです（プロファイル接続スペース）。 例えば、カラープロファイルは RGB から PCS に変換して、その後 CMYK に変換することができます。

色や画像のタグ付けに使用する入力、表示または出力プロファイルでは、PCS の種類は XYZ または Lab です。このプロファイルを、ICC 仕様に定義されている対応する特定のカラースペースとして解釈します。
