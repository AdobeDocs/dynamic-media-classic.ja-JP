---
title: Adobe Dynamic Media Classicプログラムの概要
description: Adobe Dynamic Media Classicプログラムとそのワークフロープロセス全体の概要です。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 17%

---

# Adobe Dynamic Media Classicプログラムの概要{#adobe-scene-platform-overview}

Adobe Dynamic Media Classicは、統合されたリッチメディア管理、公開、および提供環境です。 リッチメディアは、あらゆる流通および販売経路を介して配信することができます。例えば、Web、印刷物、電子メールによる宣伝、Web ポータル、デスクトップ、デバイスを介して配信することができます。

関連トピック [Platform の概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) トレーニングビデオ。

## ワークフロープロセス {#workflow-process}

主なAdobe Dynamic Media Classicワークフロー手順は次のとおりです。

* **アセットのアップロードと管理**  — メディアアセットをAdobe Dynamic Media Classicにアップロードします。 システム上のアセットに対して、整理、参照および検索を行うことができます。また、アセットにメタデータを適用することもできます。

* **リッチメディアの作成** - eCatalog、画像セット、スピンセット、スウォッチセット、混在メディアセット、基本テンプレート、FXG テンプレートなど、アセットの様々な設定を作成します。

* **公開と管理**  — アセットをAdobe Dynamic Media Classic SaaS ネットワークに公開します。 アセットが公開された際のステータスを監視します。 ユーザー権限の管理とセキュリティの維持。

* **提供** - Adobe Dynamic Media Classic SaaS ネットワークから Web ページ、アプリケーション、モバイルデバイスにメディアを配信するメディアはパフォーマンスに最適化されており、CDN キャッシュと共に配信されます。 Adobe Dynamic Media Classicには、各アセットの URL が表示されます。 アセットを公開すると、URL がアクティブになります。

![Adobe Dynamic Media Classicワークフロープロセス](/help/using/assets/gs_workflow.png)

## 単一のプライマリ画像と単一の URL 呼び出し {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classicは他のシステムとは根本的に異なります。単一のプライマリアセットと URL 呼び出しから動的にメディアを配信するためにAdobe Dynamic Media Classicを使用できるからです。

Adobe Dynamic Media Classicで生成する URL 文字列には、アセットが配信されたときの表示方法をサーバーに伝える手順が含まれています。 例えば、同じプライマリ画像を異なるサイズ、形式、重み、色、ズームビューで配信できます。 Adobe Dynamic Media Classicを使用したメディアアセットの構築と公開の一環として、効果を視覚的に設定します。 その際に、プライマリアセットをアプリケーションに提示する方法をサーバーに正しく伝える URL 呼び出しを作成します。

![Adobe Dynamic Media Classicは、異なるサイズと形式で、異なるメディアに同じプライマリ画像を配信できます。](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classicでは、サイズや帯域幅に関係なく、一貫性のある高品質なエクスペリエンスをあらゆる画面に配信できます。*

## コンテンツのキャッシング {#content-caching}

Adobe Dynamic Media Classicが動的に生成する画像は、キャッシュに適しています。通常は、JPEGを識別する一意の URL 呼び出しを持つ画像です。 画像はコンテンツ配信ネットワーク（CDN）方式で配信されます。この方式は、コンテンツ配信を高速化するために、サーバをインターネット上で相互接続する方式です。画像はグローバルに配置されたサーバ間で配信されてから、コンピュータに配信されます。任意の CDN ベンダーを使用してキャッシュメカニズムを実装する場合は、CDN が有効なDynamic Media Image Server を指すようにサーバー名を変更するだけです。 すべてのAdobe Dynamic Media Classicエディションには、バンドルされた CDN キャッシュが含まれています。
