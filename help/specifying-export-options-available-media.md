---
title: Media Portal ユーザが使用できる書き出しオプションの指定
description: Adobe Dynamic Media Classicで Media Portal ユーザーが使用できる書き出しオプションを指定する方法について説明します。
uuid: 5258b8a4-0704-43cd-97d1-c9af2e4e298b
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
discoiquuid: 9bfd95da-3714-4e38-98af-331a04c685f5
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: c27df6c2-76f4-441c-bd26-cee98203291e
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 61%

---

# Media Portal ユーザが使用できる書き出しオプションの指定 {#specifying-export-options-available-to-media-portal-users}

管理者から権限が付与されている場合、Media Portal ユーザは画像を書き出すときにその形式を変更できます。例えば、サイズ、ファイル形式および画質を変更できます。書き出し時に画像の形式を自動的に変更することで、画像を個別に変換する手間を省き、時間を節約できます。また、管理者はプリセット、つまり事前に選択した画像形式の設定を作成できます。画像の書き出し時にプリセットを使用すると、会社が指定した内容で画像の形式を変更できます。

ユーザー定義変換を使用して画像アセットを書き出す場合、または元のプライマリ画像を書き出す場合は、次の 2 つの制限が適用されます。

* 書き出しジョブの場合、書き出し用の圧縮 ZIP ファイルの最大ファイルサイズは 1 GB です。
* 書き出しジョブあたり合計 500 個のアセットまで許容されています。

関連トピック [Adobe Dynamic Media Classicからのアセットの書き出し](exporting-assets-from-dmc.md#exporting-assets-from_dmc).

**Media Portal ユーザが使用できる書き出しオプションを指定するには:**

1. グローバルナビゲーションバーで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**.
1. 画像プリセットウィンドウで、必要に応じて次のオプションを選択します。

   * **ユーザ定義コンバージョンの有効化**  — このオプションを選択すると、ユーザーは、 **[!UICONTROL サイズ]** 選択したアセットを書き出しウィンドウのドロップダウンリスト。 次に、ユーザはピクセルまたはセンチメートルなどの測定単位を選択して、希望の幅と高さを指定できます。ユーザがこれらのファイルを書き出したり、ダウンロードしたりするとき、画像ファイルの形式が変更されます。

      **[!UICONTROL サイズ]**&#x200B;ドロップダウンリストから **[!UICONTROL pixel]** が選択されている場合、画像の幅 × 高さ は 1 億 pixel を超えることはできません。このサイズは 10,000 × 10,000 pixel の画像（正方形）または 8,000 × 12,000 pixel の画像（縦横比 2x3）と同一です。このサイズ制限は、元のプライマリ画像を書き出す場合は適用されません。

      ダウンロードするときにファイルの形式を変更せずに、ファイルをダウンロードできるようにするには、このオプションの選択を解除します。

   * **オリジナルの書き出しを有効にする** ：オリジナルのプライマリ画像を書き出すことができます。 内 **[!UICONTROL 選択したアセットを書き出し]** パネルを開くと、 **[!UICONTROL コンバージョン]** ドロップダウンメニューで「 **[!UICONTROL オリジナルを書き出し]** 元のファイルを書き出すには 画像の書き出し時にユーザーが画像プリセットを選択するか、変換オプションを選択するように強制する場合は、このオプションの選択を解除します。

>[!MORELIKETHIS]
>
>* [画像プリセット](application-setup.md#image_presets)
>* [グループの画像プリセットへのアクセス権限の選択](creating-media-portal-groups.md#choosing_image_preset_access_permissions_for_a_group)

