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
source-git-commit: 910410706fbd9dd79a8dda402af454a50132cc41
workflow-type: tm+mt
source-wordcount: '1227'
ht-degree: 33%

---

# オファーセットの作成 {#creating-an-offer-set}

以下のいずれかのオファーセットを作成できます。

* ビデオ
* パラメータ化テンプレート
* イメージ

テンプレートの場合は、「 」を選択します。 **[!UICONTROL 追加とプレビュー]**&#x200B;をクリックし、選択したパラメーターを設定します。 他のオファーセットタイプにはパラメーターは含まれませんが、「 」を選択することでカスタマイズできます **[!UICONTROL プレビュー]** 使用可能なプリセットを変更します。

Adobe Dynamic Media Classicには、編集用のツールやオファーセットの作成用のツールが用意されています。

>[!NOTE]
>
>オファーセットを作成する前に、セットに使用するすべてのアセットをAdobe Dynamic Media Classicに公開してください。 [手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)を参照してください。

## オファーセットのタイプ {#types-of-offer-sets}

以下のオファーセットのタイプからオファーセットを作成します。

* **画像** ：オファーセット用の画像をアセンブルできます。 各画像には、セット内の異なるオファーが含まれます。

* **画像テンプレート** - Adobe Dynamic Media Classicで、画像テンプレートを **[!UICONTROL ビルド]** /「基本テンプレート」コマンドを使用します。 テンプレートのパラメータ、コンポーネントを通じて、テキストフレームのテキストや様々な画像をスワップアウトおよびカスタマイズできます。オファーセットの場合は、テンプレートパラメータを使用して、オファーセット内の同じ画像のバリエーションなどを作成できます。画像テンプレートの作成とパラメータ化について詳しくは、 [テンプレートパラメーターの作成](creating-template-parameters.md#creating_template_parameters).

関連トピック [基本テンプレート](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) トレーニングビデオ。

* **ビデオ**  — オファーセット用のビデオを組み立てることができます。 各ビデオはセット内の異なるオファーになります。

## パラメーター化されたテンプレートを使用したオファーセットの作成 {#creating-an-offer-set-with-a-parameterized-template}

オファーセットを作成する際には、「**[!UICONTROL 保存後に公開]**」オプションがセットおよびセットメンバーに対して次のように影響します。

| **[!UICONTROL 保存後に公開]** 保存する前に選択したオプション？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**パラメーター化されたテンプレートを使用してオファーセットを作成するには：**

1. テンプレートまたはバナーを選択します。
1. に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL Test&amp;Target オファーセット]**.

   Test&amp;Target のオファーセットページには、オファーセット内のオファーが一覧表示されます。 リストの先頭アイテムがオブジェクトです。

1. オブジェクトを選択し、「 」を選択します。 **[!UICONTROL 追加とプレビュー]**.

   このページの左側には、テンプレートのパラメーターと値が表示されます。

1. パラメータ値を変更して、オファーを作成します。例えば、テキストフィールドに別のテキストを入力したり、レイヤーのサイズを変更したり、画像を別の画像に入れ替えたり、別のビューアプリセットを選択したりすることができます。
1. 選択 **[!UICONTROL 保存]** または **[!UICONTROL 名前を付けて保存**]** をクリックして、オファーをオファーセットの一部として保存します。

   Test&amp;Target のオファーセットページに、作成したオファーが一覧表示されます。

1. 手順 3 から 5 を繰り返して、セットのオファーをさらに作成します。
1. 作業が完了したら、ページの右下隅付近にある、 **[!UICONTROL 保存後に公開*]** が選択されています（デフォルト）。
1. 選択 **[!UICONTROL 閉じる]**、オファーセットの名前を入力し、「 」を選択します。 **[!UICONTROL 保存]**.

Test&amp;Target オファーセットページを閉じる前に、オファーセットをAdobe Target Standard/Premium にプッシュします。 詳しくは、 [オファーセットを Test&amp;Target にプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## 画像またはビデオを含むオファーセットの作成 {#creating-an-offer-set-with-images-or-videos}

オファーセットを作成する際には、「**[!UICONTROL 保存後に公開]**」オプションがセットおよびセットメンバーに対して次のように影響します。

| **[!UICONTROL 保存後に公開]** 保存する前に選択したオプション？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**画像またはビデオを含むオファーセットを作成するには：**

1. オファーセット用の画像またはビデオをアセンブルします。 Test&amp;Target オファーセット画面、グリッド表示またはリスト表示で開始し、次のいずれかの方法を使用します。

   * **Test&amp;Target オファーセット画面**  — に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL Test&amp;Target オファーセット]**. 画像またはビデオを画面にドラッグします。異なるサイズの画像またはビデオを作成するには、画像またはビデオの複数のコピーをドラッグして、個別にサイズを設定します。

   * **グリッド表示またはリスト表示**  — 画像またはビデオを選択し、次にに移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL Test&amp;Target オファーセット]**.

