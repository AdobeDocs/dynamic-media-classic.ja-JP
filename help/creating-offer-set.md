---
title: オファーセットの作成
seo-title: オファーセットの作成
description: 'null'
seo-description: オファーセットの作成方法を説明します。
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '1220'
ht-degree: 57%

---


# オファーセットの作成{#creating-an-offer-set}

以下のいずれかのオファーセットを作成できます。

* ビデオ
* パラメータ化テンプレート
* イメージ

For templates, click **Add and Preview**, then set the parameters you choose. 他のオファーセットのタイプにはパラメーターが含まれていませんが、「**プレビュー**」をクリックしてプリセットを変更することでカスタマイズ可能です。

オファーセットの編集および作成を行うためのダイナミックMedia Classicオファーツール。

>[!NOTE]
>
>オファーセットを作成する前に、ダイナミックメディアクラシックに設定するアセットに使用するすべてのアセットを公開してください。 [手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)を参照してください。

## オファーセットのタイプ {#types-of-offer-sets}

以下のオファーセットのタイプからオファーセットを作成します。

* **画像**&#x200B;オファーセット用に画像をアセンブリできます。 各画像は、セット内に異なるオファーを含みます。

* **画像テンプレート** Dynamic Media Classicで、ビルド/基本テンプレートコマンドを使用して画像テンプレートをパラメータ化できます。 テンプレートのパラメータ、コンポーネントを通じて、テキストフレームのテキストや様々な画像をスワップアウトおよびカスタマイズできます。オファーセットの場合は、テンプレートパラメータを使用して、オファーセット内の同じ画像のバリエーションなどを作成できます。画像テンプレートの作成とパラメータ化について詳しくは、テンプレートパラメータの作成を参照してください。

* **ビデオ**&#x200B;オファーセット用にビデオをアセンブルできます。 各ビデオはセット内の異なるオファーになります。

## パラメータ化オファーを使用したテンプレートセットの作成 {#creating-an-offer-set-with-a-parameterized-template}

オファーセットを作成する際には、「**保存後に公開**」オプションがセットおよびセットメンバーに対して次のように影響します。

| 保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- |--- |--- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**パラメータ化オファーを使用してテンプレートセットを作成するには**

1. テンプレートまたはバナーを選択します。
1. **ビルド**／**Test&amp;Target オファーセット**&#x200B;をクリックします。

   テストターゲットオファーセットページのリストオファーは、オファーセット内にあります。 リストの先頭アイテムがオブジェクトです。

1. オブジェクトを選択し、「**追加とプレビュー**」をクリックします。

   このページの左側には、テンプレートのパラメーターと値が表示されます。

1. パラメータ値を変更して、オファーを作成します。例えば、テキストフィールドに別のテキストを入力したり、レイヤーのサイズを変更したり、画像を別の画像に入れ替えたり、別のビューアプリセットを選択したりすることができます。
1. 「**保存**」または「**名前を付けて保存**」をクリックして、オファーをオファーセットの一部として保存します。

   テストターゲットオファーセットページには、作成したオファーがリストされます。

1. 手順 3 から 5 を繰り返して、セットのオファーをさらに作成します。
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

Test&amp;ターゲットオファーセットページを閉じる前に、オファーセットをTarget Standard/Premiumにプッシュします。 詳しくは、[Test&amp;Target へのオファーセットのプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target)を参照してください。

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

オファーセットを作成する際には、「**保存後に公開**」オプションがセットおよびセットメンバーに対して次のように影響します。

| 保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- |--- |--- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**画像またはビデオを使用してオファーセットを作成するには**

1. オファーセット用の画像またはビデオをアセンブルします。 テスト&amp;ターゲットオファーセット画面、グリッド表示またはリスト表示で開始し、次のいずれかの方法を使用します。

   * **テスト&amp;ターゲットオファーセット画面**&#x200B;ビル **[!UICONTROL ド/テスト&amp;ターゲットオファーセットをクリックします]**。 画像またはビデオを画面にドラッグします。異なるサイズの画像またはビデオを作成するには、画像またはビデオの複数のコピーをドラッグして、個別にサイズを設定します。

   * **グリッドまたはリストの表示**&#x200B;画像またはビデオを選択し、 **[!UICONTROL ビルド/Test&amp;ターゲットオファーセットをクリックします]**。

1. または、画像またはビデオを選択して「**プレビュー**」をクリックします。プレビューオファーページで、選択した画像またはビデオのサイズと外観を変更できます。 または、オファーセット内のすべての画像またはビデオを変更できます。

   * プリセットを選択して、画像またはビデオの外観とサイズを変更します。
   * 「選択したプリセットをすべてに適用」チェックボックスをオンにして、選択したプリセットをオファーセットのすべてのオファーに適用します。

   「**保存**」をクリックして、変更内容を画像またはビデオオファーに保存します。次に、「**閉じる**」をクリックして Test&amp;Target オファーセット画面に戻ります。

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. 「**保存**」をクリックし、オファーセットの名前を入力し、「**保存**」をクリックします。

テストターゲットオファーセットページを閉じる前に、オファーセットをTarget Standard/Premiumにプッシュします。 詳しくは、[Test&amp;Target へのオファーセットのプッシュ](pushing-offer-sets-target.md#pushing_offer_sets_to_target)を参照してください。

## オファーセットの編集 {#editing-an-offer-set}

編集するセットが公開済みか非公開かに応じて、「**保存後に公開**」オプションがセットおよびセットメンバーに対して次のように影響します。

| セットが既に公開されているか？ | 編集内容の保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- |--- |--- |--- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーは公開済み状態を保持します。編集中に追加した新しいセットメンバーは公開済みまたは非公開の状態を保持します。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを編集するには**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. テストターゲットオファーセットページで、次のいずれかの操作を行います。

   * **オファーの削除**&#x200B;オファーを選択し、 
**「削除** 」で、オファーをセットから削除します。
   * **オファーの追加**&#x200B;オファーの追加方法は、操作しているオファーセットのタイプに応じて異なります。
   * **テンプレート**&#x200B;クリック 
**&amp;プレビュー追加**、および追加プレビューオファーページで別のオファーを作成します。
   * **画像とビデオ**&#x200B;画像またはビデオをテストターゲットオファーセットページにドラッグします。
   >[!NOTE]
   >
   >キャンペーンと関連付けられているオファーセットは削除できません。キャンペーンに関連付けられているオファーセットを削除するには、Target Standard/Premiumにサインインし、最初にキャンペーンの関連付けを削除します。 キャンペーンから関連付けを解除した後でも、アセットを削除するにはDynamic Media Classicからのみ可能です。Target Standard/Premiumにサインインする必要があり、Target Standard/Premium内からは削除できません。

1. When you finish editing, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. 「**保存**」をクリックし、保存するフォルダーを選択し、セットの名前を入力して、「**保存**」をクリックします。

## オファーセットの削除 {#deleting-an-offer-set}

オファーセットを削除すると、そのセット自体はごみ箱に移されます。ただし、そのセット内のメンバー（「子」）は影響を受けず、それらの既存の公開または非公開の状態が維持されます。

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを削除するには**

1. グリッドビュー、リストビューまたは詳細ビューで、1 つ以上のオファーセットを選択します。
1. グローバルナビゲーションバーで、**ファイル**／**削除**／**削除**&#x200B;をクリックします。

>[!MORELIKETHIS]
>
>* [テンプレートパラメータの作成](creating-template-parameters.md#creating_template_parameters)

