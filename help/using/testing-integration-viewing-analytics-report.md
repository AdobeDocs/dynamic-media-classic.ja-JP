---
title: Adobe Analytics レポートを表示して統合をテストする
description: Adobe Analytics レポートを表示して、Adobe Dynamic Media Classicでの統合をテストする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T20:14:40.601Z'
TQID: 'https://experienceleague.adobe.com/BwQe9AuhBfi-bLCuO-j48kE-3gw9rgtz5GEI9nIBRjE'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 345
ht-degree: 5%

---

# Adobe Analytics レポートを表示して統合をテストする{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Adobe Analyticsで必要な変数を作成し、それらをAdobe Dynamic Media Classic イベントにリンクし、必要な実装手順を完了したら、設定をテストできます。 Adobe Analytics自体にデータが取り込まれていることをテストし、検証できます。 設定が正常に動作する場合は、それ以上の手順は必要ありません。 上記の手順に従い、Adobe Dynamic Media Classic イベントデータを1つ以上のカスタムトラフィック変数にリンクした場合、次のワークフローに従ってAdobe Analytics内のデータをテストします。

**Adobe Analytics レポートを表示して統合をテストするには：**

1. アカウントからAdobe Dynamic Media Classic ビューア（特に、取得する指標をブロードキャストするビューア）を開始し、操作してイベントデータを作成します。

   例えば、画像セット内の一般的な代替ビューを測定する場合は、画像セットをプレビューし、別のサムネール画像をクリックします。

1. Adobe Analytics内で、**[!UICONTROL カスタムトラフィック]** > **[!UICONTROL カスタムトラフィック 1-10]** > [ プロップの名前]に移動し、メニューの選択肢からトラフィックプロップ名を選択します。

   例えば、サンプルアカウントの&#x200B;**[!UICONTROL LoadAsset]** propにアクセスするには、適切なメニューの選択肢は&#x200B;**[!UICONTROL カスタムトラフィック]** > **[!UICONTROL カスタムトラフィック 1-10]** > **[!UICONTROL LoadAsset]**&#x200B;です。 10個を超えるカスタム propがある場合は、他のメニューの選択肢も表示されます。

1. Adobe Analytics が生成したチャートを参照します。 このグラフは通常、単一の指標のデータです。 このデータがどのアセットに関連付けられているかも知りたい場合は、このイベントのアセットデータを取得します。 例えば、どのビデオが50%しか視聴されているか、またはセット内のどの画像が人気があるかを知ることはしばしば有用です。

>[!NOTE]
>
>すべてのAdobe Dynamic Media Classic ビューアデータは、Adobe Analyticsのカスタムトラフィックレポートまたはカスタムコンバージョンレポートに表示およびレポートされます。

詳しくは、[Analytics チュートリアル &#x200B;](https://experienceleague.adobe.com/en/docs/analytics-learn/tutorials/overview)を参照してください。