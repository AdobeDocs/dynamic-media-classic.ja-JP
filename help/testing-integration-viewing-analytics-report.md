---
title: Adobe Analytics レポートの表示による統合のテスト
description: Adobe Analyticsレポートを表示して統合をテストする方法を学習します。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Mediaクラシック
role: Data Engineer,Administrator,Business Practitioner
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 15%

---

# Adobe Analytics レポートの表示による統合のテスト{#testing-the-integration-by-viewing-an-adobe-analytics-report}

必要な変数をAdobe Analyticsで作成し、それらの変数をDynamic Mediaクラシックイベントにリンクし、必要な実装手順を完了したら、設定をテストできます。 データが Adobe Analytics 内で収集されることをテストして確認できます。設定が正常に動作する場合は、それ以上の手順は必要ありません。上記の手順に従って、Dynamic Mediaクラシックイベントデータを1つ以上のカスタムトラフィック変数にリンクしたと仮定し、次のワークフローに従ってAdobe Analytics内のデータをテストします。

**Adobe Analyticsレポートを表示して統合をテストするには：**

1. アカウントからDynamic Mediaクラシックビューアを開始します。特に、取得する指標をブロードキャストするビューアで、これを操作してイベントデータを作成します。

   例えば、画像セット内の人気のある代替表示を測定する場合は、画像セットをプレビューし、様々なサムネール画像をクリックします。

1. Adobe Analytics内で、**[!UICONTROL カスタムトラフィック]**/**[!UICONTROL カスタムトラフィック1-10]**/[prop]に移動し、メニュー項目から適切なトラフィックprop名を選択します。

   例えば、サンプルアカウントの&#x200B;**[!UICONTROL LoadAsset]** propにアクセスする場合、適切なメニュー項目は&#x200B;**[!UICONTROL カスタムトラフィック]** > **[!UICONTROL カスタムトラフィック1-10]** > **[!UICONTROL LoadAsset]**&#x200B;です。 カスタムpropが10個を超える場合は、他のメニュー項目も表示されます。

1. Adobe Analytics が生成したチャートを参照します。通常、このグラフは1つの指標のデータに過ぎません。 このデータが関連付けられているアセットも特定したい場合は、このイベントのアセットデータを取得します。 例えば、50%までしか視聴されていないビデオや、セット内のどの画像が人気があるかを知ると役立ちます。

>[!NOTE]
>
>すべてのDynamic Mediaクラシックビューアのデータは、Adobe Analyticsのカスタムトラフィックレポートまたはカスタムコンバージョンレポートに表示およびレポートされます。

詳しくは、[AnalyticsTutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html)を参照してください。