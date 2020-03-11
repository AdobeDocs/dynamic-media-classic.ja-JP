---
title: マスター画像のアップロード
seo-title: マスター画像のアップロード
description: 'null'
seo-description: マスター画像をアップロードする方法を説明します。
uuid: 50bcf2e2-852b-48f1-a7c7-5063a87ce9c1
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: 8c94bafc-94cc-496f-a394-a945cd7b02cf
translation-type: tm+mt
source-git-commit: dfe86e040d0acc3135fcb596c85867f2d55d9090

---


# マスター画像のアップロード{#uploading-master-images}

Scene7 Publishing System に画像をアップロードする前に、画像が最も優れた画質を得られるサイズと形式であることを確認してください。Dynamic Media Classicでは、十分なピクセル数（長辺が1500 ～ 2000 pixel）の高品質な画像をアップロードすることをお勧めします。 これにより、あらゆるダイナミックイメージングに対応できます。

画像のアップロードについて詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

**マスター画像のアップロード準備**

Scene7 Publishing System にアップロードする前に、次の要件を満たすようにマスター画像ファイルを準備します。

* **画像サイズ**&#x200B;使用する予定の最大サイズの画像を作成します。 一般的な画像サイズは、長辺が 1500 ～ 2500 pixel です。ズーム機能を使用する場合は、ズームの詳細を最適化するために、長辺が少なくとも2000ピクセルの画像を使用することをお勧めします。 Dynamic Media Classicでは、各画像を最大25メガピクセルまでレンダリングできます。 例えば、5000 x 5000メガピクセルの画像や、その他のサイズの組み合わせを25メガピクセルまで使用できます。

* **ファイル形式** Dynamic Media Classicは、TIFF、BMP、JPEG、PSD、GIF、EPSなど、すべての標準的な画像ファイル形式をサポートしています。 可逆圧縮画像形式の TIFF および PNG を使用することをお勧めします。JPEG 画像を使用する場合は、最高の画質設定を使用してください。

* **カラースペース** RGBは、Web画像表示用のカラースペースです。印刷に一般的に使用されるCMYK画像は、アップロード時に自動的にRGBに変換されます。 RGB への変換用の ICC カラープロファイルが埋め込まれた CMYK 画像をアップロードすることをお勧めします。詳しくは、ICC プロファイルも参照してください。
