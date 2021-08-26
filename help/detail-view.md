---
title: 詳細ビューで作業する
description: Dynamic Media Classicの詳細ビューでの作業方法をAdobeします。
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 24%

---

# 詳細ビューで作業する{#working-in-detail-view}

アセットを詳細ビューで開くことで、アセットを操作したり、アセットについて学習したりできます。 詳細ビューには、アセットのサイズ、属性、派生物、メタデータが表示されます。 また、アセットが公開済みかどうか、アセットが公開されたのはいつかを確認し、公開済みアセットの URL を取得することもできます。アセットの種類によっては、様々な表示サイズでのプレビュー、ズームイン、シャープ、切り抜きなどのフォーマット操作を行うことができます。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![左側の](/help/assets/image_0.img.png)
*表示からは、[アセットライブラリ]パネルが非表示の詳細表示詳細表示。*

>[!NOTE]
>
>アセットが保存されているフォルダーを開くには、情報パネルの上部でフォルダーパスを選択します。

## 詳細ビューでアセットを開く {#open-an-asset-in-detail-view}

アセットを詳細ビューで表示して、アセットを詳細に確認、プレビュー、または操作できます。

1. 参照パネルで、次のいずれかの操作を行います。

   * アセットを選択します。AdobeDynamic Media Classicの右上隅付近にある&#x200B;**[!UICONTROL 詳細ビュー]**&#x200B;アイコンを選択します。
   * アセットをダブルクリックします。
   * アセットを選択し、**[!UICONTROL File]** > **[!UICONTROL Details]**&#x200B;に移動します。

>[!NOTE]
>
>詳細ビューで同じフォルダー内のアセット間を移動するには、「**[!UICONTROL 前のアセット]**」または「**[!UICONTROL 次のアセット]**」を選択します。 これらのボタンは、詳細ビューの右上隅にあります。

## 詳細ビューでの情報の取得 {#getting-information-in-detail-view}

詳細ビューには、アセットまたはファイルに関する情報が表示されます。 項目に関する次の情報が表示されます。保存先のフォルダー、ファイル名、AdobeDynamic Media Classicにアイテムがアップロードされた日付、公開履歴。 詳細表示では、メタデータの表示と編集、アセットのキーワードの追加も可能です。

詳細ビューでアセットURLを取得できます。ただし、URLはアセットを公開するまでアクティブになりません。 画像の場合、詳細ビューには、ビルドおよび派生アセットとメタデータ（ズームターゲットや画像セットなど）のリストも表示されます。

## 詳細ビューでのアセットの操作 {#working-with-assets-in-detail-view}

詳細表示には、開いたアセットを操作するためのツールが用意されています。 使用できるツールは、操作しているアセットの種類に応じて異なりますが、詳細ビューでは常に次の機能が提供されます。

* **公開する項目**  — 名前の左側にあ **** る「公開」アイコンを選択するか、 **[!UICONTROL ファイル]** / **** 公開 **[!UICONTROL またはファイル]** / **[!UICONTROL 非公開]**&#x200B;に移動します。

* **アセットの名前を変更**  — 名前を選択し、新しい名前を入力します。

* **メタデータの編集と追加**  — メタデータパネルを選択し、必要に応じて変更します。[メタデータの表示、追加、書き出し](/help/viewing-adding-exporting-metadata.md)を参照してください。

* **キーワードの編集と追加**  - 「キーワード」を選択し、必要に応じてキーワードを追加または削除します。詳しくは、[キーワードの追加または編集](/help/viewing-adding-exporting-metadata.md)を参照してください。

* **アセットを削除します**  -  **[!UICONTROL File]** / **[!UICONTROL Delete]**&#x200B;に移動します。

個別のファイル（画像、画像セット、フォントなど）の場合は、詳細ビューで公開と編集の履歴を表示し、ジョブの詳細を確認できます。

次の表に、詳細ビューで様々なタイプのアセットで使用できるその他のオプションを示します。

| アセットタイプ | 編集/調整 | プレビュー |
| --- | --- | --- |
| 画像 | 画像マップの追加<br>ズームターゲットの<br><br><br>追加CropSharpenCreate調整済みビュー | 可。ズームと画像プリセット |
| キャビネットおよびウィンドウカバリング画像 | 不可 | サムネール |
| eCatalog | 編集 | はい<br>情報パネルも利用できます |
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
| ビネットとレンダリングされたビネット | 不可 | 画像が表示されます<br>ビネットのレンダリング可能な要素の内容と構造をXML形式で表示できます |
| XML ファイル | 不可 | 内容が表示される |
| ZIP ファイル | 不可 | コンテンツが表示されない |

>[!MORELIKETHIS]
>
>* [メタデータの表示、追加、書き出し](viewing-adding-exporting-metadata.md#viewing_adding_and_exporting_metadata)

