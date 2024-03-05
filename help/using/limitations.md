---
title: Dynamic Mediaの制限
description: 「画像セットやスピンセットを作成したり、画像をアップロードしたりする際の、ベストプラクティスと適用される制限について説明します。PDF また、Dynamic Mediaでサポートされていない Web ブラウザーとオペレーティングシステムの組み合わせについても説明します。」
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
source-git-commit: 0e1b2e9dcbee182f3ec0da53b56b5b8d3eb29cce
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 1%

---

# Dynamic Mediaの制限

次の節では、Dynamic Mediaの制限について説明します。

このトピックには、次の節が含まれます。

* [アセットタイプに関するDynamic Mediaのベストプラクティスと適用される制限](#best-practice-enforced-limits)
* [Dynamic Mediaでサポートされていない Web ブラウザーとオペレーティングシステムの組み合わせ](#unsupported-browser-os)

## アセットタイプに関するDynamic Mediaのベストプラクティスと適用される制限 {#best-practice-enforced-limits}

Adobeでは、ページ抽出用にスピンセットや画像セットを作成したり、PDFをアップロードしたりする際に、次のベストプラクティスを推奨し、次の制限を適用します。

| アセット — 制限タイプ | ベストプラクティス | 制限が適用されました |
| --- | --- | --- |
| **画像**  — 画像あたりのスマート切り抜きの数 | 5 | 100 |
| **すべてのセット**  — セットあたりの重複アセット数 | 重複なし | 20‡ |
| **すべてのセット**  — セットあたりの最大アセット数 | 1 セットあたり 5～10 個の画像 | 1000 |
| **スピンセット** - 2D セットあたりの最大行数/列数 | 1 セットあたり 12～18 個の画像 | 1000 |
| **PDF**  — 抽出対象となるPDFの最大ページ数 |  | 100( すべてのPDF) |

‡ベストプラクティスは、重複するアセットをセットに含めないことです。 1 つのアセットに対する重複は 20 個までに制限されます。 そのアセットに別の重複を追加した場合は、そのセット内で、リクエストがエラーを表示するか、重複を無視します。

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Dynamic Mediaでサポートされていない Web ブラウザーとオペレーティングシステムの組み合わせ {#unsupported-browser-os}

<!-- CQDOC-19433 -->

AdobeDynamic Mediaでは、次の Web ブラウザーとオペレーティングシステムの組み合わせをサポートしていません。

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Internet Explorer 11 + Windows Phone 8.1 の更新
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9 Mavericks
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 ヨセミテ

## Secure Socket Layer 2.0 および 3.0 と Transport Layer Security 1.0 および 1.1 のサポートの終了 {#tls}

<!-- CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) -->

2024 年 4 月 30 日をもって、AdobeDynamic Mediaは次のサポートを終了します。

* SSL (Secure Socket Layer) 2.0
* SSL 3.0
* TLS(Transport Layer Security)1.0 および 1.1
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

