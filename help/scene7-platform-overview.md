---
title: Adobe Dynamic Media Classicプラットフォームの概要
seo-title: Adobe Dynamic Media Classicプラットフォームの概要
description: 'null'
seo-description: Dynamic Media Classicプラットフォームとワークフロープロセスの概要です。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# Adobe Dynamic Media Classicプラットフォームの概要{#adobe-scene-platform-overview}

Dynamic Media Classicは、統合されたリッチメディア管理、公開、および提供環境です。 リッチメディアは、あらゆる流通および販売経路を介して配信することができます。例えば、Web、印刷物、電子メールによる宣伝、Web ポータル、デスクトップ、デバイスを介して配信することができます。

## ワークフロープロセス {#workflow-process}

Dynamic Media Classicの主なワークフロー手順は次のとおりです。

* **アセットのアップロードと管理** SPSへのメディアアセットのアップロード。 システム上のアセットに対して、整理、参照および検索を行うことができます。また、アセットにメタデータを適用することもできます。Adobe Scene7 Publishing System デスクトップアプリケーションをインストールすると、ファイルやフォルダをデスクトップからアップロードフォルダにドラッグすることでアップロードできます。

* **リッチメディア**&#x200B;の作成eCatalog、画像セット、スピンセット、スウォッチセット、混在メディアセット、基本テンプレート、FXGテンプレートなど、様々なアセットの設定を作成します。 詳しくは、リッチメディアについてを参照してください。

* **Dynamic Media Classic Saas**&#x200B;ネットワークに対するアセットの公開と管理、およびアセットの公開時のステータスの監視、ユーザ権限の管理、セキュリティの維持を行います。

* **Dynamic Media** Classic SaaSネットワークからWebページ、アプリケーションおよび携帯端末にメディアを配信する。メディアはパフォーマンスに最適化され、CDNキャッシュと共に配信されます。 Dynamic Media Classicでは、各アセットのURLが提供されます。 アセットを公開すると、URL がアクティブになります。

![Dynamic Media Classicのワークフロープロセス](/help/assets/gs_workflow.png)

## 1 つのマスター画像と 1 回の URL 呼び出し {#single-master-images-and-single-url-calls}

Dynamic Media Classicは、他のシステムとは根本的に異なります。これは、Dynamic Media Classicを使用して、単一のマスターアセットやURL呼び出しからメディアを動的に配信できるからです。

Dynamic Media Classicで生成するURL文字列には、アセットの配信時にアセットをどのように表示するかをサーバーに指示する命令が含まれます。 例えば、1 つのマスター画像をもとに、サイズ、形式、重み、色、ズームビューをそれぞれ変えて配信させることができます。Dynamic Media Classicでメディアアセットを作成および公開する際に、効果を視覚的に設定します。 この設定を行うには、マスターアセットをアプリケーションにどのような形態で配信するのかを正しくサーバに通知する URL 呼び出しを作成します。

![Dynamic Media Classicは、同じマスター画像を異なるサイズや形式の異なるメディアに配信できます。](/help/assets/gs_dynamic_publishing.png)

## コンテンツのキャッシング {#content-caching}

Dynamic Media Classicで動的に生成される画像は、キャッシュに適した形式です。ほとんどの場合、これらはJPEG画像を識別する一意のURL呼び出しを持つJPEG画像です。 画像はコンテンツ配信ネットワーク（CDN）方式で配信されます。この方式は、コンテンツ配信を高速化するために、サーバをインターネット上で相互接続する方式です。画像はグローバルに配置されたサーバ間で配信されてから、コンピュータに配信されます。CDNベンダーを使用してキャッシュメカニズムを実装する場合は、CDNが有効なダイナミックメディアイメージサーバーを指すようにサーバー名を変更します。 すべてのDynamic Media Classicエディションには、CDNキャッシュのバンドルが含まれています。
