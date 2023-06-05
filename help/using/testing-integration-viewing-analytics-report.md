---
title: レポートを表示して Adobe Analytics 統合をテストする
description: Adobe Analyticsレポートを表示して、Adobe Dynamic Media Classicで統合をテストする方法を説明します。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 15%

---

#  レポートを表示して Adobe Analytics 統合をテストする{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Adobe Analyticsで必要な変数を作成し、Adobe Dynamic Media Classicイベントにリンクし、必要な実装手順を完了したら、設定をテストできます。 データが Adobe Analytics 内で収集されることをテストして確認できます。設定が正常に動作する場合は、それ以上の手順は必要ありません。上記の手順に従い、Adobe Dynamic Media Classicイベントデータを 1 つ以上のカスタムトラフィック変数にリンクしたと仮定した場合は、このワークフローに従ってAdobe Analytics内のデータをテストします。

**Adobe Analyticsレポートを表示して統合をテストするには：**

1. アカウント（特に、取得する指標をブロードキャストするビューア）からAdobe Dynamic Media Classicビューアを起動し、それを操作して、一部のイベントデータを作成します。

   例えば、画像セットで一般的な代替ビューを測定する場合は、画像セットをプレビューし、様々なサムネール画像をクリックします。

1. Adobe Analytics内で、 **[!UICONTROL カスタムトラフィック]** > **[!UICONTROL カスタムトラフィック 1-10]** > [prop の名前]をクリックし、メニューの選択肢からトラフィック prop 名を選択します。

   例えば、 **[!UICONTROL LoadAsset]** サンプルアカウントで prop を指定する場合、適切なメニュー選択は次のとおりです。 **[!UICONTROL カスタムトラフィック]** > **[!UICONTROL カスタムトラフィック 1-10]** > **[!UICONTROL LoadAsset]**. 10 個を超えるカスタム prop がある場合は、他のメニュー選択も表示されます。

1. Adobe Analytics が生成したチャートを参照します。このグラフは通常、単一の指標のデータに過ぎません。 このデータが関連付けられているアセットも把握したい場合は、このイベントのアセットデータを取得します。 例えば、50%までしか視聴されていないビデオや、セット内のどの画像が人気があるかを知ると便利です。

>[!NOTE]
>
>すべてのAdobe Dynamic Media Classicビューアデータが、Adobe Analyticsのカスタムトラフィックレポートまたはカスタムコンバージョンレポートに表示され、レポートされます。

詳しくは、 [AnalyticsTutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html).