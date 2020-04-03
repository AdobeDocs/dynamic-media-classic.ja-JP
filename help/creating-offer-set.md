---
title: オファーセットの作成
seo-title: オファーセットの作成
description: 'null'
seo-description: オファーセット
uuid: 6d6a4af9-70c0-4cfa-9a8f-855d6adfcc8f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/target_classic_integration
discoiquuid: 59b6437d-c21e-4929-9291-3032dbb34565
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# オファーセットの作成{#creating-an-offer-set}

以下のいずれかのオファーセットを作成できます。

* ビデオ
* パラメータ化テンプレート
* イメージ

For templates, click **Add and Preview**, then set the parameters you choose. 他のオファーセットのタイプにはパラメーターが含まれていませんが、「**プレビュー**」をクリックしてプリセットを変更することでカスタマイズ可能です。

ダイナミックMedia Classicオファーツールを使用して、編集やオファーセットの作成を行います。

>[!NOTE]
>
>オファーセットを作成する前に、そのセットに使用するすべてのアセットをScene7 Publishing Systemに公開してください。 [手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)を参照してください。

## オファーセットのタイプ {#types-of-offer-sets}

以下のオファーセットのタイプからオファーセットを作成します。

* **画像**：画像セット用に画像をオファーできます。 各画像セットには、異なるオファーが含まれます。

* **画像テンプレート**：ビルド/基本テンプレートコマンドを使用して、ダイナミックメディアクラシックで画像テンプレートをパラメータ化できます。 テンプレートのパラメータ、コンポーネントを通じて、テキストフレームのテキストや様々な画像をスワップアウトおよびカスタマイズできます。オファーセットの場合は、テンプレートパラメータを使用して、オファーセット内の同じ画像のバリエーションなどを作成できます。画像テンプレートの作成とパラメータ化について詳しくは、テンプレートパラメータの作成を参照してください。

* **ビデオ**：ビデオセット用にビデオをオファーできます。 各ビデオはセット内の異なるオファーになります。

## パラメータ化オファーを使用したテンプレートセットの作成 {#creating-an-offer-set-with-a-parameterized-template}

オファーセットを作成する際には、「**保存後に公開**」オプションがセットおよびセットメンバーに対して次のように影響します。

| 保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- |--- |--- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**パラメータ化オファーを使用してテンプレートセットを作成するには**

1. テンプレートまたはバナーを選択します。
1. Click **Build** > **Target Classic Offer Set**.

   ターゲットクラシックオファーセットページでは、リストセット内のオファーがオファーされます。 リストの先頭アイテムがオブジェクトです。

1. オブジェクトを選択し、「**追加とプレビュー**」をクリックします。

   このページの左側には、テンプレートのパラメーターと値が表示されます。

1. パラメータ値を変更して、オファーを作成します。例えば、テキストフィールドに別のテキストを入力したり、レイヤーのサイズを変更したり、画像を別の画像に入れ替えたり、別のビューアプリセットを選択したりすることができます。
1. 「**保存**」または「**名前を付けて保存**」をクリックして、オファーをオファーセットの一部として保存します。

   ターゲットクラシックオファーセットページには、作成したオファーが表示されます。

1. 手順 3 から 5 を繰り返して、セットのオファーをさらに作成します。
1. When you finish, near the lower-right corner of the page, ensure that **Publish after save** is selected (default).
1. Click **Close**, enter a name for the offer set, and then click **Save**.

「ターゲットクラシックオファーセット」ページを閉じる前に、オファーセットを「ターゲットクラシック」に移動します。 See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## Creating an offer set with images or videos {#creating-an-offer-set-with-images-or-videos}

オファーセットを作成する際には、「**保存後に公開**」オプションがセットおよびセットメンバーに対して次のように影響します。

| 保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- |--- |--- |
| はい | 公開 | 公開 |
| いいえ | 非公開 | セットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**画像またはビデオを使用してオファーセットを作成するには**

