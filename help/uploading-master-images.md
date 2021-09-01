---
title: マスター画像のアップロード
description: マスター画像をDynamic Media Classicにアップロードする方法をAdobeします。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 2%

---

# マスター画像のアップロード{#uploading-master-images}

画像をDynamic Media ClassicにAdobeにアップロードする前に、画像が最高品質のサイズと形式であることを確認してください。 AdobeDynamic Media Classicでは、十分なピクセル数（長さが1,500～2,000ピクセル）を持つ高品質の画像をアップロードすることをお勧めします。 このサイズ設定により、必要なDynamic Imagingを設定できます。

画像のアップロードについて詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

**アップロード用のマスター画像を準備します。**

マスター画像ファイルをAdobeDynamic Media Classicにアップロードする前に、次の手順で準備します。

* **画像サイズ**  — 使用が予想される最大サイズの画像を作成します。一般的な画像サイズの範囲は、最長で1500 ～ 2500ピクセルです。 ズーム機能を使用する場合、最適なズーム詳細を得るために、最長で2,000ピクセル以上の画像をAdobeDynamic Media Classicで使用することをお勧めします。 AdobeDynamic Media Classicでは、それぞれ最大25メガピクセルの画像をレンダリングできます。 例えば、5000 x 5000 MPの画像や、その他のサイズの組み合わせを最大25 MPで使用できます。

* **ファイル形式**  -AdobeDynamic Media Classicは、TIFF、BMP、JPEG、PSD、GIF、EPSを含む、すべての標準的な画像ファイル形式をサポートします。可逆圧縮画像形式の TIFF および PNG を使用することをお勧めします。JPEG画像を使用する場合は、最高画質の設定を使用します。

* **カラースペース** - RGBは、Web画像プレゼンテーション用のカラースペースです。印刷に一般的に使用されるCMYK画像は、アップロード時にRGBに自動的に変換されます。RGBに変換するICC(International Color Consortium)カラープロファイルが埋め込まれたCMYK画像をアップロードすることをお勧めします。 [ICC(International Color Consortium)のプロファイル](/help/icc-profiles.md)も参照してください。
