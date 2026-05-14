---
title: プライマリ画像のアップロード
description: Adobe Dynamic Media Classicにプライマリ画像をアップロードする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:17:09.649Z'
TQID: 'https://experienceleague.adobe.com/xi8ZvTLYacPSL7P2uqo142VpXY6SOOU7cZvA7tT0zOQ'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 275
ht-degree: 0%

---

# プライマリ画像のアップロード{#uploading-master-images}

Adobe Dynamic Media Classicに画像をアップロードする前に、画像が最高画質のサイズとフォーマットであることを確認します。 Adobe Dynamic Media Classicでは、十分な画素数（長いサイズで1500 ～ 2000 ピクセル）の高品質な画像をアップロードすることをお勧めします。 このサイズは、必要な任意のDynamic Imagingを使用できます。

画像のアップロードについて詳しくは、[ ファイルのアップロード ](uploading-files.md#uploading_files)を参照してください。

**アップロード用にプライマリ画像を準備：**

Adobe Dynamic Media Classicにアップロードする前に、プライマリ画像ファイルを準備します。

* **画像サイズ**：使用すると予想される最大サイズの画像を作成します。 一般的な画像のサイズは、1500 ～ 2500 ピクセルの範囲で、最も長いサイズになります。 ズーム機能を使用する場合は、最適なズームのディテールを得るために、Adobe Dynamic Media Classicでは、最長サイズで2000 ピクセル以上の画像を使用することをお勧めします。 Adobe Dynamic Media Classicは、1つにつき最大25 メガピクセルの画像をレンダリングできます。 例えば、5000 × 5000 MPの画像や、最大25 MPのサイズの組み合わせを使用できます。

* **ファイル形式**: Adobe Dynamic Media Classicはすべての標準的な画像ファイル形式をサポートしています。 これらのフォーマットには、TIFF、BMP、JPEG、PSD、GIF、EPSが含まれます。 ロスレス画像フォーマット（TIFFおよびPNG）をお勧めします。 JPEG画像を使用している場合は、最高画質の設定を使用します。

* **カラースペース**: RGBはWeb画像プレゼンテーション用のカラースペースです。印刷に一般的に使用されるCMYK画像は、アップロード時に自動的にRGBに変換されます。 RGBに変換する際には、ICC （International Color Consortium）カラープロファイルが組み込まれたCMYK画像をアップロードすることをお勧めします。 [ICC （International Color Consortium） プロファイル ](/help/using/icc-profiles.md)も参照してください。