1. オプションで、画像またはビデオを選択し、「 」を選択します。 **[!UICONTROL プレビュー]**. オファーをプレビューページで、選択した画像やビデオのサイズや外観を変更できます。 または、オファーセット内のすべての画像やビデオを変更できます。

   * プリセットを選択して、画像またはビデオの外観とサイズを変更します。
   * 選択したプリセットをオファーセット内のすべてのオファーに適用するには、「 **[!UICONTROL すべてのプリセットにプリセットを選択]** 」チェックボックスをオンにします。

   選択 **[!UICONTROL 保存]** をクリックして、画像またはビデオオファーに対する変更を保存します。 次に、 **[!UICONTROL 閉じる]** をクリックして、 Test&amp;Target のオファーセットページに戻ります。

1. オファーセット用のオファーの作成を完了し、様々な画像用の画像プリセットの選択を完了したら、次の点を確認します。 **[!UICONTROL 保存後に公開]** が選択されています（デフォルト）。
1. 選択 **[!UICONTROL 保存]** オファーセットの名前を入力し、「 」を選択します。 **[!UICONTROL 保存]**.

Test&amp;Target オファーセットページを閉じる前に、オファーセットをAdobe Target Standard/Premium にプッシュします。 詳しくは、 [オファーセットを Test&amp;Target にプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target).

## オファーセットの編集 {#editing-an-offer-set}

公開済みセットと非公開セットのどちらを編集する場合でも、 **[!UICONTROL 保存後に公開]** このオプションは、次の方法でセットおよびセットメンバーに影響を与えます。

| セットが既に公開されているか？ | **[!UICONTROL 保存後に公開]** オプションを選択して編集を保存しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバは、公開済みの状態を保持します。 編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを編集するには：**

1. オファーセットを編集するには、オファーセットをグリッド表示またはリスト表示で表示し、オファーセットを選択します **[!UICONTROL 編集]** ロールオーバーボタン。
1. Test&amp;Target オファーセットページで、次のいずれかの操作をおこないます。

   * **オファーの削除**  — オファーを選択し、「 」を選択します。 **[!UICONTROL 削除]** をクリックして、オファーをセットから削除します。
   * **オファーの追加**  — オファーの追加方法は、使用するオファーセットのタイプによって異なります。
      * **テンプレート**  — 選択 **[!UICONTROL 追加とプレビュー]**「オファーを追加してプレビュー」ページで、別のオファーを作成します。
      * **画像とビデオ**  — 画像またはビデオを Test&amp;Target オファーセットページにドラッグします。

   >[!NOTE]
   >
   >キャンペーンと関連付けられているオファーセットは削除できません。キャンペーンに関連付けられているオファーセットを削除するには、Adobe Target Standard/Premium にログインし、最初にキャンペーンの関連付けを削除します。 キャンペーンから関連付けを解除した後でも、アセットを削除するにはAdobe Dynamic Media Classicからのみを使用します。その場合、Adobe Target Standard/Premium 内からではなく、Adobe Target Standard/Premium へのログインを必要とします。

1. 編集が終了したら、ページの右下隅付近にある **[!UICONTROL 保存後に公開]** が選択されています（デフォルト）。
1. 選択 **[!UICONTROL 保存]**、ストレージフォルダーを選択し、セットの名前を入力して、「 」を選択します。 **[!UICONTROL 保存]**.

## オファーセットの削除 {#delet-an-offer-set}

オファーセットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（「子」）は影響を受けません。代わりに、それぞれの既存の公開済みまたは非公開の状態が保持されます。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを削除するには：**

1. グリッド表示、リスト表示、または詳細表示で、1 つ以上のオファーセットを選択します。
1. グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **削除**.

>[!MORELIKETHIS]
>
>* [テンプレートパラメーターの作成](creating-template-parameters.md#creating_template_parameters)
