---
title: 詳細ビューで作業する
description: Adobe Dynamic Media Classicの詳細ビューでの作業方法を説明します。
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
topic: Content Management
level: Intermediate
source-git-commit: ae7d0c6d3047d68ed3da4187ef516dc51c95de30
workflow-type: tm+mt
source-wordcount: '618'
ht-degree: 20%

---

# 詳細ビューで作業する{#working-in-detail-view}

アセットを詳細ビューで開くことで、アセットを操作したり、アセットについて学習したりできます。 詳細ビューには、アセットのサイズ、属性、派生、メタデータが表示されます。 また、アセットが公開されたかどうか、およびいつ公開されたかを確認し、公開されたアセットの URL を取得できます。 アセットの種類によっては、様々な表示サイズでのプレビュー、ズームイン、シャープ、切り抜きなどのフォーマット操作を行うことができます。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![詳細ビュー](/help/using/assets/image_0.img.png)
*左側のビューでは、アセットライブラリパネルを非表示にした詳細ビュー。*

>[!NOTE]
>
>アセットが保存されているフォルダーを開くには、情報パネルの上部でフォルダーパスを選択します。

## 詳細ビューでアセットを開く {#open-an-asset-in-detail-view}

アセットを詳細ビューで表示して、アセットを詳細に確認、プレビュー、または操作することができます。

1. 参照パネルで、次のいずれかの操作を行います。

   * アセットを選択します。 Adobe Dynamic Media Classicの右上隅近くにある、 **[!UICONTROL 詳細ビュー]** アイコン。
   * アセットをダブルクリックします。
   * アセットを選択し、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 詳細]**.

>[!NOTE]
>
>詳細ビューで同じフォルダ内のアセット間を移動するには、次の項目を選択します。 **[!UICONTROL 前のアセット]** または **[!UICONTROL 次のアセット]**. これらのボタンは、詳細ビューの右上隅にあります。

## 詳細ビューで情報を取得する {#getting-information-in-detail-view}

詳細ビューには、アセットまたはファイルに関する情報が表示されます。 項目に関するこの情報 ( 保存先のフォルダー、ファイル名、項目がAdobe Dynamic Media Classicにアップロードされた日付、公開履歴 ) が表示されます。 また、詳細ビューでは、メタデータの表示と編集、アセットのキーワードの追加を行うこともできます。

アセット URL は詳細ビューで取得できますが、この URL はアセットを公開するまでアクティブになりません。 詳細ビューには、ビルドおよび派生アセットとメタデータ（ズームターゲットや画像セットなど）のリストも表示されます。

## 詳細ビューでのアセットの操作 {#working-with-assets-in-detail-view}

詳細表示には、開いたアセットを操作するためのツールが表示されます。 使用できるツールは、操作しているアセットの種類に応じて異なりますが、詳細ビューでは常に次の機能が提供されます。

* **公開用項目**  — を選択します。 **[!UICONTROL 公開]** 名前の左にあるアイコン、または **[!UICONTROL ファイル]** > **[!UICONTROL 公開]** または **[!UICONTROL ファイル]** > **[!UICONTROL 非公開]**.

* **アセット名を変更**  — 名前を選択し、新しい名前を入力します。

* **メタデータの編集と追加**  — メタデータパネルを選択し、必要に応じて変更します。 詳しくは、 [メタデータの表示、追加、書き出し](/help/using/viewing-adding-exporting-metadata.md).

* **キーワードの編集と追加** - 「キーワード」を選択し、必要に応じてキーワードを追加または削除します。 詳しくは、[キーワードの追加または編集](/help/using/viewing-adding-exporting-metadata.md)を参照してください。

* **アセットの削除**  — に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 削除]**.

個別のファイル（画像、画像セット、フォントなど）の場合は、詳細ビューで公開と編集の履歴を表示し、ジョブの詳細を確認できます。

次の表は、詳細ビューで、様々なタイプのアセットで使用できるその他のオプションを示しています。

| アセットタイプ | 編集/調整 | プレビュー |
| --- | --- | --- |
| 画像 | 画像マップを追加<br>ズームターゲットの追加<br>切り抜き<br>シャープ<br>調整済みビューの作成 | 可。ズームと画像プリセット |
| キャビネットおよびウィンドウカバリング画像 | 不可 | サムネール |
| eCatalog | 編集 | はい<br>情報パネルも使用できます。 |
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
| ビネットとレンダリングされたビネット | 不可 | 画像が表示されます<br>ビネットのレンダリング可能な要素のコンテンツと構造を XML 形式で表示できます。 |
| XML ファイル | 不可 | 内容が表示される |
| ZIP ファイル | 不可 | コンテンツが表示されません |

>[!MORELIKETHIS]
>
>* [メタデータの表示、追加、書き出し](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)
