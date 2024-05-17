---
title: Media Portal ユーザが使用できる書き出しオプションの指定
description: Adobe Dynamic Media Classicで Media Portal ユーザーが使用できる書き出しオプションを指定する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
topic: Collaboration, Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 42%

---

# Media Portal ユーザが使用できる書き出しオプションの指定 {#specifying-export-options-available-to-media-portal-users}

管理者から権限が付与されている場合、Media Portal ユーザは画像を書き出すときにその形式を変更できます。例えば、サイズ、ファイル形式および画質を変更できます。書き出し時に画像の形式を自動的に変更することで、画像を個別に変換する手間を省き、時間を節約できます。また、管理者はプリセット、つまり事前に選択した画像形式の設定を作成できます。画像の書き出し時にプリセットを使用すると、会社が指定した内容で画像の形式を変更できます。

ユーザー定義の変換を使用して画像アセットを書き出す場合、または元のプライマリ画像を書き出す場合は、次の 2 つの制限が適用されます。

* 書き出しジョブの場合、書き出し用の圧縮 ZIP ファイルの最大ファイルサイズは 1 GB です。
* 書き出しジョブあたり合計 500 個のアセットまで許容されています。

関連トピック [Adobe Dynamic Media Classicからのアセットの書き出し](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Media Portal ユーザーが使用できる書き出しオプションを指定するには：**

1. グローバルナビゲーションバーで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**.
1. 画像プリセットウィンドウで、必要に応じて次のオプションを選択します。

   * **ユーザー定義変換を有効にする**：このオプションを選択すると、ユーザーは次から他を選択できます **[!UICONTROL サイズ]** 選択したアセットを書き出しウィンドウのドロップダウンリスト 次に、ピクセルやセンチメートルなどの測定単位を選択し、目的の幅と高さを指定できます。 ユーザがこれらのファイルを書き出したり、ダウンロードしたりするとき、画像ファイルの形式が変更されます。

     条件 **[!UICONTROL ピクセル]** はから選択されます。 **[!UICONTROL サイズ]** ドロップダウンリストに表示される画像の幅×高さは、1 億ピクセルを超えることはできません。 このサイズは、正方形の画像の場合は 10,000 × 10,000 ピクセル、アスペクト比の 2 x 3 の画像の場合は約 8,000 × 12,000 ピクセルに相当します。 元のプライマリ画像を書き出す場合、このサイズ制限は適用されません。

     ユーザーがダウンロード時にファイルを再フォーマットせずにダウンロードする場合は、このオプションの選択を解除します。

   * **オリジナルを書き出しを有効にする**：元のプライマリ画像を書き出すことができます。 が含まれる **[!UICONTROL 選択したアセットの書き出し]** パネルに追加された、ユーザーは **[!UICONTROL 変換]** ドロップダウンメニューからの選択 **[!UICONTROL オリジナルをエクスポート]** 元のファイルを書き出します。 ユーザが画像を書き出すときに画像プリセットを選択するか、変換オプションを選択することを強制するには、このオプションの選択を解除します。

>[!MORELIKETHIS]
>
>* [画像プリセット](application-setup.md#image_presets)
>* [グループの画像プリセットのアクセス権限の選択](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)
