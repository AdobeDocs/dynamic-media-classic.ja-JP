---
title: オファーセットの作成
description: Adobe Dynamic Media Classicでオファーセットを作成する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 21%

---

# オファーセットの作成 {#creating-an-offer-set}

次のタイプのオファーセットを作成できます。

* ビデオ
* パラメータ化テンプレート
* イメージ

テンプレートの場合は、「**[!UICONTROL 追加とプレビュー]** を選択し、選択したパラメーターを設定します。 その他のオファーセットタイプにはパラメーターは含まれていませんが、**[!UICONTROL プレビュー]** を選択して使用可能なプリセットを変更することで、カスタマイズできます。

Adobe Dynamic Media Classicには、オファーセットの作成や編集を行うためのツールが用意されています。

>[!NOTE]
>
>オファーセットを作成する前に、セットに使用するすべてのアセットをAdobe Dynamic Media Classicに公開してください。 [手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)を参照してください。

## オファーセットのタイプ {#types-of-offer-sets}

次のタイプのオファーセットからオファーセットを作成します。

* **画像**：オファーセットの画像を作成できます。 各画像のセットには、異なるオファーが含まれます。

* **画像テンプレート**:**[!UICONTROL 作成]**/「テンプレートの基本」コマンドを使用して、Adobe Dynamic Media Classicの画像テンプレートをパラメーター化できます。 テンプレートのパラメーター、コンポーネント、テキストフレーム内のテキスト、様々な画像を入れ替えてカスタマイズできます。 オファーセットの場合、例えばテンプレートパラメーターを使用して、オファーセット内の同じ画像にバリエーションを作成できます。 画像テンプレートの作成とパラメーター化について詳しくは、[ テンプレートパラメーターの作成 ](creating-template-parameters.md#creating_template_parameters) を参照してください。

[ テンプレートの基本 ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) トレーニングビデオも参照してください。

* **ビデオ**：オファーセットのビデオを組み合わせることができます。 各ビデオはセット内の異なるオファーになります。

## パラメーター化されたテンプレートを使用したオファーセットの作成 {#creating-an-offer-set-with-a-parameterized-template}

オファーセットを作成する場合、**[!UICONTROL 保存後のPublish]** オプションはセットおよびセットメンバーに次のように影響します。

| **[!UICONTROL 保存後にPublish]** 保存する前にオプションを選択しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**パラメーター化テンプレートを使用してオファーセットを作成するには：**

1. テンプレートまたはバナーを選択します。
1. **[!UICONTROL ビルド]**/**[!UICONTROL Test&amp;Target オファーセット]** に移動します。

   Test&amp;Target オファーセットページには、オファーセットのオファーが一覧表示されます。 リストの先頭アイテムがオブジェクトです。

1. オブジェクトを選択し、「**[!UICONTROL 追加とプレビュー]**」を選択します。

   このページの左側には、テンプレートのパラメーターと値が表示されます。

1. パラメータ値を変更して、オファーを作成します。例えば、テキストフィールドに異なるテキストを入力したり、レイヤーのサイズを変更したり、画像を入れ替えたり、別のビューアプリセットを選択したりします。
1. オファーをオファーセットの一部として保存するには、**[!UICONTROL 保存]** または **[!UICONTROL 別名で保存**]** を選択します。

   Test&amp;Target オファーセットページには、作成したオファーが一覧表示されます。

1. 手順 3 から 5 を繰り返して、セットのオファーをさらに作成します。
1. 完了したら、ページの右下隅付近で、「save*]**の後に**[!UICONTROL  Publish」が選択されていることを確認します（デフォルト）。
1. 「**[!UICONTROL 閉じる]**」を選択し、オファーセットの名前を入力して、「**[!UICONTROL 保存]**」を選択します。

Test&amp;Target オファーセットページを閉じる前に、オファーセットをAdobe Target Standard/Premium にプッシュします。 [Test&amp;Target へのオファーセットのプッシュ ](pushing-offer-sets-target.md#pushing_offer_sets_to_target) を参照してください。

## 画像またはビデオを含むオファーセットの作成 {#creating-an-offer-set-with-images-or-videos}

オファーセットを作成する場合、**[!UICONTROL 保存後のPublish]** オプションはセットおよびセットメンバーに次のように影響します。

| **[!UICONTROL 保存後にPublish]** 保存する前にオプションを選択しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**画像またはビデオを含むオファーセットを作成するには：**

1. オファーセット用の画像やビデオの組み立て。 Test&amp;Target オファーセット画面、グリッド表示またはリスト表示で開始し、次のいずれかの方法を使用します。

   * **Test&amp;Target オファーセット画面**:**[!UICONTROL ビルド]**/**[!UICONTROL Test&amp;Target オファーセット]** に移動します。 画像またはビデオを画面にドラッグします。異なるサイズの画像またはビデオを作成するには、画像またはビデオの複数のコピーをドラッグして、個別にサイズを設定します。

   * **グリッド表示またはリスト表示**：画像またはビデオを選択し、**[!UICONTROL 作成]**/**[!UICONTROL Test&amp;Target オファーセット]** に移動します。

1. オプションで、画像またはビデオを選択し、「**[!UICONTROL プレビュー]**」を選択します。 プレビューオファーページで、選択した画像やビデオのサイズと外観を変更できます。 または、オファーセット内のすべての画像やビデオを変更できます。

   * プリセットを選択して、画像またはビデオの外観とサイズを変更します。
   * 選択したプリセットをオファーセット内のすべてのオファーに適用するには、「**[!UICONTROL プリセットをすべてに選択]** チェックボックスをオンにします。

   「**[!UICONTROL 保存]**」を選択して、画像またはビデオオファーに対する変更を保存します。 次に、「**[!UICONTROL 閉じる]**」を選択して、Test&amp;Target オファーセット ページに戻ります。

1. オファーセットのオファーを作成し、様々な画像の画像プリセットを選択したら、必ず **[!UICONTROL 保存後のPublish]** を選択します（デフォルト）。
1. 「**[!UICONTROL 保存]**」を選択して、オファーセットの名前を入力し、「**[!UICONTROL 保存]**」を選択します。

Test&amp;Target オファーセットページを閉じる前に、オファーセットをAdobe Target Standard/Premium にプッシュします。 [Test&amp;Target へのオファーセットのプッシュ ](pushing-offer-sets-target.md#pushing_offer_sets_to_target) を参照してください。

## オファーセットを編集 {#editing-an-offer-set}

公開済みセットと非公開セットのどちらを編集する場合でも、「**[!UICONTROL 保存後のPublish]**」オプションは、次のようにセットとセットメンバーに影響します。

| セットが既に公開されているか？ | 編集内容を保存する前に ]**保存後に**[!UICONTROL  Publish」オプションが選択されていますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーは、公開済みの状態を維持します。 編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを編集するには：**

1. オファーセットを編集するには、グリッド表示またはリスト表示でオファーセットを表示し、その **[!UICONTROL 編集]** ロールオーバーボタンを選択します。
1. Test&amp;Target オファーセット ページで、次のいずれかの操作を行います。

   * **オファーの削除**：オファーを選択し、「**[!UICONTROL 削除]**」を選択してセットからオファーを削除します。
   * **オファーの追加**：オファーの追加方法は、使用しているオファーセットのタイプによって異なります。
      * **テンプレート**:「**[!UICONTROL 追加とプレビュー]**」を選択し、「オファーを追加とプレビュー」ページで別のオファーを作成します。
      * **画像とビデオ**：画像またはビデオを Test&amp;Target オファーセット ページにドラッグします。

   >[!NOTE]
   >
   >キャンペーンに関連付けられているオファーセットは削除できません。 キャンペーンに関連付けられているオファーセットを削除するには、Adobe Target Standard/Premium にサインインし、最初にキャンペーンの関連付けを削除します。 キャンペーンから関連付けを解除した後でも、アセットはAdobe Dynamic Media Classicからのみ削除できます。削除するにはAdobe Target Standard/Premium へのログインが必要で、Adobe Target Standard/Premium 内からは削除できません。

1. 編集が完了したら、ページの右下隅付近で、「**[!UICONTROL 保存後にPublish]**」が選択されていることを確認します（デフォルト）。
1. 「**[!UICONTROL 保存]**」を選択し、ストレージフォルダーを選択します。次に、セットの名前を入力して、「**[!UICONTROL 保存]**」を選択します。

## オファーセットの削除 {#delet-an-offer-set}

オファーセットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（または「子」）は影響を受けません。代わりに、それぞれのメンバーが既存の公開済み状態または未公開状態を保持します。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを削除するには：:**

1. グリッド表示、リスト表示、詳細表示から、オファーセットを 1 つ以上選択します。
1. グローバルナビゲーションバーで **[!UICONTROL ファイル]**/**[!UICONTROL 削除]**/**削除** に移動します。

>[!MORELIKETHIS]
>
>* [ テンプレートパラメーターの作成 ](creating-template-parameters.md#creating_template_parameters)
