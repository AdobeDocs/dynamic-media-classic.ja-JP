---
title: Dynamic Mediaの制限
description: 画像セットやスピンセットを作成したり、PDFをアップロードしたりする際の、ベストプラクティスと適用される制限について説明します。 また、Dynamic Mediaでサポートしていない web ブラウザーとオペレーティングシステムの組み合わせについても説明します。」
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 1%

---

# Dynamic Mediaの制限

次の節では、Dynamic Mediaの制限について説明します。

このトピックには、次のセクションが含まれます。

* [アセットタイプに関するDynamic Mediaのベストプラクティスと適用される制限](#best-practice-enforced-limits)
* [Dynamic Mediaでサポートしていない web ブラウザーとオペレーティングシステムの組み合わせ](#unsupported-browser-os)

## アセットタイプに関するDynamic Mediaのベストプラクティスと適用される制限 {#best-practice-enforced-limits}

スピンセットや画像セットを作成したり、ページ抽出用にPDFをアップロードしたりする場合、Adobeでは次のベストプラクティスを推奨します。 Adobeでは、次の制限も適用されます。

| アセット：制限タイプ | ベストプラクティス | 適用される制限 |
| --- | --- | --- |
| **画像**：画像あたりのスマート切り抜き数 | 5 | 100 |
| **すべてのセット**:1 セットあたりの重複アセット数 | 重複なし | 20‡ |
| **すべてのセット**:1 セットあたりの最大アセット数 | 1 セットあたり 5～10 個の画像 | 1000 |
| **スピンセット**:2D セットあたりの最大行数/列数 | 1 セットあたり 12～18 個の画像 | 1000 |
| **PDF**：抽出対象となるPDFの最大ページ数 |  | 100 （すべてのPDF用） |

‡セットに重複したアセットを含めないでください。 1 つのアセットに対する重複の上限は 20 個です。 そのアセットに対して別の重複を（そのセット内で）追加した場合、リクエストでエラーが発生するか、重複が無視されます。

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Dynamic Mediaでサポートしていない web ブラウザーとオペレーティングシステムの組み合わせ {#unsupported-browser-os}

<!-- CQDOC-19433 -->

AdobeDynamic Mediaでは、次の web ブラウザーとオペレーティングシステムの組み合わせをサポートしていません。

* Internet Explorer 11 と Windows 7
* Internet Explorer 11 と Windows 8.1
* Internet Explorer 11 と Windows Phone 8.1
* Internet Explorer 11 と Windows Phone 8.1 Update
* Safari 6 とiOS 6.0.1
* Safari 7 とiOS 7.1
* Safari 7 と OS X 10.9 Mavericks
* Safari 8 とiOS 8.4
* Safari 8 と OS X 10.10 Yosemite

## Secure Socket Layer 2.0 および 3.0 と Transport Layer Security 1.0 および 1.1 のサポート終了 {#tls}

<!-- CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) -->

2024 年 4 月 30 日（PT）より、AdobeDynamic Mediaは、以下のサポートを終了します。

* SSL （Secure Socket Layer） 2.0
* SSL 3.0
* TLS （Transport Layer Security） 1.0 および 1.1
* TLS 1.2 での以下の脆弱な暗号：
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384`
   * `TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_RSA_WITH_AES_256_GCM_SHA384`
   * `TLS_RSA_WITH_AES_256_CBC_SHA256`
   * `TLS_RSA_WITH_AES_256_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_AES_128_GCM_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA256`
   * `TLS_RSA_WITH_AES_128_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_256_CBC_SHA`
   * `TLS_RSA_WITH_CAMELLIA_128_CBC_SHA`
   * `TLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHA`
   * `TLS_RSA_WITH_SDES_EDE_CBC_SHA`

