---
title: オファーセットの作成
description: Adobe Dynamic Media Classicでオファーセットを作成する方法を説明します。
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
source-git-commit: 53551f938946bb78074127c05f984ae97e9ccca1
workflow-type: tm+mt
source-wordcount: '1293'
ht-degree: 35%

---

# オファーセットの作成 {#creating-an-offer-set}

以下のいずれかのオファーセットを作成できます。

* ビデオ
* パラメータ化テンプレート
* イメージ

テンプレートの場合は、「**[!UICONTROL 追加してプレビュー]**」を選択し、選択したパラメーターを設定します。 他のオファーセットタイプにはパラメーターは含まれていませんが、「**[!UICONTROL プレビュー]**」を選択して使用可能なプリセットを変更することで、パラメーターをカスタマイズすることもできます。

Adobe Dynamic Media Classicには、編集用のツールやオファーセットの作成用のツールが用意されています。

>[!NOTE]
>
>オファーセットを作成する前に、セットに使用するすべてのアセットをAdobe Dynamic Media Classicに公開してください。 [手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)を参照してください。

## オファーセットのタイプ {#types-of-offer-sets}

以下のオファーセットのタイプからオファーセットを作成します。

* **画像**  — オファーセット用に画像をアセンブリできます。各画像には、セット内の異なるオファーが含まれます。

