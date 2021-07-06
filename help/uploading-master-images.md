---
title: マスター画像のアップロード
description: マスター画像をアップロードする方法を説明します。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
feature: Dynamic Media Classic，アセット管理
role: User
exl-id: 410ba80c-7f01-4cd0-9ab3-db9658757ba7
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 19%

---

# マスター画像のアップロード{#uploading-master-images}

Dynamic Media Classicに画像をアップロードする前に、画像が最高品質のサイズと形式であることを確認してください。 Dynamic Media Classicでは、十分なピクセル数（長さが1,500～2,000ピクセル）で高品質の画像をアップロードすることをお勧めします。 このサイズ設定により、必要なあらゆるダイナミックイメージングが可能になります。

画像のアップロードについて詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

**マスター画像のアップロード準備:**

マスター画像ファイルをDynamic Media Classicにアップロードする前に、次の手順で準備します。

* **画像サイズ**  — 使用が予想される最大サイズの画像を作成します。一般的な画像サイズの範囲は、最長で1500 ～ 2500ピクセルです。 ズーム機能を使用する場合、最適なズーム詳細を得るために、最も長いサイズで2,000ピクセル以上の画像を使用することをお勧めします。 Dynamic Media Classicでは、それぞれ最大25メガピクセルの画像をレンダリングできます。 例えば、5,000 x 5,000メガピクセルの画像や、その他のサイズの組み合わせを25メガピクセルまで使用できます。

* **ファイル形式**  - Dynamic Media Classicは、TIFF、BMP、JPEG、PSD、GIF、EPSを含む、すべての標準的な画像ファイル形式をサポートします。可逆圧縮画像形式の TIFF および PNG を使用することをお勧めします。JPEG画像を使用する場合は、最高画質の設定を使用します。

* **カラースペース** - RGBは、Web画像プレゼンテーション用のカラースペースです。印刷に一般的に使用されるCMYK画像は、アップロード時にRGBに自動的に変換されます。RGB への変換用の ICC カラープロファイルが埋め込まれた CMYK 画像をアップロードすることをお勧めします。詳しくは、[ICC プロファイル](/help/icc-profiles.md)も参照してください。
