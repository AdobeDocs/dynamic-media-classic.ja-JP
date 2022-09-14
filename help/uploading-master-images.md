---
title: プライマリ画像のアップロード
description: プライマリ画像をAdobe Dynamic Media Classicにアップロードする方法を説明します。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
source-git-commit: cb55e09a997b9d36002c4ac429603576d52fb8bd
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 2%

---

# プライマリ画像のアップロード{#uploading-master-images}

画像をAdobe Dynamic Media Classicにアップロードする前に、画像が最高品質のサイズと形式であることを確認してください。 Adobe Dynamic Media Classicでは、十分なピクセル数（長さが 1,500 ～ 2,000 ピクセル）を持つ高品質な画像をアップロードすることをお勧めします。 このサイズ設定により、必要なDynamic Imagingを設定できます。

画像のアップロードについて詳しくは、 [ファイルをアップロード](uploading-files.md#uploading_files).

**アップロード用のプライマリ画像を準備する：**

プライマリ画像ファイルをAdobe Dynamic Media Classicにアップロードする前に、次の手順で準備します。

* **画像サイズ**  — 使用すると予想される最大サイズの画像を作成します。 一般的な画像サイズの範囲は、最長 1500 ～ 2500 ピクセルです。 ズーム機能を使用する場合、最適なズーム詳細を得るために、最長サイズで 2,000 ピクセル以上の画像を使用することをお勧めします。 Adobe Dynamic Media Classicでは、それぞれ最大 25 メガピクセルの画像をレンダリングできます。 例えば、5000 x 5000 MP の画像や、その他のサイズの組み合わせを最大 25 MP まで使用できます。

* **ファイル形式** - Adobe Dynamic Media Classicは、TIFF、BMP、JPEG、PSD、GIF、EPSを含むすべての標準的な画像ファイル形式をサポートしています。 可逆圧縮画像形式の TIFF および PNG を使用することをお勧めします。JPEG画像を使用する場合は、最高品質の設定を使用します。

* **色空間** -RGBは、Web 画像プレゼンテーション用のカラースペースです。印刷に一般的に使用される CMYK 画像は、アップロード時にRGBに自動的に変換されます。 RGBへの変換用に、埋め込み ICC(International Color Consortium) カラープロファイルを持つ CMYK 画像をアップロードすることをお勧めします。 関連トピック [ICC(International Color Consortium) プロファイル](/help/icc-profiles.md).
