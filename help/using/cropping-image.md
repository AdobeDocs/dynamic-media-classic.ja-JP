---
title: 画像の切り抜き
description: Adobe Dynamic Media Classicでの画像の切り抜き方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 31%

---

# 画像の切り抜き{#cropping-an-image}

Adobe Dynamic Media Classicで画像を切り抜くことができます。 システムは、切り抜かれた画像に関する情報を保持するので、画像を元の状態に戻すことが可能です。また画像を切り抜き、切り抜かれたバージョンを新しい名前で保存することもできます。

画像を切り抜き、画像の周りの空白を除去したり、画像の領域を切り抜いたりできます。

>[!NOTE]
>
>切り抜いた後、「**[!UICONTROL 名前を付けて保存]** を選択して、切り抜いた画像を別の名前で保存できます。 「名前を付けて保存」ウィンドウで、「**[!UICONTROL 新規プライマリとして保存]**」を選択して、イメージの 2 番目のコピーを保存します。 「**[!UICONTROL プライマリの追加ビューとして保存]**」を選択すると、元のビューと切り抜いたビューを別の名前で保存できます。 「**[!UICONTROL 元の画像を置換]**」を選択して、画像を切り抜いた元のファイルを削除します。 次に、画像の名前を入力し、「**[!UICONTROL 送信]**」を選択します。

## 画像の周りの空白の除去 {#crop-to-remove-white-space-around-an-image}

画像の端から透明またはべた塗りのピクセルを切り抜くことができます。

1. 画像を切り抜くには、ロールオーバー **[!UICONTROL 編集]** ボタンを選択してから **[!UICONTROL 切り抜き]** を選択するか、詳細ビューの参照パネルで画像を表示して **[!UICONTROL 切り抜き]** ボタンを選択します。
1. 切り抜きエディターページで、次のいずれかの操作を行います。

   * カラーピクセルをトリミングするには、**[!UICONTROL トリミング]**/**[!UICONTROL カラー]** に移動します。 **[!UICONTROL カラーによる自動切り抜き]** ダイアログボックスで、**[!UICONTROL 隅]** メニューを選択し、背景色で切り抜く隅を選択します。 次に、0 ～ 1 の **[!UICONTROL 公差]** 設定を入力します。 0 に設定すると、画像の隅で選択した色と正確に一致するピクセルのみが切り抜かれます。設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。**[!UICONTROL 切り抜き]** を選択します。
   * 透明なピクセルをトリミングするには、**[!UICONTROL トリミング]**/**[!UICONTROL 透明]** に移動します。 **[!UICONTROL 透明度による自動切り抜き]** ダイアログボックスで、0 ～ 1 の許容範囲設定を入力します。 0 を設定すると、ピクセルが透明な場合にのみ切り抜かれます。 設定値が 1 に近づくにつれ、透明度の低いピクセルも切り抜かれるようになります。**[!UICONTROL 切り抜き]** を選択します。

1. **[!UICONTROL 保存]** を選択します。

>[!NOTE]
>
>切り抜いた画像を元の状態に復元するには、切り抜きエディター画面で画像を表示して「**[!UICONTROL リセット]**」を選択します。

## 切り抜き領域の選択 {#select-an-area-to-crop}

1. 画像を切り抜くには、ロールオーバー **[!UICONTROL 編集]** ボタンを選択し、**[!UICONTROL 切り抜き]** を選択するか、詳細ビューの参照パネルで画像を表示して **[!UICONTROL 切り抜き]** を選択します。

1. 切り抜きエディターウィンドウで、切り抜きしない画像の部分を切り抜きボックスに配置します。 ボックス内に表示されるものは、「保存 **[!UICONTROL を選択して画像を切り抜いた後に残]** ものです。
1. 切り抜き領域を調整するには、次のいずれかの操作を行います。

   * ボックスの辺または角をドラッグします。サイズは変更しますが、切り抜きボックスの縦横比（シェイプ）は維持したまま、Shift キーを押しながらドラッグします。
   * 「サイズ」ボックスで、切り抜くサイズをピクセル単位で指定します。
   * ドラッグして切り抜きボックスを移動します。ボックスの境界内でポインタを移動します。ポインタが 4 方向の矢印アイコンに変わったら、ボックスを画面上の移動先の位置にドラッグします。

1. **[!UICONTROL 保存]** を選択します。

>[!NOTE]
>
>切り抜いた画像を元の状態に復元するには、切り抜きエディター画面で画像を表示して「**[!UICONTROL リセット]**」を選択します。

>[!MORELIKETHIS]
>
>* [ アップロード時の画像編集のオプション ](image-editing-options-upload.md#image-editing-options-at-upload)
>* [PDF ファイルから空白を切り抜く ](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [PDFページの端から切り抜く ](pdfs.md#cropping_from_the_sides_of_pdf_pages)
