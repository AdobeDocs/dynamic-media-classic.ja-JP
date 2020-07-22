---
title: Adobe Platforms Classicプラットフォームの概要
seo-title: Adobe Platforms Classicプラットフォームの概要
description: 'null'
seo-description: Platform ClassicDynamic Mediaとワークフロープロセスの概要を示します。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 1df4f88ef856160ee06c43dc6ec430df122f2408
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 32%

---


# Adobe Platforms Classicプラットフォームの概要{#adobe-scene-platform-overview}

Dynamic Mediaクラシックは、統合されたリッチメディア管理、公開、サービング環境です。 リッチメディアは、あらゆる流通および販売経路を介して配信することができます。例えば、Web、印刷物、電子メールによる宣伝、Web ポータル、デスクトップ、デバイスを介して配信することができます。

## ワークフロープロセス {#workflow-process}

Classicの主なDynamic Media手順は次のとおりです。

* **アセットのアップロードと管理** Media Classicへのメディアアセットのアップロードを参照してください。 システム上のアセットに対して、整理、参照および検索を行うことができます。また、アセットにメタデータを適用することもできます。

* **リッチメディアの作成eCatalog、画像セット、スピンセット、スウォッチセット、混在メディアセット、基本テンプレート、FXGテンプレートなど、様々なアセット設定を**&#x200B;作成できます。 詳しくは、リッチメディアについてを参照してください。

* **アセットの公開と管理** Classic SaasDynamic Mediaへの公開、および公開時のアセットのステータス監視、ユーザ権限の管理、セキュリティの維持を行います。

* **Serve** Classic SaaSDynamic MediaからWebページ、アプリケーション、モバイルデバイスにメディアを配信します。 メディアはパフォーマンスに関して最適化されており、CDNキャッシュと共に配信されます。 Dynamic Mediaクラシックでは、各アセットのURLが提供されます。 アセットを公開すると、URL がアクティブになります。

![Dynamic Mediaクラシックワークフロープロセス](/help/assets/gs_workflow.png)

## 1 つのマスター画像と 1 回の URL 呼び出し {#single-master-images-and-single-url-calls}

Dynamic Mediaクラシックは、他のシステムとは根本的に異なります。Dynamic Mediaクラシックを使用して、1つのマスターアセットとURL呼び出しからメディアを動的に配信できるからです。

Dynamic MediaClassicで生成されるURL文字列には、アセットの配信時にアセットをどのように表示するかをサーバに指示する命令が含まれます。 例えば、1 つのマスター画像をもとに、サイズ、形式、重み、色、ズームビューをそれぞれ変えて配信させることができます。Dynamic Mediaクラシックを使用したメディアアセットの作成と公開の一環として、視覚的に効果を設定できます。 この設定を行うには、マスターアセットをアプリケーションにどのような形態で配信するのかを正しくサーバに通知する URL 呼び出しを作成します。

![Dynamic Mediaクラシックでは、同じマスター画像を様々なサイズと形式で様々な媒体に配信できます。](/help/assets/gs_dynamic_publishing.png)

## コンテンツのキャッシング {#content-caching}

Dynamic MediaClassicが動的に生成する画像は、キャッシュに優しく、 ほとんどの場合、画像はJPEG画像で、画像を識別する一意のURL呼び出しを持ちます。 画像はコンテンツ配信ネットワーク（CDN）方式で配信されます。この方式は、コンテンツ配信を高速化するために、サーバをインターネット上で相互接続する方式です。画像はグローバルに配置されたサーバ間で配信されてから、コンピュータに配信されます。CDNベンダーを使用したキャッシュメカニズムを実装する場合は、サーバー名をCDN対応Dynamic MediaのImage Serverを指すように変更します。 すべてのDynamic MediaのClassicエディションには、CDNキャッシュのバンドルが含まれています。
