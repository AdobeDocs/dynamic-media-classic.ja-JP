---
title: 作業詳細ビュー
description: Adobe Dynamic Media Classicの詳細ビューでの操作方法について説明します
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 20%

---

# 作業詳細ビュー{#working-in-detail-view}

詳細表示でアセットを開くことで、アセットの操作や詳細を行うことができます。 詳細表示には、アセットのサイズ、属性、派生、メタデータが表示されます。 また、アセットが公開されたかどうかとタイミングを確認し、公開されたアセットの URL を取得することもできます。 アセットの種類によっては、様々な表示サイズでのプレビュー、ズームイン、シャープ、切り抜きなどのフォーマット操作を行うことができます。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![詳細ビュー](/help/using/assets/image_0.img.png)
*左側のビューにアセットライブラリパネルが表示されない詳細ビュー。*

>[!NOTE]
>
>アセットが格納されているフォルダーを開くには、情報パネルの上部にあるフォルダーパスを選択します。

## 詳細表示でアセットを開く {#open-an-asset-in-detail-view}

アセットを詳細ビューで表示して、詳細に調べたり、プレビューしたり、作業したりできます。

1. 参照パネルで、次のいずれかの操作を行います。

   * アセットを選択します。 Adobe Dynamic Media Classicの右上隅付近にある **[!UICONTROL 詳細ビュー]** アイコン。
   * アセットをダブルクリックします。
   * アセットを選択し、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 詳細]**.

>[!NOTE]
>
>詳細表示の同じフォルダー内でアセットからアセットにページできます。 クリックする **[!UICONTROL 前のアセット]** または **[!UICONTROL 次のアセット]**. これらのボタンは、詳細ビューの右上隅にあります。

## 詳細表示で情報を取得 {#getting-information-in-detail-view}

詳細表示には、アセットまたはファイルに関する情報が表示されます。 項目に関する情報が表示されます。項目の保存先のフォルダー、ファイル名、項目がAdobe Dynamic Media Classicにアップロードされた日付、および公開履歴です。 また、詳細表示でアセットのメタデータを表示して編集したり、キーワードを追加したりすることもできます。

詳細表示でアセット URL を取得できますが、URL はアセットを公開するまでアクティブになりません。 画像の場合、詳細表示には、ズームターゲットや画像セットなどの作成および派生アセットとメタデータのリストも表示されます。

## 詳細表示でのアセットの操作 {#working-with-assets-in-detail-view}

詳細表示には、開いたアセットを操作するためのツールが用意されています。 使用できるツールは、使用しているアセットのタイプによって異なりますが、詳細表示には常に次の機能があります。

* **公開用アイテム**：を選択します **[!UICONTROL `Publish`]** アイコンをクリックするか、 **[!UICONTROL ファイル]** > **[!UICONTROL 公開]** または **[!UICONTROL ファイル]** > **[!UICONTROL 非公開]**.

* **アセットの名前を変更**：名前を選択し、新しい名前を入力します。

* **メタデータの編集と追加**：メタデータパネルを選択し、必要に応じて変更します。 参照： [メタデータの表示、追加、書き出し](/help/using/viewing-adding-exporting-metadata.md).

* **キーワードの編集と追加**：キーワードを選択し、必要に応じて追加または削除します。 詳しくは、[キーワードの追加または編集](/help/using/viewing-adding-exporting-metadata.md)を参照してください。

* **アセットの削除**：に移動します **[!UICONTROL ファイル]** > **[!UICONTROL 削除]**.

個別のファイル（画像、画像セット、フォントなど）の場合は、詳細表示で、公開履歴と編集履歴を表示したり、ジョブの詳細を確認したりできます。

次の表に、詳細表示で様々なタイプのアセットに使用できるその他のオプションを示します。

| アセットタイプ | 編集/調整 | プレビュー |
| --- | --- | --- |
| 画像 | 画像マップを追加<br>ズームターゲットの追加<br>切り抜き<br>シャープ<br>調整済みビューの作成 | 可。ズームと画像プリセット |
| キャビネットおよびウィンドウカバリング画像 | 不可 | サムネール |
| eCatalog | 編集 | はい<br>情報パネルも使用できます |
| フォント | フォント情報の編集 | 不可 |
| FXG ファイル | 編集 | 可 |
| ICC プロファイル［ICC ぷろふぁいる］ | プロファイル情報の編集 | 不可 |
| Illustrator ファイル | 不可（FXG に変換していない場合） | 不可 |
| 画像セット | 編集 | 可 |
| InDesign ファイル | 不可（FXG に変換していない場合） | 不可 |
| PDF ファイル | 不可 | いいえ |
| PSD ファイル | 可（個々のレイヤーで） | 可（個々のレイヤーで） |
| スピンセット | 編集 | 可 |
| SVG ファイル | 不可 | いいえ |
| テンプレート | 編集 | 可 |
| ビデオ | 不可 | はい |
| ビネットとレンダリングされたビネット | 不可 | 画像は次のように表示されます<br>ビネットのレンダリング可能な要素の内容と構造を XML 形式で表示できます |
| XML ファイル | 不可 | 内容が表示される |
| ZIP ファイル | 不可 | コンテンツが表示されない |

>[!MORELIKETHIS]
>
>* [メタデータの表示、追加、書き出し](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
