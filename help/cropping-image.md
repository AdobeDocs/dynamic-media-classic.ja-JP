---
title: 画像の切り抜き
description: 画像の切り抜き方法を説明します。
uuid: 84f199de-cbfc-4d06-877f-6e9148e82e15
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
discoiquuid: 99dfa476-4f11-4569-a27e-a76ed7787674
feature: Dynamic Media Classic，アセット管理
role: User
exl-id: aec4c256-f5ed-4307-afec-dec848be95f9
source-git-commit: 7be3f63bfadeafa71eeb2567f982f579ccb85975
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 39%

---

# 画像の切り抜き{#cropping-an-image}

Dynamic Media Classicで画像の切り抜きが可能です。 システムは、切り抜かれた画像に関する情報を保持するので、画像を元の状態に戻すことが可能です。また画像を切り抜き、切り抜かれたバージョンを新しい名前で保存することもできます。

画像を切り抜き、画像の周りの空白を除去したり、画像の領域を切り抜いたりできます。

>[!NOTE]
>
>切り抜いた後、「**[!UICONTROL 名前を付けて保存]**」を選択して、切り抜いたバージョンの画像を別の名前で保存できます。 「名前を付けて保存」ウィンドウで、「新しいマスターとして保存」を選択すると、元の画像の 2 番目のコピーとして保存されます。「**[!UICONTROL マスターの追加表示として保存]**」を選択すると、元のバージョンと切り抜いたバージョンを別の名前で保存できます。 「**[!UICONTROL オリジナルを置換]**」を選択すると、画像を切り抜いた元のファイルが削除されます。 次に、画像の名前を入力し、「**[!UICONTROL 送信]**」を選択します。

## 画像の周りの空白の除去 {#crop-to-remove-white-space-around-an-image}

画像の端から透明またはべた塗りのピクセルを切り抜くことができます。

1. 画像を切り抜くには、ロールオーバーの&#x200B;**[!UICONTROL 編集]**&#x200B;ボタンを選択して&#x200B;**[!UICONTROL 切り抜き]**&#x200B;を選択するか、詳細ビューの参照パネルで画像を表示して&#x200B;**[!UICONTROL 切り抜き]**&#x200B;ボタンを選択します。
1. 切り抜きエディターページで、次のいずれかの操作を行います。

   * カラーピクセルをトリミングするには、**[!UICONTROL Trim]** > **[!UICONTROL Color]**&#x200B;に移動します。 **[!UICONTROL 色で自動切り抜き]**&#x200B;ダイアログボックスで、**[!UICONTROL 角]**&#x200B;メニューを選択し、切り抜く背景色の角を選択します。 次に、0 ～ 1の&#x200B;**[!UICONTROL 許容値]**&#x200B;設定を入力します。 0 に設定すると、画像の隅で選択した色と正確に一致するピクセルのみが切り抜かれます。設定値が 1 に近づくにつれ、許容される色の違いが大きくなります。「**[!UICONTROL 切り抜き]**」を選択します。
   * 透明なピクセルをトリミングするには、**[!UICONTROL Trim]** > **[!UICONTROL Transparent]**&#x200B;に移動します。 [**[!UICONTROL 透明度で自動切り抜き]**]ダイアログボックスで、0 ～ 1の許容値を入力します。 0を設定すると、ピクセルが透明な場合にのみ切り抜かれます。 設定値が 1 に近づくにつれ、透明度の低いピクセルも切り抜かれるようになります。「**[!UICONTROL 切り抜き]**」を選択します。

1. 「**[!UICONTROL 保存]**」を選択します。

>[!NOTE]
>
>切り抜いた画像を元の状態に戻すには、切り抜きエディタ画面で画像を表示し、「**[!UICONTROL リセット]**」を選択します。

## 切り抜き領域の選択 {#select-an-area-to-crop}

1. 画像を切り抜くには、ロールオーバーの&#x200B;**[!UICONTROL 編集]**&#x200B;ボタンを選択して「**[!UICONTROL 切り抜き]**」を選択するか、詳細ビューの参照パネルに表示して「**[!UICONTROL 切り抜き]**」を選択します。

1. 切り抜きエディタ(Crop Editor)ウィンドウで、切り抜く画像の一部を切り抜きボックスに配置します。 ボックス内に表示される内容は、「**[!UICONTROL 保存]**」を選択して画像を切り抜いた後に残る内容です。
1. 切り抜き領域を調整するには、次のいずれかの操作を行います。

   * ボックスの辺または角をドラッグします。切り抜きボックスの縦横比（形状）を維持しながらサイズを変更するには、Shift キーを押しながらドラッグします。
   * 「サイズ」ボックスで、切り抜くサイズをピクセル単位で指定します。
   * ドラッグして切り抜きボックスを移動します。ボックスの境界内でポインタを移動します。ポインタが 4 方向の矢印アイコンに変わったら、ボックスを画面上の移動先の位置にドラッグします。

1. 「**[!UICONTROL 保存]**」を選択します。

>[!NOTE]
>
>切り抜いた画像を元の状態に戻すには、切り抜きエディタ画面で画像を表示し、「**[!UICONTROL リセット]**」を選択します。

>[!MORELIKETHIS]
>
>* [アップロード時の画像編集のオプション](image-editing-options-upload.md#image-editing-options-at-upload)
* [PDFファイルからの空白の切り抜き](pdfs.md#cropping_white_space_from_a_pdf_file)
* [PDFページの端からの切り抜き](pdfs.md#cropping_from_the_sides_of_pdf_pages)

