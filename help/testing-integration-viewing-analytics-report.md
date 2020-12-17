---
title: Adobe Analytics レポートの表示による統合のテスト
seo-title: Adobe Analytics レポートの表示による統合のテスト
description: 'null'
seo-description: Adobe Analyticsレポートを表示して統合をテストする方法を学習します。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 42%

---


# Adobe Analytics レポートの表示による統合のテスト{#testing-the-integration-by-viewing-an-adobe-analytics-report}

必要な変数をAdobe Analyticsで作成し、それらの変数をDynamic Mediaクラシックイベントにリンクし、必要な実装手順を完了した後、設定をテストする必要があります。 データが Adobe Analytics 内で収集されることをテストして確認できます。設定が正常に動作する場合は、それ以上の手順は必要ありません。上記の手順に従って、Dynamic Mediaクラシックイベントデータを1つ以上のカスタムトラフィック変数にリンクしたと仮定し、次のワークフローに従ってAdobe Analytics内のデータをテストします。

**Adobe Analytics レポートを表示して統合をテストするには**

1. アカウントからDynamic Mediaクラシックビューアを起動し、特に、取り込む指標をブロードキャストするビューアを起動し、このビューアを操作してイベントデータを作成します。

   例えば、画像セット内の最も人気のある代替表示を測定する場合は、画像セットをプレビューして、様々なサムネール画像をクリックします。

1. Adobe Analytics内で、カスタムトラフィック/カスタムトラフィック1-10/[prop]の名前に移動し、メニュー項目から適切なトラフィックprop名を選択します。

   例えば、サンプルアカウントで LoadAsset prop にアクセスするための適切なメニュー項目は、カスタムトラフィック／カスタムトラフィック 1～10／LoadAsset となります。カスタム prop が 11 個以上ある場合は、追加のメニュー項目も表示されます。

1. Adobe Analytics が生成したチャートを参照します。これは通常、1 つのメトリックに対するデータに過ぎません。このデータが関連付けられているアセット(50%のみに視聴されているビデオや、最も人気のあるセット内のイベントなど)も把握したい場合は、この画像のアセットデータも必ず取り込んでください。

>[!NOTE]
>
>すべてのDynamic Mediaクラシックビューアのデータは、Adobe Analyticsのカスタムトラフィックレポートまたはカスタムコンバージョンレポートに表示およびレポートされます。

詳しくは、[www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en)を参照してください。
