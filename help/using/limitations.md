---
title: Dynamic Mediaの制限
description: 画像セットやスピンセットを作成したり、PDFをアップロードしたりする際のベストプラクティスと適用される制限について説明します。 Dynamic MediaでサポートされていないWeb ブラウザーとオペレーティングシステムの組み合わせについても説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/ecatalogs
feature: Dynamic Media Classic,Asset Management,Image Sets,Spin Sets,eCatalog
role: User
exl-id: ee30a2c1-2b26-41bd-8758-e7337a3727bb
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:02:23.354Z'
TQID: 'https://experienceleague.adobe.com/7dtiaPb7sWkPb5gocOc8xLOnz3U3gJuSdaW2LSkajMk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 352
ht-degree: 1%

---

# Dynamic Mediaの制限

次の節では、Dynamic Mediaの制限事項について説明します。

このトピックには、次のセクションが含まれます。

* [アセットタイプに関するDynamic Mediaによるベストプラクティスと強制された制限](#best-practice-enforced-limits)
* [Dynamic MediaでサポートされていないWeb ブラウザーとオペレーティングシステムの組み合わせ](#unsupported-browser-os)

## アセットタイプに関するDynamic Mediaによるベストプラクティスと強制された制限 {#best-practice-enforced-limits}

スピンセットまたは画像セットを作成する場合、またはページ抽出用にPDFをアップロードする場合、Adobeでは次のベストプラクティスをお勧めします。 Adobeでは、次の制限も適用されます。

| アセット：制限タイプ | ベストプラクティス | 制限が適用されました |
| --- | --- | --- |
| **画像**：画像ごとのスマート切り抜きの数 | 5 | 100 |
| **すべてのセット**: セットあたりの重複アセットの数 | 重複なし | 20‡ |
| **すべてのセット**: 1 セットあたりのアセットの最大数 | 5～10枚/セット | 1000 |
| **スピンセット**: 2D セットあたりの最大行数/列数 | 12～18枚/セット | 1000 |
| **PDF**：抽出で考慮されるPDFの最大ページ数 |  | 100 （すべてのPDF） |

‡ベストプラクティスは、セット内に重複するアセットを含めないことです。 1つのアセットに対する重複の数は20件までです。 そのセット内で、そのアセットに別の重複を追加すると、リクエストはエラーを与えるか、重複を無視します。

<!-- See also [Dynamic Media limitations](/help/using/assets/limitations.md). -->

## Dynamic MediaでサポートされていないWeb ブラウザーとオペレーティングシステムの組み合わせ {#unsupported-browser-os}

<!-- CQDOC-19433 -->

Adobe Dynamic Mediaでは、次のWeb ブラウザーとオペレーティングシステムの組み合わせはサポートされていません。

* Internet Explorer 11 + Windows 7
* Internet Explorer 11 + Windows 8.1
* Internet Explorer 11 + Windows Phone 8.1
* Internet Explorer 11 + Windows Phone 8.1 アップデート
* Safari 6 + iOS 6.0.1
* Safari 7 + iOS 7.1
* Safari 7 + OS X 10.9 Mavericks
* Safari 8 + iOS 8.4
* Safari 8 + OS X 10.10 Yosemite

## Secure Socket Layer 2.0および3.0、Transport Layer Security 1.0および1.1のサポート終了 {#tls}

<!-- 
CQDOC-19433 (original ticket)
and CQDOC-19792 (removed as per this ticket December 5, 2022) 
-->

2024年4月30日（PT）より、Adobe Dynamic Mediaは次のサポートを終了します。

* SSL （セキュアソケットレイヤー） 2.0
* SSL 3.0
* TLS （Transport Layer Security） 1.0および1.1
* TLS 1.2の以下の脆弱な暗号：
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

