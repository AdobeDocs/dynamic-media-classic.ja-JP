---
title: '詳細ビューでの操作 '
description: 詳細ビューでの作業方法を説明します。
uuid: cb62f765-9b7f-4a53-8206-99afae2fb80d
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eaa214ff-d1ef-4691-9148-d01bf243c810
feature: Dynamic Media Classic，アセット管理
role: User
exl-id: 618ae6a4-6f60-4a80-b197-a9d35b3c47af
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 65%

---

# 詳細ビューでの操作 {#working-in-detail-view}

アセットを詳細ビューで開いて、アセットを操作したり確認することができます。詳細ビューでは、アセットのサイズ、属性、派生物およびメタデータを確認できます。また、アセットが公開済みかどうか、アセットが公開されたのはいつかを確認し、公開済みアセットの URL を取得することもできます。アセットの種類によっては、様々な表示サイズでのプレビュー、ズームイン、シャープ、切り抜きなどのフォーマット操作を行うことができます。

<!-- 

Comment Type: remark
Last Modified By: Rick Brough (rbrough@adobe.com)
Last Modified Date: 2018-06-14T13:52:46.623-0400

<p>as_detail_view_popup.png found in Downloads on local in folder "scene7-images"</p>

 -->

![左側の](/help/assets/image_0.img.png)
*表示からは、アセットライブラリパネルが非表示の詳細ビュー。*

>[!NOTE]
>
>アセットが保存されているフォルダを開くには、情報パネルの上部のフォルダパスをクリックします。

## 詳細ビューでアセットを開く {#open-an-asset-in-detail-view}

アセットを詳細ビューで表示すると、アセットの詳細の確認、プレビュー、操作を行うことができます。

1. 参照パネルで、次のいずれかの操作を行います。

   * アセットを選択します。Dynamic Media Classicの右上隅付近にある&#x200B;**[!UICONTROL 詳細ビュー]**&#x200B;アイコンをクリックします。
   * アセットをダブルクリックします。
   * アセットを選択し、**[!UICONTROL File]** > **[!UICONTROL Details]**&#x200B;をクリックします。

>[!NOTE]
>
>前のアセットまたは次のアセットボタンを選択して、同じフォルダ内の次のアセットまたは前のアセットを詳細ビューで表示することができます。これらのボタンは、詳細ビューの右上隅にあります。

## 詳細ビューでの情報の取得 {#getting-information-in-detail-view}

詳細ビューには、アセットやファイルに関する情報が表示されます。項目に関する次の情報が表示されます。保存先のフォルダー、ファイル名、項目がDynamic Media Classicにアップロードされた日付、および公開履歴。 詳細ビューでは、メタデータを表示して編集し、アセットのキーワードを追加することもできます。

詳細ビューでアセットの URL を取得できますが、URL はアセットを公開するまでアクティブになりません。画像の場合は、ズームターゲットや画像セットなど、ビルドと派生アセットおよびメタデータのリストも詳細ビューに表示されます。

## 詳細ビューでのアセットの操作 {#working-with-assets-in-detail-view}

開いているアセットを操作するためのツールが詳細ビューに表示されます。利用可能なツールは、操作しているアセットタイプによって異なります。ただし、次の機能は常に表示されます。

* **公開用の項目**  — 名前の左側にあ **** る「公開」アイコンをクリックするか、ファ **[!UICONTROL イル/公]** 開/非公 **[!UICONTROL 開]**&#x200B;をクリックします。

* **アセットの名前の変更**  — 名前を選択し、新しい名前を入力します。

* **メタデータの編集と追加**  — メタデータパネルを選択し、必要に応じて変更します。詳しくは、[メタデータの表示、追加、書き出し](/help/viewing-adding-exporting-metadata.md)を参照してください。

* **キーワードの編集と追加**  - 「キーワード」を選択し、必要に応じてキーワードを追加または削除します。詳しくは、[キーワードの追加または編集](/help/viewing-adding-exporting-metadata.md)を参照してください。

* **アセットの削除**  -  **[!UICONTROL File]** / **[!UICONTROL Delete]**&#x200B;をクリックします。

画像、画像セット、フォントなどの独立したファイルの場合は、詳細ビューで公開および編集ヒストリーを確認したり、ジョブの詳細を確認することができます。

次の表に、様々なタイプのアセットで使用可能なその他のオプションの詳細表示を示します。

| アセットタイプ | 編集/調整 | プレビュー |
|--- |--- |--- |
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

