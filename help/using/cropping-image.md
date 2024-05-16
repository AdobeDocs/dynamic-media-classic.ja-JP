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
source-git-commit: ad7e20fdbe9028c6255865cce95d109f9e9eeab2
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 31%

---

# 画像の切り抜き{#cropping-an-image}

Adobe Dynamic Media Classicで画像を切り抜くことができます。 システムは、切り抜かれた画像に関する情報を保持するので、画像を元の状態に戻すことが可能です。また画像を切り抜き、切り抜かれたバージョンを新しい名前で保存することもできます。

画像を切り抜き、画像の周りの空白を除去したり、画像の領域を切り抜いたりできます。

>[!NOTE]
>
>切り抜いた後、以下を選択できます。 **[!UICONTROL 名前を付けて保存]** 切り抜いた画像を別の名前で保存します。 「名前を付けて保存」ウィンドウで、を選択します。 **[!UICONTROL 新規プライマリとして保存]** ：画像の 2 番目のコピーを保存します。 を選択 **[!UICONTROL プライマリの追加ビューとして保存]** したがって、元のバージョンと切り抜いたバージョンを別の名前で保存できます。 を選択 **[!UICONTROL オリジナルを置換]** 画像の切り抜き元のファイルを削除します。 次に、画像の名前を入力し、を選択します。 **[!UICONTROL Submit]**.

## 画像の周りの空白の除去 {#crop-to-remove-white-space-around-an-image}

画像の端から透明またはべた塗りのピクセルを切り抜くことができます。

1. 画像を切り抜くには、そのロールオーバーを選択します **[!UICONTROL 編集]** ボタンをクリックしてから、を選択します **[!UICONTROL 切り抜き]**&#x200B;または、詳細ビューの参照パネルに表示し、 **[!UICONTROL 切り抜き]** ボタン。
1. 切り抜きエディターページで、次のいずれかの操作を行います。

   * カラーピクセルをトリミングするには、に移動します **[!UICONTROL Trim]** > **[!UICONTROL カラー]**. が含まれる **[!UICONTROL カラーで自動切り抜き]** ダイアログボックスで、 **[!UICONTROL Corner]** メニューをクリックし、切り抜く背景色のコーナーを選択します。 次に、 **[!UICONTROL 許容値]** 0 ～ 1 の範囲で設定します。 0 に設定すると、画像の隅で選択した色と正確に一致するピクセルのみが切り抜かれます。設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。を選択 **[!UICONTROL 切り抜き]**.
   * 透明なピクセルをトリミングするには、に移動します。 **[!UICONTROL Trim]** > **[!UICONTROL 透明]**. が含まれる **[!UICONTROL 透明度による自動切り抜き]** ダイアログ ボックスで、0 ～ 1 の許容差の設定を入力します。 0 を設定すると、ピクセルが透明な場合にのみ切り抜かれます。 設定値が 1 に近づくにつれ、透明度の低いピクセルも切り抜かれるようになります。を選択 **[!UICONTROL 切り抜き]**.

1. を選択 **[!UICONTROL 保存]**.

>[!NOTE]
>
>切り抜いた画像を元の状態に復元するには、切り抜きエディター画面で画像を表示し、以下を選択します。 **[!UICONTROL Reset]**.

## 切り抜き領域の選択 {#select-an-area-to-crop}

1. 画像を切り抜くには、そのロールオーバーを選択します **[!UICONTROL 編集]** ボタンをクリックし、 **[!UICONTROL 切り抜き]**&#x200B;または、詳細ビューの参照パネルに表示して選択します **[!UICONTROL 切り抜き]**.

1. 切り抜きエディターウィンドウで、切り抜きしない画像の部分を切り抜きボックスに配置します。 ボックス内に表示される内容は、選択した後に残ります **[!UICONTROL 保存]** 画像を切り抜きます。
1. 切り抜き領域を調整するには、次のいずれかの操作を行います。

   * ボックスの辺または角をドラッグします。サイズは変更しますが、切り抜きボックスの縦横比（シェイプ）は維持したまま、Shift キーを押しながらドラッグします。
   * 「サイズ」ボックスで、切り抜くサイズをピクセル単位で指定します。
   * ドラッグして切り抜きボックスを移動します。ボックスの境界内でポインタを移動します。ポインタが 4 方向の矢印アイコンに変わったら、ボックスを画面上の移動先の位置にドラッグします。

1. を選択 **[!UICONTROL 保存]**.

>[!NOTE]
>
>切り抜いた画像を元の状態に復元するには、切り抜きエディター画面で画像を表示し、以下を選択します。 **[!UICONTROL Reset]**.

>[!MORELIKETHIS]
>
>* [アップロード時の画像編集のオプション](image-editing-options-upload.md#image-editing-options-at-upload)
>* [PDFファイルから空白を切り抜く](pdfs.md#cropping_white_space_from_a_pdf_file)
>* [PDFページの端から切り抜く](pdfs.md#cropping_from_the_sides_of_pdf_pages)