* **画像テンプレート**  - Adobe Dynamic Media Classicで、ビルド/テンプレートの基本コマンドを使用して、画像テ **[!UICONTROL ンプレートをパラメータ化できます。]** テンプレートのパラメータ、コンポーネントを通じて、テキストフレームのテキストや様々な画像をスワップアウトおよびカスタマイズできます。オファーセットの場合は、テンプレートパラメータを使用して、オファーセット内の同じ画像のバリエーションなどを作成できます。画像テンプレートの作成とパラメータ化について詳しくは、[ テンプレートパラメータの作成 ](creating-template-parameters.md#creating_template_parameters) を参照してください。

[ テンプレートの基本 ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) トレーニングビデオも参照してください。

* **ビデオ**  — オファーセット用にビデオを組み立てることができます。各ビデオはセット内の異なるオファーになります。

## パラメーター化テンプレートを使用したオファーセットの作成 {#creating-an-offer-set-with-a-parameterized-template}

オファーセットを作成する際には、「**[!UICONTROL 保存後に公開]**」オプションがセットおよびセットメンバーに対して次のように影響します。

| **[!UICONTROL 保存前に「保存後に]** 公開」オプションが選択されているか | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**パラメーター化テンプレートを使用してオファーセットを作成するには：**

1. テンプレートまたはバナーを選択します。
1. **[!UICONTROL Build]** > **[!UICONTROL Test&amp;Target Offer Set]** に移動します。

   Test&amp;Target オファーセットページには、オファーセット内のオファーが一覧表示されます。 リストの先頭アイテムがオブジェクトです。

1. オブジェクトを選択し、「**[!UICONTROL 追加とプレビュー]**」を選択します。

   このページの左側には、テンプレートのパラメーターと値が表示されます。

1. パラメータ値を変更して、オファーを作成します。例えば、テキストフィールドに別のテキストを入力したり、レイヤーのサイズを変更したり、画像を別の画像に入れ替えたり、別のビューアプリセットを選択したりすることができます。
1. 「**[!UICONTROL 保存]**」または「**[!UICONTROL 名前を付けて保存**]**」を選択して、オファーをオファーセットの一部として保存します。

   Test&amp;Target オファーセットページに、作成したオファーが一覧表示されます。

1. 手順 3 から 5 を繰り返して、セットのオファーをさらに作成します。
1. 終了したら、ページの右下隅付近にある「保存後に公開」が選択されている（デフォルト）ことを確認します。****
1. 「**[!UICONTROL 閉じる]**」を選択し、オファーセットの名前を入力して、「**[!UICONTROL 保存]**」を選択します。

Test&amp;Target オファーセットページを閉じる前に、オファーセットをAdobe Target Standard/Premium にプッシュします。 [Test&amp;Target へのオファーセットのプッシュ ](pushing-offer-sets-target.md#pushing_offer_sets_to_target) を参照してください。

## 画像またはビデオを含むオファーセットの作成 {#creating-an-offer-set-with-images-or-videos}

オファーセットを作成する際には、「**[!UICONTROL 保存後に公開]**」オプションがセットおよびセットメンバーに対して次のように影響します。

| **[!UICONTROL 保存前に「保存後に]** 公開」オプションが選択されているか | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**画像またはビデオを使用してオファーセットを作成するには:**

1. オファーセット用の画像またはビデオをアセンブルします。 Test&amp;Target オファーセット画面、グリッドビューまたはリストビューで開始し、次のいずれかの方法を使用します。

   * **Test&amp;Target オファーセット画面**  — ビ **[!UICONTROL ルド]** / **[!UICONTROL Test&amp;Target オファーセット]**&#x200B;に移動します。画像またはビデオを画面にドラッグします。異なるサイズの画像またはビデオを作成するには、画像またはビデオの複数のコピーをドラッグして、個別にサイズを設定します。

   * **グリッド表示またはリスト表示**  — 画像またはビデオを選択し、ビル **[!UICONTROL ド]** / **[!UICONTROL Test&amp;Target オファーセット]**&#x200B;に移動します。

1. 必要に応じて、画像またはビデオを選択し、「**[!UICONTROL プレビュー]**」を選択します。 オファーをプレビューページで、選択した画像またはビデオのサイズと外観を変更できます。 または、オファーセット内のすべての画像やビデオを変更できます。

   * プリセットを選択して、画像またはビデオの外観とサイズを変更します。
   * 選択したプリセットをオファーセット内のすべてのオファーに適用するには、「**[!UICONTROL すべてにプリセットを選択]**」チェックボックスをオンにします。

   「**[!UICONTROL 保存]**」を選択して、画像またはビデオオファーに対する変更を保存します。 次に、「**[!UICONTROL 閉じる]**」を選択して、Test&amp;Target オファーセットページに戻ります。

1. オファーセット用のオファーの作成を終了し、異なる画像用の画像プリセットを選択した後、「**[!UICONTROL 保存後に公開]**」が選択されている（デフォルト）ことを確認します。
1. 「**[!UICONTROL 保存]**」を選択し、オファーセットの名前を入力して、「**[!UICONTROL 保存]**」を選択します。

Test&amp;Target オファーセットページを閉じる前に、オファーセットをAdobe Target Standard/Premium にプッシュします。 [Test&amp;Target へのオファーセットのプッシュ ](pushing-offer-sets-target.md#pushing_offer_sets_to_target) を参照してください。

## オファーセットの編集 {#editing-an-offer-set}

公開済みセットと非公開セットのどちらを編集する場合でも、「**[!UICONTROL 保存後に公開]**」オプションは、セットおよびセットメンバーに次のように影響します。

| セットが既に公開されているか？ | **[!UICONTROL 編集を保存する前]** に「保存後に公開する」オプションを選択した場合 | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーの公開状態が維持される。編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを編集するには：**

1. オファーセットを編集するには、オファーセットをグリッド表示またはリスト表示で表示し、**** ロールオーバーボタンを編集を選択します。
1. Test&amp;Target オファーセットページで、次のいずれかの操作をおこないます。

   * **オファーの削除**  — オファーを選択し、「削除」を選択し **** て、オファーをセットから削除します。
   * **オファーの追加**  — オファーの追加方法は、操作しているオファーセットのタイプによって異なります。
      * **テンプレート**  - 「追加と **[!UICONTROL プレビュー]**」を選択し、オファーを追加とプレビューページで別のオファーを作成します。
      * **画像とビデオ**  — 画像またはビデオを Test&amp;Target オファーセットページにドラッグします。

   >[!NOTE]
   >
   >キャンペーンと関連付けられているオファーセットは削除できません。キャンペーンに関連付けられているオファーセットを削除するには、Adobe Target Standard/Premium にログインし、最初にキャンペーンの関連付けを削除します。 キャンペーンとの関連付けを解除した後でも、アセットを削除するにはAdobe Dynamic Media Classicからのみが可能で、Adobe Target Standard/Premium 内からではなく、Adobe Target Standard/Premium へのログインが必要です。

1. 編集が終了したら、ページの右下隅付近にある「**[!UICONTROL 保存後に公開]**」が選択されている（デフォルト）ことを確認します。
1. 「**[!UICONTROL 保存]**」を選択し、保存フォルダーを選択し、セットの名前を入力して、「**[!UICONTROL 保存]**」を選択します。

## オファーセットの削除 {#deleting-an-offer-set}

オファーセットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（「子」）は影響を受けず、それらの既存の公開または非公開の状態が維持されます。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを削除するには：**

1. グリッド表示、リスト表示または詳細表示で、1 つ以上のオファーセットを選択します。
1. グローバルナビゲーションバーで、**[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **削除** に移動します。

>[!MORELIKETHIS]
>
>* [テンプレートパラメータの作成](creating-template-parameters.md#creating_template_parameters)

