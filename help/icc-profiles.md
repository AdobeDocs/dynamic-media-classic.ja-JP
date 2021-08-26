---
title: ICC(International Color Consortium)プロファイル
description: Dynamic Media ClassicのICCプロファイルについて説明します。
uuid: 708ff2ad-9a47-4e3e-b643-5b19648f726b
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/support_files
discoiquuid: 44f1b4c4-6d7f-4e0f-84ce-11d26745e0f0
feature: Dynamic Media Classic
role: User
exl-id: 989f2761-f5d0-4ece-b2a6-f7b4577aa8a2
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 54%

---

# ICC プロファイル［ICC ぷろふぁいる］{#icc-profiles}

ICC（International Color Consortium）プロファイルは、画像ファイルのカラースペースを正しく変換する方法が記述されたファイルです。ICC プロファイルにより、画像の正しい色を得ることができます。例えば、コンピュータのモニタに出力するように設計された画像を正しく表示するには、ICC プロファイルを選択します。このプロファイルは、画像を異なるカラースペースに変換し、オンラインで正確に色が表示されるようにします。

AdobeDynamic Media Classicでは、画像をアップロードする際に、ICCプロファイルを選択して、画像を別のカラースペースに変換できます。 すべての標準的なPhotoshop ICCプロファイルは、AdobeDynamic Media Classicでデフォルトで使用できます。 アップロード画面でカラープロファイル名を表示するには、カラープロファイルメニューを選択します。そして、「カスタム アップロード元 > アップロード先」を選択して、変換前メニューと変換後メニューで ICC プロファイル名を選択します。

[アップロード時の画像編集オプション](image-editing-options-upload.md#image-editing-options-at-upload)を参照してください。

デフォルトのICCプロファイルを使用する以外に、他のICCプロファイルをAdobeDynamic Media Classicにアップロードして、カラースペース変換に使用できるようにすることができます。 参照パネルの詳細表示に切り替えて、ICCプロファイルのプロファイルクラス、カラースペースの種類、PCSの種類を調べます。

## ICCプロファイルのアップロード {#uploading-icc-profiles}

ICC プロファイルのアップロードは、ファイルをアップロードするのと同じ方法で行います。ICCプロファイルは、任意のAdobeDynamic Media Classicフォルダーに保存できます。

[ファイルのアップロード](uploading-files.md#uploading_your_files)を参照してください。

## ICCプロファイルの確認 {#examining-an-icc-profile}

ICCプロファイルを確認するには、参照パネルでICCプロファイルを選択して詳細ビューで表示します。 詳細表示は、ICCプロファイルに関する次の情報を提供します。

* **[!UICONTROL プロファイルクラス]**  - ICC(International Color Consortium)は、アプリケーションのタイプをカバーする各クラスを定義します。例えば、入力プロファイルはデジタルカメラやスキャナなどに対応し、出力プロファイルはプリンタに対応しています。

* **[!UICONTROL カラースペースタイプ]**  — この番号は、ICCによって定義される、プロファイルの「入力」カラースペースです。カラースペースの種類は、カラースペースの構成要素数とそれらの構成要素の解釈を定義します。例えば、RGB は、赤、緑、青の 3 つの構成要素のあるカラースペースです。カラースペースの種類は、スペースの特定の色特性は定義しません（例えば、原色の色度）。

* **[!UICONTROL PCSの種類]**  — このPCSの種類は、プロファイルの「出力」カラースペースで、プロファイル接続スペースです。例えば、カラープロファイルは RGB から PCS に変換して、その後 CMYK に変換することができます。

色や画像のタグ付けに使用する入力、表示または出力プロファイルでは、PCS の種類は XYZ または Lab です。このプロファイルを、ICC 仕様に定義されている対応する特定のカラースペースとして解釈します。
