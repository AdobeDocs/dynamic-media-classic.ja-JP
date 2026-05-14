---
title: Media Portal ユーザが使用できる書き出しオプションの指定
description: Adobe Dynamic Media ClassicのMedia Portal ユーザーが使用できる書き出しオプションを指定する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
autotag-review: '2026-05-13T20:13:39.327Z'
TQID: 'https://experienceleague.adobe.com/gw9YPj-PDme06RNMU-X9suAD2O7etGAqB62V-GPIJdI'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 390
ht-degree: 42%

---

# Media Portal ユーザが使用できる書き出しオプションの指定 {#specifying-export-options-available-to-media-portal-users}

管理者から権限が付与されている場合、Media Portal ユーザは画像を書き出すときにその形式を変更できます。 例えば、サイズ、ファイル形式および画質を変更できます。 書き出し時に画像の形式を自動的に変更することで、画像を個別に変換する手間を省き、時間を節約できます。 また、管理者はプリセット、つまり事前に選択した画像形式の設定を作成できます。 画像の書き出し時にプリセットを使用すると、会社が指定した内容で画像の形式を変更できます。

ユーザー定義の変換を使用して画像アセットを書き出す場合や、元のプライマリ画像を書き出す場合は、次の2つの制限が適用されます。

* 書き出しジョブの場合、書き出し用の圧縮 ZIP ファイルの最大ファイルサイズは 1 GB です。
* 書き出しジョブあたり合計 500 個のアセットまで許容されています。

[Adobe Dynamic Media Classicからのアセットの書き出し](exporting-assets-from-dmc.md#exporting-assets-from_dmc)も参照してください。

**Media Portal ユーザーが使用できる書き出しオプションを指定するには：**

1. グローバルナビゲーションバーで、**[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**&#x200B;に移動します。
1. 画像プリセットウィンドウで、必要に応じて次のオプションを選択します。

   * **Enable User-Defined Conversion**：このオプションを選択すると、ユーザーは選択したAssetsを書き出しウィンドウの&#x200B;**[!UICONTROL サイズ]** ドロップダウンリストから「その他」を選択できます。 次に、ピクセルやセンチメートルなどの測定単位を選択し、目的の幅と高さを指定します。 ユーザがこれらのファイルを書き出したり、ダウンロードしたりするとき、画像ファイルの形式が変更されます。

     **[!UICONTROL サイズ]** ドロップダウンリストから&#x200B;**[!UICONTROL ピクセル]**&#x200B;を選択した場合、画像の幅×高さは1億ピクセルを超えることはできません。 このサイズは、正方形の画像の場合は10,000 × 10,000 ピクセル、縦横比が2 x 3の画像の場合は約8,000 × 12,000 ピクセルになります。 このサイズ制限は、元のプライマリ画像を書き出す場合には適用されません。

     ユーザーがダウンロードしたファイルを再フォーマットせずにダウンロードするには、このオプションの選択を解除します。

   * **オリジナルの書き出しを有効にする**：元のプライマリ画像を書き出すことができます。 **[!UICONTROL 選択したAssetsを書き出し]** パネルで、**[!UICONTROL コンバージョン]** ドロップダウンメニューを開き、**[!UICONTROL 元のファイルを書き出し]**&#x200B;を選択して元のファイルを書き出すことができます。 ユーザが画像を書き出すときに画像プリセットを選択するか、変換オプションを選択することを強制するには、このオプションの選択を解除します。

>[!MORELIKETHIS]
>
>* [画像プリセット](application-setup.md#image_presets)
>* [&#x200B; グループの画像プリセットのアクセス権限を選択](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
