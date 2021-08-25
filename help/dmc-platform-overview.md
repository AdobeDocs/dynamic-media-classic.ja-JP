---
title: AdobeDynamic Media Classicプログラムの概要
description: Dynamic Media Classicプログラムとワークフロープロセスの概要です。
uuid: e7d3bfb3-1cfe-43ea-b862-aae3b3928c71
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
discoiquuid: 2b134cfa-7f46-4f5f-959e-b30aae610bb9
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
source-git-commit: 47845c30311fb9afb3fffb8502b6e7c534e4bfdb
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 30%

---

# AdobeDynamic Media Classicプログラムの概要{#adobe-scene-platform-overview}

Dynamic Media Classicは、統合されたリッチメディア管理、公開、および提供環境です。 リッチメディアは、あらゆる流通および販売経路を介して配信することができます。例えば、Web、印刷物、電子メールによる宣伝、Web ポータル、デスクトップ、デバイスを介して配信することができます。

## ワークフロープロセス {#workflow-process}

主なDynamic Media Classicワークフロー手順は次のとおりです。

* **アセットのアップロードと管理**  - Dynamic Media Classicにメディアアセットをアップロードします。システム上のアセットに対して、整理、参照および検索を行うことができます。また、アセットにメタデータを適用することもできます。

* **リッチメディアの作成**  - eCatalog、画像セット、スピンセット、スウォッチセット、混在メディアセット、基本テンプレート、FXGテンプレートなど、アセットの様々な設定を作成します。

* **公開と管理**  - Dynamic Media Classic SaaSネットワークにアセットを公開し、公開されたアセットのステータスを監視し、ユーザー権限を管理し、セキュリティを維持します。

* **提供**  - Dynamic Media Classic SaaSネットワークからWebページ、アプリケーション、モバイルデバイスにメディアを配信する。メディアはパフォーマンスに最適化され、CDNキャッシュと共に配信されます。Dynamic Media Classicには、各アセットのURLが表示されます。 アセットを公開すると、URL がアクティブになります。

![Dynamic Media Classicのワークフロープロセス](/help/assets/gs_workflow.png)

## 1 つのマスター画像と 1 回の URL 呼び出し {#single-master-images-and-single-url-calls}

Dynamic Media Classicは、単一のマスターアセットおよびURL呼び出しから動的にメディアを配信できるので、他のシステムとは根本的に異なります。

Dynamic Media Classicで生成されるURL文字列には、アセットの配信時の表示方法をサーバーに伝える手順が含まれます。 例えば、1 つのマスター画像をもとに、サイズ、形式、重み、色、ズームビューをそれぞれ変えて配信させることができます。Dynamic Media Classicを使用したメディアアセットの構築と公開の一環として、効果を視覚的に設定できます。 この設定を行うには、マスターアセットをアプリケーションにどのような形態で配信するのかを正しくサーバに通知する URL 呼び出しを作成します。

![Dynamic Media Classicは、サイズと形式が異なる異なるメディアに同じマスター画像を配信できます。](/help/assets/gs_dynamic_publishing.png)
*Dynamic Media Classicを使用すると、サイズや帯域幅に関係なく、一貫性のある高品質のエクスペリエンスをあらゆる画面に配信できます。*

## コンテンツのキャッシング {#content-caching}

Dynamic Media Classicが動的に生成する画像は、キャッシュに適しています。通常、これらは一意のURL呼び出しで識別されるJPEG画像です。 画像はコンテンツ配信ネットワーク（CDN）方式で配信されます。この方式は、コンテンツ配信を高速化するために、サーバをインターネット上で相互接続する方式です。画像はグローバルに配置されたサーバ間で配信されてから、コンピュータに配信されます。任意のCDNベンダーを使用してキャッシュメカニズムを実装する場合は、サーバー名をCDN対応のDynamic Media Image Serverを指すように変更するだけです。 すべてのDynamic Media Classicエディションには、CDNキャッシュのバンドルが含まれています。
