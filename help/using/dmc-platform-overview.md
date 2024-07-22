---
title: Adobe Dynamic Media Classic プログラムの概要
description: Adobe Dynamic Media Classic プログラムとそのワークフロープロセス全体の概要です。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/getting_started
feature: Dynamic Media Classic
role: Admin,User
exl-id: ac50cb9c-fd87-4608-80cb-8d40a0b8f131
topic: Administration
level: Beginner
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 12%

---

# Adobe Dynamic Media Classic プログラムの概要{#adobe-scene-platform-overview}

Adobe Dynamic Media Classicは、統合されたリッチメディア管理、公開および提供環境です。 リッチメディアは、すべてのマーケティングチャネルと販売チャネルに配信できます。 これらのチャネルには、Web、印刷資料、メールキャンペーン、Web ポータル、デスクトップ、デバイスなどがあります。

[Platform の概要 ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/572_Platform%20Overview_converted%20renamed_Getting%20Started-AVS) トレーニングビデオも参照してください。

## ワークフロープロセス {#workflow-process}

Adobe Dynamic Media Classicの主なワークフロー手順は次のとおりです。

* **アセットのアップロードと管理**：メディアアセットをAdobe Dynamic Media Classicにアップロードします。 システム上のアセットに対して、整理、参照および検索を行うことができます。アセットにメタデータを適用することもできます。

* **リッチメディアの作成**:eCatalog、画像セット、スピンセット、スウォッチセット、混在メディアセット、基本テンプレート、FXG テンプレートなど、アセットの様々な設定を作成します。

* **Publishと管理**:Publish Assets をAdobe Dynamic Media Classic SaaS ネットワークに追加します。 アセットの公開時のステータスの監視 ユーザー権限の管理とセキュリティの維持。

* **サービス**:Adobe Dynamic Media Classic SaaS Network から web ページ、アプリケーション、モバイルデバイスにメディアを配信します。メディアはパフォーマンスが最適化され、CDN キャッシングで配信されます。 Adobe Dynamic Media Classicは各アセットの URL を提供します。 アセットを公開すると、URL がアクティブになります。

![Adobe Dynamic Media Classic ワークフロープロセス ](/help/using/assets/gs_workflow.png)

## 単一のプライマリ画像と単一の URL 呼び出し {#single-master-images-and-single-url-calls}

Adobe Dynamic Media Classicは他のシステムとは基本的に異なり、Adobe Dynamic Media Classicを使用して、1 つのプライマリアセットおよび URL 呼び出しから動的にメディアを配信できます。

Adobe Dynamic Media Classicで生成した URL 文字列には、配信時にアセットを表示する方法をサーバーに指示する命令が含まれています。 例えば、同じプライマリ画像を異なるサイズ、形式、重み、カラーおよびズームビューで配信することができます。 Adobe Dynamic Media Classicを使用したメディアアセットの作成と公開の一環として、効果を視覚的に設定できます。 その際に、プライマリアセットをアプリケーションに表示する方法をサーバーに正しく指示する URL 呼び出しを作成します。

![Adobe Dynamic Media Classicは、同じプライマリ画像を異なるメディアに、異なるサイズおよび形式で配信できます。](/help/using/assets/gs_dynamic_publishing.png)
*Adobe Dynamic Media Classicでは、サイズや帯域幅に関係なく、一貫性のある高品質なエクスペリエンスをあらゆる画面に確実に配信します。*

## コンテンツのキャッシング {#content-caching}

Adobe Dynamic Media Classicが動的に生成する画像は、キャッシュに適しています。通常、画像は、画像を識別する一意の URL 呼び出しを持つJPEG画像です。 画像はコンテンツ配信ネットワーク（CDN）方式で配信されます。この方式は、コンテンツ配信を高速化するために、サーバをインターネット上で相互接続する方式です。画像はグローバルに配置されたサーバ間で配信されてから、コンピュータに配信されます。任意の CDN ベンダーを使用してキャッシュメカニズムを実装する場合は、サーバー名を変更して CDN 対応のDynamic Media Image Server を指すようにするだけです。 すべてのAdobe Dynamic Media Classic エディションには、バンドルされた CDN キャッシングが含まれています。
