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
source-git-commit: 914fde11270dc731a261da3305b29dd573584d93
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 2%

---

# プライマリ画像のアップロード{#uploading-master-images}

画像をAdobe Dynamic Media Classicにアップロードする前に、画像が最高品質のサイズと形式であることを確認してください。 Adobe Dynamic Media Classicでは、十分なピクセル数（長いサイズで 1500～2000 ピクセル）を持つ高品質の画像をアップロードすることをお勧めします。 このサイズ設定により、必要なDynamic Imagingがすべて可能になります。

画像のアップロードについて詳しくは、を参照してください [ファイルをアップロード](uploading-files.md#uploading_files).

**アップロード用のプライマリ画像を準備します。**

Adobe Dynamic Media Classicにアップロードする前に、プライマリ画像ファイルを準備します。

* **画像サイズ**  – 予想される最大サイズの画像を作成します。 一般的な画像サイズは、最長サイズで 1500 ～ 2500 ピクセルです。 Adobe Dynamic Media Classic ズーム機能を使用する場合は、最適なズーム詳細を実現するために、最長サイズで 2,000 ピクセル以上の画像を使用することをお勧めします。 Adobe Dynamic Media Classicでは、各画像を最大 25 メガピクセルまでレンダリングできます。 例えば、5000 × 5000 MP の画像や、25 MP までのその他のサイズの組み合わせを使用できます。

* **ファイル形式** - Adobe Dynamic Media Classicでは、TIFF、BMP、JPEG、PSD、GIF、EPSなど、標準の画像ファイル形式をすべてサポートしています。 可逆圧縮画像形式の TIFF および PNG を使用することをお勧めします。JPEGの画像を使用する場合は、最高画質の設定を使用します。

* **カラースペース** - RGBは、web 画像表示のカラースペースです。一般的に印刷に使用される CMYK 画像は、アップロード時に自動的にRGBに変換されます。 RGBに変換するには、ICC （International Color Consortium）カラープロファイルが埋め込まれた CMYK 画像をアップロードすることをお勧めします。 関連トピック [ICC （International Color Consortium）プロファイル](/help/using/icc-profiles.md).