1. 画像セットの画像またはビデオをオファーします。 開始は、ターゲットクラシックオファーセット画面、グリッド表示またはリスト表示で、次のいずれかの方法を使用します。

   * **ターゲットクラシックオファーセット画面**&#x200B;ビルド/ターゲットクラシックオファーセットをクリックします。 画像またはビデオを画面にドラッグします。異なるサイズの画像またはビデオを作成するには、画像またはビデオの複数のコピーをドラッグして、個別にサイズを設定します。

   * **グリッドまたはリスト表示**&#x200B;画像またはビデオを選択し、ビルド/ターゲットクラシックオファーセットをクリックします。

1. または、画像またはビデオを選択して「**プレビュー**」をクリックします。プレビューオファーページで、選択した画像またはビデオのサイズと外観を変更できます。 また、画像セット内のすべての画像やビデオを変更することもオファーできます。

   * プリセットを選択して、画像またはビデオの外観とサイズを変更します。
   * 「選択したプリセットをすべてに適用」チェックボックスをオンにして、選択したプリセットをオファーセットのすべてのオファーに適用します。
   「**保存**」をクリックして、変更内容を画像またはビデオオファーに保存します。Then click **Close** to return to the Target Classic Offer Set page.

1. After you finish creating offers for the offer set and choosing Image Presets for different images, ensure that **Publish after save** is selected (default).
1. 「**保存**」をクリックし、オファーセットの名前を入力し、「**保存**」をクリックします。

「ターゲットクラシックオファーセット」ページを閉じる前に、オファーセットを「ターゲットクラシック」に移動します。 See [Pushing offer sets to Target Classic](pushing-offer-sets-target-classic.md#pushing_offer_sets_to_target_classic).

## オファーセットの編集 {#editing-an-offer-set}

編集するセットが公開済みか非公開かに応じて、「**保存後に公開**」オプションがセットおよびセットメンバーに対して次のように影響します。

| セットが既に公開されているか？ | 編集内容の保存前に「保存後に公開」オプションが選択されているか？ | 保存後のセットの状態 | 保存後のセットメンバーの状態 |
|--- |--- |--- |--- |
| はい | はい | 公開 | 公開 |
| はい | いいえ | 公開 | 既存のセットメンバーは、公開状態を保持します。編集中に追加した新しいセットメンバーは、公開状態または非公開の状態を保持します。 |
| いいえ | はい | 公開 | 公開 |
| いいえ | いいえ | 非公開 | 既存のセットメンバーおよび編集中に追加した新しいセットメンバーの公開または非公開の状態が維持される。 |

[手動でのアセットの公開](publishing-files.md#manually_publishing_assets)と[手動でのアセットの非公開](publishing-files.md#manually_unpublishing_assets)も参照してください。

**オファーセットを編集するには**

1. To edit an offer set, display the offer set in Grid view or List view, and then click its **Edit** rollover button.
1. [ターゲットクラシックオファーセット]ページで、必要に応じて次の操作を行います。

   * **オファーの削除**&#x200B;オファーを選択し、「削除」をク **リックして** 、セットからオファーを削除します。
   * **オファーの追加**&#x200B;オファーの追加方法は、操作するオファーセットの種類に応じて異なります。
   * **テンプレ**&#x200B;ートク **リック&amp;プレビュー**(&amp;プレビュー)ページで、別のオファーを作成します。
   * **画像とビデオ画像また**&#x200B;はビデオを画像クラシックターゲットセットページにドラッグします。
   >[!NOTE]
   >
   >キャンペーンと関連付けられているオファーセットは削除できません。キャンペーンに関連付けられたオファーセットを削除するには、まずターゲットクラシックにログオンし、キャンペーンの関連付けを削除します。 キャンペーンから関連付けを解除した後でも、アセットはScene7 Publishing Systemからのみ削除でき、ターゲットClassicにログインする必要があり、ターゲットClassic内からは削除できません。

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

