---
title: Adobe Analytics レポートの表示による統合のテスト
seo-title: Adobe Analytics レポートの表示による統合のテスト
description: 'null'
seo-description: Adobe Analyticsレポートを表示して統合をテストする方法を学習します。
uuid: 937375e0-6dea-4baa- a2b0-4f3e461c9ee2
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/adobe_ analytics_ recurtion_ kit
discoiquuid: 1ddc89ff- d2e9-42eb- a442- aa6b9871c991
translation-type: tm+mt
source-git-commit: a1722c15d3c049f05959d895e85297d47d730872

---


# Adobe Analytics レポートの表示による統合のテスト{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Adobe Analyticsで必要な変数を作成して、それらをDynamic Media Classicイベントにリンクし、必要な実装手順を完了した後、セットアップをテストする必要があります。データが Adobe Analytics 内で収集されることをテストして確認できます。設定が正常に動作する場合は、それ以上の手順は必要ありません。上記の手順に従ってDynamic Media Classicイベントデータを1つ以上のカスタムトラフィック変数にリンクした場合は、このワークフローに従ってAdobe Analytics内のデータをテストします。

**Adobe Analytics レポートを表示して統合をテストするには**

1. アカウントからDynamic Media Classicビューアを起動して、特にキャプチャする指標をブロードキャストし、それを操作してイベントデータを作成します。

   例えば、画像セット内の最も人気のある代替表示を測定する場合は、画像セットをプレビューして、様々なサムネール画像をクリックします。

1. Inside Adobe Analytics, go to Custom Traffic &gt; Custom Traffic 1-10 &gt; [Name of prop], selecting your traffic prop name from the menu choices.

   例えば、サンプルアカウントで LoadAsset prop にアクセスするための適切なメニュー項目は、カスタムトラフィック／カスタムトラフィック 1～10／LoadAsset となります。カスタム prop が 11 個以上ある場合は、追加のメニュー項目も表示されます。

1. Adobe Analytics が生成したチャートを参照します。これは通常、1 つのメトリックに対するデータに過ぎません。このデータが関連付けられているアセット（50%のみに視聴されているビデオ、最も人気のあるセットの画像など）も把握したい場合は、このイベントのアセットデータも必ずキャプチャしてください。

>[!NOTE]
>
>すべてのDynamic Media Classicビューアデータは、Adobe Analyticsのカスタムトラフィックレポートまたはカスタムコンバージョンレポートに表示およびレポートされます。

For more information, see [www.adobe.com/go/learn_sc7_sitecatalystguide_en](https://www.adobe.com/go/learn_sc7_sitecatalystguide_en).
