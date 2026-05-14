---
title: クイックスタート：スピンセット
description: Adobe Dynamic Media Classicの概要とクイックスタート スピンセットを使用して、すぐに使い始める方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
autotag-review: '2026-05-13T20:10:31.990Z'
TQID: 'https://experienceleague.adobe.com/dYjjsyvPAPOS5icw4Yi6Kpo93Nh2qvnCiW5-ih2hmDk'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 856
ht-degree: 16%

---

# クイックスタート：スピンセット{#quick-start-spin-sets}

スピンセットを使用することで、現実と同じようにオブジェクトを回転させて確認することができます。 つまり、アイテムをあらゆる角度から表示して、特徴的な部分を詳細に確認できるようになります。 スピンセットでは、360°の方向からアイテムを表示することができます。 Adobe Dynamic Media Classicでは、1次元スピンセットでアイテムを回転させることができます。また、2次元スピンセットでアイテムを回転させたり反転させたりすることもできます。 さらに、ユーザーは数回のマウスをクリックするだけで、任意のビューを「フリーフォーム」でズームおよびパンできます。 これらの機能により、特定の方向からアイテムを詳細に確認することができます。

![&#x200B; スピンセットの画像](/help/using/assets/spin_set.png)

スピニングセットは画像マップも受け入れます。 画像マップは、回転セット内の画像上の領域で、テキスト付きのロールオーバーパネルを表示します。 ユーザーが画像マップを選択すると、何らかのアクションがトリガーされます。 例えば、ユーザーが製品について詳しく知ることができるように、Web ページが起動されます。 スピンセット内の画像マップを指し示すために、ユーザーが画像マップ自体の上にマウスポインターを移動すると、その周りにアウトラインが表示されます。

[画像マップの作成](creating-image-maps.md)を参照してください。

[画像とスピンセット：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)のトレーニングビデオを参照してください。

スピンセットを作成する場合、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| スピンセット制限タイプ | ベストプラクティス | 制限が適用されました |
| --- | --- | --- |
| 2D セットあたりの最大行数/列数 | 12～18枚/セット | 1000 |

[Dynamic Mediaの制限](/help/using/limitations.md)も参照してください。

このクイックスタートは、Adobe Dynamic Media Classicのスピンセットのテクニックを使用して、すばやく起動できるように設計されています。 手順 1 ～ 7 に従ってください。 各ステップの最後に、トピックリンクを選択して詳細を確認できます。

## &#x200B;1. 画像の作成とアップロード

最低でも、1次元スピンセットでは8～12 ショット、2次元スピンセットでは16～24 ショットが必要です。 アイテムが回転および反転しているように見せるには、一定の角度間隔でアイテムを撮影する必要があります。 例えば、1次元スピンセットに12枚のショットが含まれる場合、各ショットに対してアイテムを30°（360/12）回転させます。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」を選択して、コンピューターまたはネットワークからAdobe Dynamic Media Classicにスピンイメージをアップロードします。

詳しくは、[スピンセット画像のキャプチャに関するガイドライン](creating-spin-set.md#guidelines-for-shooting-spin-set-images)を参照してください。

## &#x200B;2. スピンセットの作成

スピンセットを作成するには、グローバルナビゲーションバーで、**[!UICONTROL ビルド]** > **[!UICONTROL スピンセット]**&#x200B;に移動します。 スピンセットサイズダイアログボックスで、必要な行数とセル数を選択し、**[!UICONTROL OK]**&#x200B;を選択します。 次に、画像をスピンセットページのグリッドにドラッグします。

[&#x200B; スピンセットの作成](creating-spin-set.md#creating-a-spin-set)を参照してください。

## &#x200B;3. スピンセットの編集

スピンセットを編集するには、グローバルナビゲーションバーで、**[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**&#x200B;に移動します。 スピンセットを選択し、**[!UICONTROL 編集]**&#x200B;を選択します。 画像の追加、削除、位置の変更を行います。 2次元スピンセットの行の位置を変更できます。

[&#x200B; スピンセットの編集](creating-spin-set.md#editing-a-spin-set)を参照してください。

## &#x200B;4. スピンセットビューアプリセットの設定

管理者はスピンセットビューアプリセットを作成できます。 これらのプリセットは、スピンセットビューアの外観を決定します。 新しいスピンセットビューアプリセットを設定するには、グローバルナビゲーションバーで、**[!UICONTROL セットアップ]** > **[!UICONTROL ビューアプリセット]**&#x200B;に移動します。

ビューアプリセットページで、「**[!UICONTROL 追加]**」を選択し、ドロップダウンリストから「**[!UICONTROL スピンセットビューア]**」を選択して、「**[!UICONTROL 追加]**」を選択します。 `Configure Viewer` ページでオプションを選択し、**[!UICONTROL 保存]**&#x200B;を選択します。

[&#x200B; スピンセットビューアプリセットの設定](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets)を参照してください。

## &#x200B;5. スピンセットのプレビュー

参照パネルでスピンセットを選択し、**[!UICONTROL プレビュー]**&#x200B;を選択します。 プレビューページで、マウスボタンを押しながらポインターを左右にドラッグすると、項目が視覚的に「スピン」します。

[&#x200B; スピンセットのプレビュー](previewing-spin-set.md#previewing-a-spin-set)を参照してください。

## &#x200B;6. スピンセットの公開

スピンセットを公開すると、Adobe Dynamic Media Classic サーバーに配置され、Web サイトやアプリケーションに動的に配信されます。 また、Dynamic Media Image ServerからWeb サイトまたはアプリケーションにスピンセットを呼び出すURL文字列もアクティブ化します。

スピンセットを公開するには、参照パネルで名前の横にある「**[!UICONTROL 公開用にマーク]**」アイコンを選択して、公開用にマークします。 グローバルナビゲーションバーで、**[!UICONTROL 公開]**&#x200B;を選択して公開を開始します。 公開ページで、**[!UICONTROL 公開を送信]**&#x200B;を選択します。

[&#x200B; スピンセットの公開](publishing-spin-set.md#publishing-a-spin-set)を参照してください。

## &#x200B;7. スピンセットをWeb ページにリンクする

Adobe Dynamic Media Classicは、スピンセットのURL コールアウト文字列を作成し、公開した後にアクティブ化します。 プレビューページからこれらのURLをコピーできます。

スピンセットを選択し、**[!UICONTROL プレビュー]**&#x200B;を選択します。 スピンセットビューアプリセットを選択し、 次に、**[!UICONTROL URLをコピー]**&#x200B;を選択します。

[&#x200B; スピンセットをWeb ページにリンクする](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page)を参照してください。
