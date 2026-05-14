---
title: 画像の切り抜き
description: Adobe Dynamic Media Classicで画像をトリミングする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:43:15.888Z'
TQID: 'https://experienceleague.adobe.com/ocIRAbDQHlduym6sy-qxPpXaD-UZJp6jzjV758oduZw'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 560
ht-degree: 32%

---

# 画像の切り抜き{#cropping-an-image}

Adobe Dynamic Media Classicで画像をトリミングできます。 システムは、切り抜かれた画像に関する情報を保持するので、画像を元の状態に戻すことが可能です。 また画像を切り抜き、切り抜かれたバージョンを新しい名前で保存することもできます。

画像を切り抜き、画像の周りの空白を除去したり、画像の領域を切り抜いたりできます。

>[!NOTE]
>
>切り抜き後、**[!UICONTROL 別名で保存]**&#x200B;を選択し、切り抜いたバージョンの画像を別の名前で保存できます。 名前を付けて保存ウィンドウで、**[!UICONTROL 新しいプライマリとして保存]**&#x200B;を選択して、画像の2番目のコピーを保存します。 「**[!UICONTROL 追加ビューとしてプライマリ]**&#x200B;として保存」を選択すると、元の画像と切り抜いた画像を別の名前で保存できます。 「**[!UICONTROL オリジナルを置換]**」を選択して、画像をトリミングした元のファイルを削除します。 次に、画像の名前を入力し、**[!UICONTROL 送信]**&#x200B;を選択します。

## 画像の周りの空白の除去 {#crop-to-remove-white-space-around-an-image}

画像の端から透明またはべた塗りのピクセルを切り抜くことができます。

1. 画像を切り抜くには、そのロールオーバー&#x200B;**[!UICONTROL 編集]** ボタンを選択し、**[!UICONTROL 切り抜き]**&#x200B;を選択するか、詳細表示の参照パネルに表示して、**[!UICONTROL 切り抜き]** ボタンを選択します。
1. 切り抜きエディターページで、次のいずれかの操作を行います。

   * カラーピクセルをトリミングするには、**[!UICONTROL トリミング]** > **[!UICONTROL カラー]**&#x200B;に移動します。 **[!UICONTROL カラーで自動切り抜き]** ダイアログボックスで、**[!UICONTROL コーナー]** メニューを選択し、切り抜く背景色のコーナーを選択します。 次に、**[!UICONTROL 許容値]**&#x200B;の設定を0 ～ 1の範囲で入力します。 0 に設定すると、画像の隅で選択した色と正確に一致するピクセルのみが切り抜かれます。 設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。 「**[!UICONTROL 切り抜き]**」を選択します。
   * 透明ピクセルをトリミングするには、**[!UICONTROL トリミング]** > **[!UICONTROL 透明]**&#x200B;に移動します。 **[!UICONTROL 透明部分で自動切り抜き]** ダイアログボックスで、0 ～ 1の許容値の設定を入力します。 「0」を設定すると、透明なピクセルのみが切り抜かれます。 設定値が 1 に近づくにつれ、透明度の低いピクセルも切り抜かれるようになります。 「**[!UICONTROL 切り抜き]**」を選択します。

1. **[!UICONTROL 保存]**&#x200B;を選択します。

>[!NOTE]
>
>画像を切り抜いた後に元の状態に戻すには、切り抜きエディター画面に画像を表示し、**[!UICONTROL リセット]**&#x200B;を選択します。

## 切り抜き領域の選択 {#select-an-area-to-crop}

1. 画像を切り抜くには、そのロールオーバー&#x200B;**[!UICONTROL 編集]** ボタンを選択し、**[!UICONTROL 切り抜き]**&#x200B;を選択するか、詳細表示の参照パネルに表示して、**[!UICONTROL 切り抜き]**&#x200B;を選択します。

1. 切り抜きエディターウィンドウで、切り抜きたい画像の一部を切り抜きボックスに配置します。 ボックス内に表示される内容は、**[!UICONTROL 保存]**&#x200B;を選択して画像を切り抜いた後に残ります。
1. 切り抜き領域を調整するには、次のいずれかの操作を行います。

   * ボックスの辺または角をドラッグします。 Shift キーを押しながらドラッグすると、サイズは変更されますが、切り抜きボックスの縦横比（シェイプ）は維持されます。
   * 「サイズ」ボックスで、切り抜くサイズをピクセル単位で指定します。
   * ドラッグして切り抜きボックスを移動します。 ボックスの境界内でポインタを移動します。 ポインタが 4 方向の矢印アイコンに変わったら、ボックスを画面上の移動先の位置にドラッグします。

1. **[!UICONTROL 保存]**&#x200B;を選択します。

>[!NOTE]
>
>画像を切り抜いた後に元の状態に戻すには、切り抜きエディター画面に画像を表示し、**[!UICONTROL リセット]**&#x200B;を選択します。

>[!MORELIKETHIS]
>
>* [ アップロード時の画像編集オプション ](image-editing-options-upload.md#image-editing-options-at-upload)
>* [PDF ファイルから空白を切り抜く](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [PDF ページの横から切り抜く](pdfs.md#cropping_from_the_sides_of_pdf_pages)
