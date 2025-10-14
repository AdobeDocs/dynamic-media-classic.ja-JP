---
title: プライマリ画像のアップロード
description: Adobe Dynamic Media Classicにプライマリ画像をアップロードする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# プライマリ画像のアップロード{#uploading-master-images}

画像をAdobe Dynamic Media Classicにアップロードする前に、画像が最高品質のサイズと形式であることを確認してください。 Adobe Dynamic Media Classicでは、十分なピクセル数（長いサイズで 1500～2000 ピクセル）を持つ高品質の画像をアップロードすることをお勧めします。 このサイズ設定により、必要なDynamic Imagingがすべて可能になります。

画像のアップロードについて詳しくは、[&#x200B; ファイルのアップロード &#x200B;](uploading-files.md#uploading_files) を参照してください。

**アップロード用のプライマリ画像を準備：**

Adobe Dynamic Media Classicにアップロードする前に、プライマリ画像ファイルを準備します。

* **画像サイズ**：予想される最大サイズの画像を作成します。 一般的な画像サイズは、最長サイズで 1500 ～ 2500 ピクセルです。 Adobe Dynamic Media Classic ズーム機能を使用する場合は、最適なズーム詳細を実現するために、最長サイズで 2,000 ピクセル以上の画像を使用することをお勧めします。 Adobe Dynamic Media Classicでは、各画像を最大 25 メガピクセルまでレンダリングできます。 例えば、5000 × 5000 MP の画像や、25 MP までのその他のサイズの組み合わせを使用できます。

* **ファイル形式**:Adobe Dynamic Media Classicでは、すべての標準画像ファイル形式をサポートしています。 これらのフォーマットには、TIFF、BMP、JPEG、PSD、GIF、EPSなどがあります。 可逆圧縮形式（TIFFおよび PNG）をお勧めします。 JPEG画像を使用する場合は、最高画質の設定を使用します。

* **カラースペース**:RGBは、web 画像表示のカラースペースです。印刷に一般的に使用される CMYK 画像は、アップロード時にRGBに自動変換されます。 ICC （International Color Consortium）カラープロファイルが埋め込まれた CMYK 画像をアップロードしてRGBに変換することをお勧めします。 [ICC （International Color Consortium） プロファイル &#x200B;](/help/using/icc-profiles.md) も参照してください。
