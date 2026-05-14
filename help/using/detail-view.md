---
title: 詳細表示での作業
description: Adobe Dynamic Media Classicの詳細ビューの操作方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:45:19.277Z'
TQID: 'https://experienceleague.adobe.com/XtUpvJz6aepSU0F9CupyrR8-cdSpNo3blHK38hh9Fc8'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 620
ht-degree: 21%

---

# 詳細表示での作業{#working-in-detail-view}

アセットを詳細ビューで開くことで、アセットの操作と学習を行うことができます。 詳細ビューでは、アセットサイズ、属性、派生、メタデータが表示されます。 また、アセットが公開されたかどうか、いつ公開されたかがわかります。また、公開されたアセットのURLを取得することもできます。 アセットの種類によっては、様々な表示サイズでのプレビュー、ズームイン、シャープ、切り抜きなどのフォーマット操作を行うことができます。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![詳細表示](/help/using/assets/image_0.img.png)
*アセットライブラリパネルを左側のビューから非表示にした詳細表示*

>[!NOTE]
>
>アセットが保存されているフォルダーを開くには、情報パネルの上部にあるフォルダーパスを選択します。

## アセットを詳細表示で開く {#open-an-asset-in-detail-view}

アセットを詳細ビューに表示して、綿密に調べたり、プレビューしたり、作業したりすることができます。

1. 参照パネルで、次のいずれかの操作を行います。

   * アセットを選択します。 Adobe Dynamic Media Classicの右上隅付近にある「**[!UICONTROL 詳細表示]**」アイコンを選択します。
   * アセットをダブルクリックします。
   * アセットを選択し、**[!UICONTROL ファイル]**/**[!UICONTROL 詳細]**&#x200B;に移動します。

>[!NOTE]
>
>アセットからアセットへのページは、同じフォルダーの詳細表示で作成できます。 「**[!UICONTROL 前のアセット]**」または「**[!UICONTROL 次のアセット]**」をクリックします。 これらのボタンは、詳細表示の右上隅にあります。

## 詳細ビューで情報を取得 {#getting-information-in-detail-view}

詳細表示には、アセットまたはファイルに関する情報が表示されます。 この情報は、アイテムについて表示されます。アイテムが保存されているフォルダー、そのファイル名、アイテムがAdobe Dynamic Media Classicにアップロードされた日付、公開履歴です。 また、詳細ビューでメタデータを表示および編集したり、アセットのキーワードを追加したりすることもできます。

アセットのURLは詳細ビューで取得できますが、アセットを公開するまでURLはアクティブになりません。 画像の場合、詳細表示には、作成および派生したアセットとメタデータ（ズームターゲットや画像セットなど）のリストも表示されます。

## 詳細ビューでのアセットの操作 {#working-with-assets-in-detail-view}

詳細ビューには、開いたアセットを操作するためのツールが用意されています。 使用可能なツールは、使用するアセットのタイプによって異なりますが、詳細ビューには常に次の機能があります。

* **パブリッシュ用アイテム**：名前の左側にある&#x200B;**[!UICONTROL `Publish`]** アイコンを選択するか、**[!UICONTROL ファイル]** > **[!UICONTROL 公開]**&#x200B;または&#x200B;**[!UICONTROL ファイル]** > **[!UICONTROL 非公開]**&#x200B;に移動します。

* **アセットの名前を変更**：名前を選択し、新しい名前を入力します。

* **メタデータの編集と追加**: メタデータパネルを選択し、必要に応じて変更します。 [ メタデータの表示、追加、エクスポート ](/help/using/viewing-adding-exporting-metadata.md)を参照してください。

* **キーワードの編集と追加**: キーワードを選択し、必要に応じて追加または削除します。 詳しくは、[キーワードの追加または編集](/help/using/viewing-adding-exporting-metadata.md)を参照してください。

* **アセットを削除**: **[!UICONTROL ファイル]** > **[!UICONTROL 削除]**&#x200B;に移動します。

ディスクリートファイル（画像、画像セット、フォントなど）の場合、公開履歴と編集履歴を表示したり、ジョブの詳細を詳細ビューで確認したりできます。

次の表は、詳細ビューで様々なタイプのアセットで使用できる他のオプションを示しています。

| アセットタイプ | 編集/調整 | プレビュー |
| --- | --- | --- |
| 画像 | 画像マップを追加<br> ズームターゲットを追加<br>切り抜き<br> シャープ <br>調整済みビューを作成 | 可。ズームと画像プリセット |
| キャビネットおよびウィンドウカバリング画像 | 不可 | サムネール |
| eCatalog | 編集 | はい<br>情報パネルも使用できます |
| フォント | フォント情報の編集 | 不可 |
| FXG ファイル | 編集 | 可 |
| ICC プロファイル［ICC ぷろふぁいる］ | プロファイル情報の編集 | 不可 |
| Illustrator ファイル | 不可（FXG に変換していない場合） | 不可 |
| 画像セット | 編集 | 可 |
| InDesign ファイル | 不可（FXG に変換していない場合） | 不可 |
| PDF ファイル | いいえ | いいえ |
| PSD ファイル | 可（個々のレイヤーで） | 可（個々のレイヤーで） |
| スピンセット | 編集 | 可 |
| SVG ファイル | いいえ | いいえ |
| テンプレート | 編集 | 可 |
| ビデオ | いいえ | はい |
| ビネットとレンダリングされたビネット | 不可 | 画像が表示されます<br> ビネットのレンダリング可能な要素の内容と構造をXML形式で表示できます |
| XML ファイル | 不可 | 内容が表示される |
| ZIP ファイル | 不可 | 内容は表示されません |

>[!MORELIKETHIS]
>
>* [ メタデータの表示、追加、書き出し](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
