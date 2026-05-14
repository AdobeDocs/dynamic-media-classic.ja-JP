---
title: Adobe Dynamic Media Classicプログラムの概要
description: Adobe Dynamic Media Classicプログラムとそのワークフロープロセス全体の概要。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
autotag-review: '2026-05-13T19:46:13.313Z'
TQID: 'https://experienceleague.adobe.com/qaWxQCcT9VjPt4MmahAR3-voOpUBjYztzNFXSZG6R6k'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 524
ht-degree: 12%

---

# Adobe Dynamic Media Classicプログラムの概要{#adobe-scene-platform-overview}

Adobe Dynamic Media Classicは、コンテンツの制作、編集、配信を一元管理できるリッチメディア管理システムです。 リッチメディアは、あらゆるマーケティングチャネルと販売チャネルに配信できます。 これらのチャネルには、web、印刷物、電子メールキャンペーン、web ポータル、デスクトップ、デバイスなどが含まれます。

[&#x200B; プラットフォームの概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS)のトレーニングビデオも参照してください。

## ワークフロープロセス {#workflow-process}

Adobe Dynamic Media Classicの主なワークフロー手順は次のとおりです。

* **アセットのアップロードと管理**：メディアアセットをAdobe Dynamic Media Classicにアップロードします。 システム上のアセットに対して、整理、参照および検索を行うことができます。 また、アセットにメタデータを適用することもできます。

* **リッチメディアの作成**：電子カタログ、画像セット、スピンセット、スウォッチセット、混在メディアセット、基本テンプレート、FXG テンプレートなど、アセットのさまざまな設定を作成します。

* **公開と管理**: アセットをAdobe Dynamic Media Classic SaaS ネットワークに公開します。 公開時にアセットのステータスを監視します。 ユーザーの権利を管理し、セキュリティを維持します。

* **サービス**: Adobe Dynamic Media Classic SaaS ネットワークからWeb ページ、アプリケーション、モバイルデバイスにメディアを配信します。メディアはパフォーマンスが最適化されており、CDN キャッシュで配信されます。 Adobe Dynamic Media Classicには、各アセットのURLが表示されます。 アセットを公開すると、URL がアクティブになります。

![Adobe Dynamic Media Classic ワークフロープロセス &#x200B;](/help/using/assets/gs_workflow.png)

## 単一プライマリ画像と単一URL呼び出し {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classicは、Adobe Dynamic Media Classicを使用して、1つのプライマリアセットとURL呼び出しから動的にメディアを配信できるため、他のシステムとは根本的に異なります。

Adobe Dynamic Media Classicで生成したURL文字列には、配信時にアセットを表示する方法をサーバーに伝える指示が含まれています。 例えば、同じプライマリ画像を、サイズ、形式、重み、色、ズームビューごとに配信できます。 Adobe Dynamic Media Classicを使用したメディアアセットの作成と公開の一環として、効果を視覚的に設定できます。 これにより、プライマリアセットをアプリケーションに表示する方法をサーバーに正しく伝えるURL呼び出しを作成します。

![Adobe Dynamic Media Classicは、異なるサイズや形式の異なるメディアに同じプライマリ画像を配信できます。](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classicを使用すると、サイズや帯域幅に関係なく、あらゆる画面に一貫性のある質の高いエクスペリエンスを確実に配信できます。*

## コンテンツのキャッシング {#content-caching}

Adobe Dynamic Media Classicが動的に生成する画像は、キャッシュに適しています。通常、これらの画像は、一意のURL呼び出しを持つJPEG画像です。 画像はコンテンツ配信ネットワーク（CDN）方式で配信されます。この方式は、コンテンツ配信を高速化するために、サーバをインターネット上で相互接続する方式です。 画像はグローバルに配置されたサーバ間で配信されてから、コンピュータに配信されます。 任意のCDN ベンダーを使用してキャッシュメカニズムを実装する場合は、CDN対応のDynamic Media Image Serverを指すようにサーバー名を変更するだけです。 すべてのAdobe Dynamic Media Classicエディションには、バンドルされたCDN キャッシュが含まれています。
