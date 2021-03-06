---
title: ガイドズーム用のズームターゲットの作成
description: Dynamic Media ClassicのAdobeでガイドズーム用のズームターゲットを作成する方法を説明します。
uuid: 501ea37b-adc5-4290-87eb-52a3501e5d26
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: e7b4673c-8681-4741-912e-9a31cf106449
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: ffb799ba-1cf1-48e0-91a8-dea758139140
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '728'
ht-degree: 44%

---

# ガイドズーム用のズームターゲットの作成{#creating-zoom-targets-for-guided-zoom}

ズームターゲットにより、画像の特定の部分に注目させることができます。フリーフォームズームに加えて、ビューアはズームターゲットのサムネールを選択し、画像内の焦点を合わせたい部分をズームできます。 ズームターゲットを使用すると、画像の魅力的な部分または特長的な部分を強調することができます。

![ガイドズーム用のズームターゲットの作成](/help/assets/zo_guided_zoom.png)

## ズームターゲットについて {#about-zoom-targets}

ズームターゲットの最大ズーム率は 100 ％です。次の表で示されているように、最小ズーム率はビューアのサイズと画像サイズの組み合わせによって異なります。

| 画像サイズ | ビューアのサイズ | ズーム率 |
| --- | --- | --- |
| 大 | 小 | 最小ズーム率は小さくなる |
| 小 | 大 | 最小ズーム率は大きくなる |

ズームビューアのサイズを変更して、Web ページで使用しているサイズと一致させることができます。この設定を永続的に変更するには、設定画面でビューアのサイズを変更します（管理者のみ実行できます）。[ズームビューアプリセットの設定](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)を参照してください。

## ズームターゲットの作成と編集 {#creating-and-editing-zoom-targets}

ズームターゲットエディタ画面でズームターゲットを作成および編集します。この画面を開くには、画像を選択し、次のいずれかの手順を実行します。

* ロールオーバーの「**[!UICONTROL 編集]**」ボタンを選択し、「ズームターゲット」を選択します。
* 参照パネルで、**[!UICONTROL 詳細ビュー]**&#x200B;に画像を表示し、**[!UICONTROL ズームターゲット]**&#x200B;を選択します。

ズームターゲットエディタ画面で、**[!UICONTROL ターゲットを選択]**&#x200B;ボタン（矢印）を選択して、サイズや位置を変更する前にターゲットを選択します。 画像にズームターゲットを作成するには、「**[!UICONTROL ターゲットを追加]**」（長方形）を選択します。 ズームターゲットエディターページには、ズームターゲットの削除、コピーおよび命名のためのツールも用意されています。

### ズームターゲットの作成 {#creating-a-zoom-target}

ズームターゲットを作成するには、ズームターゲットエディタページを開き、次の操作を行います。

1. 「**[!UICONTROL ターゲットを追加]**」（長方形）を選択し、画像の上にポインターを置き、ズームターゲットにする場所を選択します。

   ズームターゲットのサムネール画像が画面の右側のパネルに表示されます。

1. **[!UICONTROL ターゲットを選択]**（矢印）を選択し、作成したズームターゲットを選択して、ターゲットのサイズと位置を調整します。

   * **サイズ変更**  — ポインターをズームターゲットの隅に移動し、ドラッグしてターゲットを拡大または縮小します。

   * **位置**  — ズームターゲット上にポインターを移動し、別の場所にドラッグします。

1. 「名前」ボックスにズームターゲットの名前を入力します。

   >[!NOTE]
   >
   >「名前」ボックスに入力する内容は名前以上の意味があり、ズームターゲットにポインタを移動すると、「名前」ボックスに入力した内容が表示されます。ズームターゲットの簡単な説明を「名前」ボックスに入力することにより、ユーザはズームできる対象を知ることができます。

1. 必要に応じて、「ユーザデータ」フィールドにユーザデータを入力します。このフィールドは、Web サイトデザイナーがズームターゲットに情報を追加できるように用意されています。
1. 「**[!UICONTROL 保存]**」を選択します。

   ズームターゲットの座標とズームレベルが保存されます。入力した名前とともにズームターゲットのサムネール画像が画面の右側に表示されます。

>[!NOTE]
>
>ズームビューアでズームターゲットがどのように表示されるかを確認するには、ズームターゲットエディタ画面で&#x200B;**[!UICONTROL プレビュー]**&#x200B;ボタンを選択し、プレビュー画面でズームビューアを選択します。 この画面について詳しくは、[様々なズームビューアで画像をプレビューする](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)を参照してください。

### ズームターゲットの編集 {#editing-zoom-targets}

ズームターゲットを編集するには、ズームターゲットエディタページで次の手法を使用します。

* **再配置**  — ターゲットを選択ボタン（矢印）を使用して、ターゲットを選択します。次に、ターゲットを別の位置にドラッグします。

* **サイズ変更**  — ターゲットを選択ボタン（矢印）を使用して、ターゲットを選択します。ターゲットを拡大または縮小するには、ズームターゲットの角にポインタを移動してドラッグします。

* **削除**  — 画面の右側でターゲットのサムネール画像を選択します。次に、「**[!UICONTROL ターゲットを削除]**」を選択します。

* **名前の変更**  — 画面の右側でターゲットのサムネール画像を選択します。次に、「**[!UICONTROL 名前]**」テキストフィールドに名前を入力し、「**[!UICONTROL 保存]**」を選択します。

### ズームターゲットのコピー {#copying-zoom-targets}

ある画像から別の画像にズームターゲットをコピーすることができます。2 つの画像に同様のコンテンツが表示され、ズームターゲットが同じ位置に属しているようにするには、ターゲットをコピーします。ズームターゲットを別の画像にコピーするには、次の操作を行います。

1. ズームターゲットエディタ画面で、コピーするズームターゲットを含む画像を開きます。
1. **[!UICONTROL Copy Targets To]**&#x200B;を選択します。
1. [イメージを選択]ダイアログボックスで、イメージを選択し、[**[!UICONTROL 選択]**]を選択します。
