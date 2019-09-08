---
title: Adobe Dynamic Media Classicプラットフォームの概要
seo-title: Adobe Dynamic Media Classicプラットフォームの概要
description: 'null'
seo-description: Dynamic Media Classicプラットフォームとワークフロープロセスの概要です。
uuid: e7d3bfb3-1cfe-43ea- b862- aae3b3928c71
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/getting_ started
discoiquuid: 2b134cfa-7f46-4f5f-959e- b30aae610bb9
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Adobe Dynamic Media Classicプラットフォームの概要{#adobe-scene-platform-overview}

リッチメディアは、あらゆる流通および販売経路を介して配信することができます。例えば、Web、印刷物、電子メールによる宣伝、Web ポータル、デスクトップ、デバイスを介して配信することができます。

## ワークフロープロセス {#workflow-process}

Dynamic Media Classicの主要なワークフロー手順は次のとおりです。

**アセット** のアップロードと管理を参照してください。システム上のアセットに対して、整理、参照および検索を行うことができます。また、アセットにメタデータを適用することもできます。Adobe Scene7 Publishing System デスクトップアプリケーションをインストールすると、ファイルやフォルダをデスクトップからアップロードフォルダにドラッグすることでアップロードできます。

**リッチメディア** の作成eCatalog、画像セット、スピンセット、スウォッチセット、混在メディアセット、基本テンプレート、FXGテンプレートなど、様々なアセットの構成を作成できます。詳しくは、リッチメディアについてを参照してください。

**Publish and administer** Publish assets to the Dynamic Media Classic Saas network, as well as monitor the status of assets when they are published, administer user rights, and maintain security.

**提供:** Dynamic Media Classic SaaSネットワークからWebページ、アプリケーション、モバイルデバイスへのメディア配信メディアはパフォーマンスに最適化され、CDNキャッシングで配信されます。Dynamic Media Classicには、各アセットのURLが表示されます。アセットを公開すると、URL がアクティブになります。

![Dynamic Media Classicワークフロープロセス](/help/assets/gs_workflow.png)

## 1 つのマスター画像と 1 回の URL 呼び出し {#single-master-images-and-single-url-calls}

Dynamic Media Classicは、他のシステムとは根本的に異なります。これは、Dynamic Media Classicを使用して、単一のマスターアセットやURL呼び出しからメディアを動的に配信できるからです。

Dynamic Media Classicで生成するURL文字列には、アセットを配信するときにサーバに表示されるように指示する命令が含まれています。例えば、1 つのマスター画像をもとに、サイズ、形式、重み、色、ズームビューをそれぞれ変えて配信させることができます。Dynamic Media Classicを使用してメディアアセットを作成および公開する過程で、効果を視覚的に設定できます。この設定を行うには、マスターアセットをアプリケーションにどのような形態で配信するのかを正しくサーバに通知する URL 呼び出しを作成します。

![Dynamic Media Classicでは、様々なサイズや形式の様々なメディアに同じマスター画像を配信できます。](/help/assets/gs_dynamic_publishing.png)

## コンテンツのキャッシング {#content-caching}

Dynamic Media Classicで動的に生成される画像は、キャッシュにわかりやすいものです。ほとんどの場合、それらを識別する一意のURL呼び出しを持つJPEG画像です。画像はコンテンツ配信ネットワーク（CDN）方式で配信されます。この方式は、コンテンツ配信を高速化するために、サーバをインターネット上で相互接続する方式です。画像はグローバルに配置されたサーバ間で配信されてから、コンピュータに配信されます。CDNベンダーを使用してキャッシュメカニズムを実装する場合、サーバー名をCDN対応のダイナミックメディアImage Serverを指すように変更するだけです。すべてのDynamic Media Classicエディションには、CDNキャッシュがバンドルされています。
