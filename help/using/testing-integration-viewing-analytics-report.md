---
title: Adobe Analytics レポートを表示して統合をテスト
description: Adobe Analytics レポートを表示してAdobe Dynamic Media Classicの統合をテストする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
topic: Integrations, Development
level: Experienced
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 5%

---

# Adobe Analytics レポートを表示して統合をテスト{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Adobe Analyticsで必要な変数を作成し、Adobe Dynamic Media Classic イベントにリンクして、必要な実装手順を完了したら、設定をテストできます。 データがAdobe Analytics自体の中に取り込まれていることをテストし、検証できます。 設定が正常に動作する場合は、それ以上の手順は必要ありません。上記の手順に従い、Adobe Dynamic Media Classic イベントデータを 1 つ以上のカスタムトラフィック変数にリンクしたとすると、このワークフローに従って、Adobe Analytics内のデータをテストします。

**Adobe Analytics レポートを表示して統合をテストするには：**

1. アカウント、特に、取得する指標をブロードキャストするアカウントからAdobe Dynamic Media Classic ビューアを開始し、そのビューアを操作してイベントデータを作成します。

   例えば、画像セットの一般的な代替ビューを測定する場合は、画像セットをプレビューし、異なるサムネール画像をクリックします。

1. Adobe Analytics内で、**[!UICONTROL カスタムトラフィック]**/**[!UICONTROL カスタムトラフィック 1～10]**/[prop の名前 ] に移動し、メニュー選択からトラフィック prop 名を選択します。

   例えば、サンプルアカウントで **[!UICONTROL LoadAsset]** prop にアクセスするには、**[!UICONTROL カスタムトラフィック]**/**[!UICONTROL カスタムトラフィック 1～10]**/**[!UICONTROL LoadAsset]** を選択する必要があります。 10 を超えるカスタム prop がある場合は、他のメニューも表示されます。

1. Adobe Analytics が生成したチャートを参照します。このグラフは、通常、単一の指標のデータです。 このデータがどのアセットに関連付けられているかも把握したい場合は、このイベントのアセットデータを取得します。 例えば、どのビデオが 50% しか視聴されていないのか、またはセット内のどの画像が人気があるのかを知ることは、多くの場合、役に立ちます。

>[!NOTE]
>
>すべてのAdobe Dynamic Media Classic ビューアデータは、Adobe Analyticsのカスタムトラフィックレポートまたはカスタムコンバージョンレポートに表示およびレポートされます。

詳しくは、[Analytics チュートリアル ](https://experienceleague.adobe.com/ja/docs/analytics-learn/tutorials/overview) を参照してください。