---
title: オファーセットの作成
description: Adobe Dynamic Media Classicでオファーセットを作成する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 05f2cce0-72bf-4933-87ab-c9003c848e35
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T17:42:42.464Z'
TQID: 'https://experienceleague.adobe.com/vSBuzOB0sC5y6Kgl0ZadvJXsKRTiEMBzq0Tgu692AYY'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588id: d378ca77-2da1-4f39-ad92-1917fe974a38
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 1292
ht-degree: 21%

---

# オファーセットの作成 {#creating-an-offer-set}

次のいずれかのタイプのオファーセットを作成できます。

* ビデオ
* パラメータ化テンプレート
* イメージ

テンプレートの場合は、**[!UICONTROL 追加とプレビュー]**&#x200B;を選択し、選択したパラメーターを設定します。 その他のオファーセットタイプにはパラメーターは含まれていませんが、**[!UICONTROL プレビュー]**&#x200B;を選択して使用可能なプリセットを変更することで、パラメーターをカスタマイズできます。

Adobe Dynamic Media Classicには、オファーセットを作成するだけでなく、編集するためのツールも用意されています。

>[!NOTE]
>
>オファーセットを作成する前に、セットに使用するすべてのアセットをAdobe Dynamic Media Classicに公開してください。 [手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)を参照してください。

## オファーセットの種類 {#types-of-offer-sets}

次のタイプのオファーセットからオファーセットを作成します。

* **画像**: オファーセットの画像を組み立てることができます。 各画像には、セット内に異なるオファーが含まれています。

