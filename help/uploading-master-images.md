---
title: マスター画像のアップロード
description: マスター画像をアップロードする方法を説明します。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Mediaクラシック，アセット管理
role: Business Practitioner
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
translation-type: tm+mt
source-git-commit: 06bd65c92c88595786b14213944a7cebd0d2590b
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 19%

---

# マスター画像のアップロード{#uploading-master-images}

画像をDynamic Mediaクラシックにアップロードする前に、画像が最高の画質を持つサイズと形式であることを確認してください。 Dynamic Mediaクラシックでは、十分なピクセル数（長辺が1500 ～ 2000 pixelの画像）を持つ高品質の画像をアップロードすることをお勧めします。 このサイズ変更により、必要なダイナミックイメージングを行うことができます。

画像のアップロードについて詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

**マスター画像のアップロード準備:**

マスター画像ファイルは、Dynamic Mediaクラシックにアップロードする前に、次の準備を行います。

* **画像サイズ**  — 使用が予想される最大サイズの画像を作成します。一般的な画像サイズは、最長サイズが1500 ～ 2500 pixelです。 ズーム機能を使用する場合は、詳細なズームを行うために、長辺が少なくとも2000 pixelの画像を使用することをお勧めします。 Dynamic Mediaクラシックでは、それぞれ25メガピクセルまでの画像をレンダリングできます。 例えば、5000 x 5000メガピクセルの画像や、25メガピクセルまでのその他のサイズの組み合わせを使用できます。

* **ファイル形式** -Dynamic Mediaクラシックは、TIFF、BMP、JPEG、PSD、GIF、EPSを含むすべての標準画像ファイル形式をサポートしています。可逆圧縮画像形式の TIFF および PNG を使用することをお勧めします。JPEG画像を使用する場合は、最高の画質設定を使用してください。

* **カラースペース** - RGBは、Web画像表示用のカラースペースです。印刷に一般的に使用されるCMYK画像は、アップロード時に自動的にRGBに変換されます。RGB への変換用の ICC カラープロファイルが埋め込まれた CMYK 画像をアップロードすることをお勧めします。詳しくは、[ICC プロファイル](/help/icc-profiles.md)も参照してください。
