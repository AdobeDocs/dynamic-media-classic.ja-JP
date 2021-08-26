---
title: Adobe Analytics レポートの表示による統合のテスト
description: Adobe Analyticsレポートを表示して統合をテストする方法を説明します。
uuid: 937375e0-6dea-4baa-a2b0-4f3e461c9ee2
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: 1ddc89ff-d2e9-42eb-a442-aa6b9871c991
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 6186fcf0-99b4-447d-ae94-b4124dcb405b
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 15%

---

# Adobe Analytics レポートの表示による統合のテスト{#testing-the-integration-by-viewing-an-adobe-analytics-report}

Adobe Analyticsで必要な変数を作成し、AdobeDynamic Media Classicイベントにリンクし、必要な実装手順を完了したら、設定をテストできます。 データが Adobe Analytics 内で収集されることをテストして確認できます。設定が正常に動作する場合は、それ以上の手順は必要ありません。上記の手順に従って、AdobeのDynamic Media Classicイベントデータを1つ以上のカスタムトラフィック変数にリンクしたと仮定した場合は、このワークフローに従ってAdobe Analytics内のデータをテストします。

**Adobe Analyticsレポートを表示して統合をテストするには：**

1. AdobeDynamic Media Classicビューアをアカウントから起動します。特に、取得する指標をブロードキャストするビューアを起動し、そのビューアを操作してイベントデータを作成します。

   例えば、画像セットで一般的な代替ビューを測定する場合は、画像セットをプレビューし、様々なサムネール画像をクリックします。

1. Adobe Analytics内で、「**[!UICONTROL カスタムトラフィック]** / **[!UICONTROL カスタムトラフィック1-10]** / [prop] 」に移動し、メニューからトラフィックprop名を選択します。

   例えば、サンプルアカウントの&#x200B;**[!UICONTROL LoadAsset]** propにアクセスするには、適切なメニュー選択は&#x200B;**[!UICONTROL カスタムトラフィック]** > **[!UICONTROL カスタムトラフィック1-10]** > **[!UICONTROL LoadAsset]**&#x200B;です。 10個を超えるカスタムpropがある場合は、その他のメニューも表示されます。

1. Adobe Analytics が生成したチャートを参照します。このグラフは通常、1つの指標のデータに過ぎません。 このデータが関連付けられているアセットも把握したい場合は、このイベントのアセットデータを取得します。 例えば、50%しか視聴されていないビデオや、一連のビデオが人気のある画像を知ると便利です。

>[!NOTE]
>
>すべてのAdobeDynamic Media Classicビューアデータは、Adobe Analyticsのカスタムトラフィックレポートまたはカスタムコンバージョンレポートに表示およびレポートされます。

詳しくは、[AnalyticsのTutorials](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/overview.html)を参照してください。