* **画像テンプレート**: **[!UICONTROL ビルド]**/テンプレートの基本コマンドを使用して、Adobe Dynamic Media Classicで画像テンプレートをパラメーター化できます。 パラメーター、テンプレートのコンポーネント、テキストフレーム内のテキスト、異なる画像を切り替えてカスタマイズできます。 オファーセットの場合、例えば、テンプレートパラメーターを使用して、オファーセット内の同じ画像にバリエーションを作成できます。 画像テンプレートの作成とパラメータ化について詳しくは、[ テンプレートパラメーターの作成](creating-template-parameters.md#creating_template_parameters)を参照してください。

[ テンプレートの基本](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)のトレーニングビデオも参照してください。

* **ビデオ**: オファーセットのビデオを組み立てることができます。 各ビデオはセット内の異なるオファーになります。

## パラメータ化されたテンプレートを使用したオファーセットの作成 {#creating-an-offer-set-with-a-parameterized-template}

オファーセットを作成する場合、保存&#x200B;]**後に**[!UICONTROL &#x200B;公開オプションは、次の方法でセットとセットメンバーに影響を与えます。

| 保存する前に保存&#x200B;]**オプションを選択した後に**[!UICONTROL &#x200B;公開しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**パラメーター化されたテンプレートを使用してオファーセットを作成するには：**

1. テンプレートまたはバナーを選択します。
1. **[!UICONTROL ビルド]** > **[!UICONTROL テスト&amp;ターゲットオファーセット]**&#x200B;に移動します。

   Test&amp;Target オファーセットページには、オファーセット内のオファーが一覧表示されます。 リストの先頭アイテムがオブジェクトです。

1. オブジェクトを選択し、**[!UICONTROL 追加とプレビュー]**&#x200B;を選択します。

   このページの左側には、テンプレートのパラメーターと値が表示されます。

1. パラメータ値を変更して、オファーを作成します。 例えば、テキストフィールドに別のテキストを入力したり、レイヤーのサイズを変更したり、ある画像を別の画像に入れ替えたり、別のビューアプリセットを選択したりすることができます。
1. オファーをオファーセットの一部として保存するには、**[!UICONTROL 保存{1**または**[!UICONTROL &#x200B;別名で保存&#x200B;]**を選択します。]**

   Test&amp;Target オファーセット ページには、作成したオファーが一覧表示されます。

1. 手順 3 から 5 を繰り返して、セットのオファーをさらに作成します。
1. 終了したら、ページの右下隅付近で、保存*]**が選択された後に**[!UICONTROL &#x200B;公開することを確認します（デフォルト）。
1. **[!UICONTROL 閉じる]**&#x200B;を選択し、オファーセットの名前を入力してから、**[!UICONTROL 保存]**&#x200B;を選択します。

Test&amp;Target オファーセットページを閉じる前に、オファーセットをAdobe Target Standard/Premiumにプッシュします。 「[ オファーセットをTest&amp;Targetにプッシュする](pushing-offer-sets-target.md#pushing_offer_sets_to_target)」を参照してください。

## 画像またはビデオを使用したオファーセットの作成 {#creating-an-offer-set-with-images-or-videos}

オファーセットを作成する場合、保存&#x200B;]**後に**[!UICONTROL &#x200B;公開オプションは、次の方法でセットとセットメンバーに影響を与えます。

| 保存する前に保存&#x200B;]**オプションを選択した後に**[!UICONTROL &#x200B;公開しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**画像またはビデオを含むオファーセットを作成するには：**

1. オファーセット用の画像またはビデオを作成します。 テスト&amp;ターゲットオファーセット画面またはグリッドビューまたはリストビューで開始し、次のいずれかの方法を使用します。

   * **テスト&amp;ターゲットオファーセット画面**: **[!UICONTROL ビルド]** > **[!UICONTROL テスト&amp;ターゲットオファーセット]**&#x200B;に移動します。 画像またはビデオを画面にドラッグします。 異なるサイズの画像またはビデオを作成するには、画像またはビデオの複数のコピーをドラッグして、個別にサイズを設定します。

   * **グリッド表示またはリスト表示**：画像またはビデオを選択し、**[!UICONTROL ビルド]** > **[!UICONTROL テスト&amp;ターゲットオファーセット]**&#x200B;に移動します。

1. オプションで、画像またはビデオを選択し、**[!UICONTROL プレビュー]**&#x200B;を選択します。 プレビューオファーページで、選択した画像またはビデオのサイズと外観を変更できます。 または、オファーセット内のすべての画像またはビデオを変更できます。

   * プリセットを選択して、画像またはビデオの外観とサイズを変更します。
   * オファーセット内のすべてのオファーに選択したプリセットを適用するには、**`Select Presets to All`** チェックボックスをオンにします。

   **[!UICONTROL 保存]**&#x200B;を選択して、画像またはビデオのオファーに対する変更を保存します。 次に、**[!UICONTROL 閉じる]**&#x200B;を選択して、テストとターゲットのオファーセットページに戻ります。

1. オファーセットのオファーを作成し、異なる画像の画像プリセットを選択したら、**[!UICONTROL 保存]**&#x200B;が選択された後に公開します（デフォルト）。
1. **[!UICONTROL 保存]**&#x200B;を選択し、オファーセットの名前を入力して、**[!UICONTROL 保存]**&#x200B;を選択します。

Test&amp;Target オファーセットページを閉じる前に、オファーセットをAdobe Target Standard/Premiumにプッシュします。 「[ オファーセットをTest&amp;Targetにプッシュする](pushing-offer-sets-target.md#pushing_offer_sets_to_target)」を参照してください。

## オファーセットの編集 {#editing-an-offer-set}

公開済みセットを編集する場合でも、非公開セットを編集する場合でも、**[!UICONTROL 保存した後に公開]** オプションは、次の方法でセットとセットメンバーに影響します。

| セットが既に公開されているか？ | **[!UICONTROL 編集を保存する前に保存]** オプションを選択した後に公開しますか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
| --- | --- | --- | --- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーの公開状態が維持される。 編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを編集するには：**

1. オファーセットを編集するには、グリッドビューまたはリストビューでオファーセットを表示し、その&#x200B;**[!UICONTROL 編集]** ロールオーバーボタンを選択します。
1. 「テストとターゲットのオファーセット」ページで、次のいずれかの操作を行います。

   * **オファーの削除**: オファーを選択し、**[!UICONTROL 削除]**&#x200B;を選択して、セットからオファーを削除します。
   * **オファーの追加**：オファーの追加方法は、使用しているオファーセットの種類によって異なります。
      * **テンプレート**: **[!UICONTROL 追加とプレビュー]**&#x200B;を選択し、「オファーを追加とプレビュー」ページで別のオファーを作成します。
      * **画像とビデオ**：画像またはビデオをTest&amp;Target オファーセットページにドラッグします。

   >[!NOTE]
   >
   >キャンペーンに関連付けられているオファーセットは削除できません。 キャンペーンに関連付けられているオファーセットを削除するには、Adobe Target Standard/Premiumにログインし、キャンペーンの関連付けを最初に削除します。 キャンペーンから関連付けを解除した後でも、アセットはAdobe Dynamic Media Classicからのみ削除でき、Adobe Target Standard/Premiumへのログインが必要となり、Adobe Target Standard/Premium内からは削除できません。

1. 編集を終了したら、ページの右下隅付近で、保存&#x200B;]**が選択された後に**[!UICONTROL &#x200B;公開することを確認します（デフォルト）。
1. **[!UICONTROL 保存]**&#x200B;を選択し、ストレージフォルダーを選択し、セットの名前を入力してから、**[!UICONTROL 保存]**&#x200B;を選択します。

## オファーセットの削除 {#delet-an-offer-set}

オファーセットを削除すると、そのセット自体はごみ箱に移されます。 ただし、そのセット内のメンバー（または「子」）は影響を受けません。代わりに、それぞれが既存の公開済みまたは未公開状態を保持します。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを削除するには：**

1. グリッド表示、リスト表示または詳細表示で、1つ以上のオファーセットを選択します。
1. グローバルナビゲーションバーで、**[!UICONTROL ファイル]** > **[!UICONTROL 削除]** > **削除**&#x200B;に移動します。

>[!MORELIKETHIS]
>
>* [ テンプレートパラメーターの作成](creating-template-parameters.md#creating_template_parameters)
