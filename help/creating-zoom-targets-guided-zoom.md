---
title: ガイドズーム用のズームターゲットの作成
seo-title: ガイドズーム用のズームターゲットの作成
description: 'null'
seo-description: ガイドズーム用のズームターゲットを作成する方法について説明します。
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: 管理者
content-type: 参照
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# ガイドズーム用のズームターゲットの作成{#creating-zoom-targets-for-guided-zoom}

ズームターゲットにより、画像の特定の部分に注目させることができます。通常のズーム機能のほかにズームターゲットを設定することで、ズームターゲットのサムネールをクリックして画像の特定の部分をズームさせることができます。ズームターゲットを使用すると、画像の魅力的な部分または特長的な部分を強調することができます。

![ガイドズーム用のズームターゲットの作成](/help/assets/zo_guided_zoom.png)

## ズームターゲットについて {#about-zoom-targets}

ズームターゲットの最大ズーム率は 100 ％です。次の表で示されているように、最小ズーム率はビューアのサイズと画像サイズの組み合わせによって異なります。

| 画像サイズ | ビューアのサイズ | ズーム率 |
|--- |--- |--- |
| 大 | 小 | 最小ズーム率は小さくなる |
| 小 | 大 | 最小ズーム率は大きくなる |

ズームビューアのサイズを変更して、Web ページで使用しているサイズと一致させることができます。この設定を永続的に変更するには、設定画面でビューアのサイズを変更します（管理者のみ実行できます）。詳しくは、[ズームビューアプリセットの設定](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)を参照してください。

## ズームターゲットの作成と編集 {#creating-and-editing-zoom-targets}

ズームターゲットエディタ画面でズームターゲットを作成および編集します。この画面を開くには、画像を選択し、次のいずれかの手順を実行します。

* Click the rollover **[!UICONTROL Edit]** button and choose Zoom Targets.
* In the Browse Panel, display the image in **[!UICONTROL Detail View]**, then click **[!UICONTROL Zoom Targets]**.

On the Zoom Target Editor screen, click **[!UICONTROL Select Target]** button (arrow) to select a target before changing its size or position. Click **[!UICONTROL Add Targets]** (rectangle) to create a zoom target on the image. ズームターゲットエディタ画面には、ズームターゲットの削除、コピーおよび名前付けを行うツールもあります。

### ズームターゲットの作成 {#creating-a-zoom-target}

ズームターゲットエディタ画面を開き、次の手順に従ってズームターゲットを作成します。

1. Click **[!UICONTROL Add Targets]** (rectangle), move the pointer over the image, and click where you want to the zoom target to be.

   ズームターゲットのサムネール画像が画面の右側のパネルに表示されます。

1. Click **[!UICONTROL Select Target]** (arrow), click to select the zoom target you created, and adjust the size and position of the target.

   * **サイズ変**&#x200B;更ズームターゲットの隅にポインタを合わせ、ドラッグしてターゲットを拡大または縮小します。

   * **位置ズ**&#x200B;ームターゲット上にポインタを移動し、別の位置にドラッグします。

1. 「名前」ボックスにズームターゲットの名前を入力します。

   >[!NOTE]
   >
   >「名前」ボックスに入力する内容は名前以上の意味があり、ズームターゲットにポインタを移動すると、「名前」ボックスに入力した内容が表示されます。ズームターゲットの簡単な説明を「名前」ボックスに入力することにより、ユーザはズームできる対象を知ることができます。

1. 必要に応じて、「ユーザデータ」フィールドにユーザデータを入力します。このフィールドは、Web サイトデザイナーがズームターゲットに情報を追加できるように用意されています。
1. Click **[!UICONTROL Save]**.

   ズームターゲットの座標とズームレベルが保存されます。入力した名前とともにズームターゲットのサムネール画像が画面の右側に表示されます。

>[!NOTE]
>
>ズームビューアでズームターゲットの外観を確認するには、ズームターゲットエディタ画面で「プレビュー」ボタンをクリックし、プレビュー画面の「ズームビューア」を選択します。この画面については、[様々なズームビューアでの画像のプレビュー](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)を参照してください。

### ズームターゲットの編集 {#editing-zoom-targets}

ズームターゲットを編集するには、ズームターゲットエディタ画面で次の手順を実行します。

* **再配置**&#x200B;ターゲットを選択ボタン（矢印）で、ターゲットをクリックして選択します。 次に、ターゲットを別の位置にドラッグします。

* **サイズ**&#x200B;変更「ターゲットを選択」ボタン（矢印）を使用して、ターゲットをクリックして選択します。 ポインタをズームターゲットの隅に移動し、ドラッグしてターゲットを拡大または縮小します。

* **削除**&#x200B;画面の右側で、ターゲットのサムネール画像をクリックします。 次に、「ターゲット **[!UICONTROL を削除」をクリックしま]**&#x200B;す。

* **名前の**&#x200B;変更画面の右側で、ターゲットのサムネール画像をクリックします。 Then enter a name in the **[!UICONTROL Name]** text field and click **[!UICONTROL Save]**.

### ズームターゲットのコピー {#copying-zoom-targets}

ある画像から別の画像にズームターゲットをコピーすることができます。2 つの画像に同様のコンテンツが表示され、ズームターゲットが同じ位置に属しているようにするには、ターゲットをコピーします。ズームターゲットを別の画像にコピーするには、次の手順に従います。

1. ズームターゲットエディタ画面で、コピーするズームターゲットを含む画像を開きます。
1. 「ターゲット **[!UICONTROL のコピー先」をクリックしま]**&#x200B;す。
1. In the Select Images dialog box, select an image and click **[!UICONTROL Select]**.

