---
title: クイックスタート：スピンセット
description: Adobe Dynamic Media Classicをすぐに使い始めるのに役立つスピンセットの概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 22%

---

# クイックスタート：スピンセット{#quick-start-spin-sets}

スピンセットを使用することで、現実と同じようにオブジェクトを回転させて確認することができます。つまり、アイテムをあらゆる角度から表示して、特徴的な部分を詳細に確認できるようになります。スピンセットでは、360°の方向からアイテムを表示することができます。Adobe Dynamic Media Classicには、ビューアがアイテムを回転できる 1 次元スピンセットと、ビューアがアイテムを回転および反転できる 2 次元スピンセットが用意されています。 さらに、ユーザーは「フリーフォーム」ズームを使用し、マウスを数回クリックするだけで任意のビューをパンできます。 これらの機能により、特定の方向からアイテムを詳細に確認することができます。

![ スピンセットの画像 ](/help/using/assets/spin_set.png)

スピンセットでは画像マップも使用できます。画像マップとは、スピンセット内の画像上の、テキストを含んだロールオーバーパネルが表示される領域です。ユーザーが画像マップを選択すると、何らかのアクションがトリガーされます。 例えば、ユーザーが製品についてさらに知ることができるように web ページが起動されます。 スピンセット内の画像マップを示すために、ユーザーがマウスポインターを画像マップ上に移動すると、画像マップ自体の周囲にアウトラインが表示されます。

[ 画像マップの作成 ](creating-image-maps.md) を参照してください。

トレーニングビデオの [ 画像セットとスピンセット：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) を参照してください。

スピンセットを作成する場合、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| スピンセットの制限タイプ | ベストプラクティス | 適用される制限 |
| --- | --- | --- |
| 2D セットあたりの最大行数/列数 | 1 セットあたり 12～18 個の画像 | 1000 |

[Dynamic Media の制限 ](/help/using/limitations.md) も参照してください。

このスピンセットクイックスタートは、Adobe Dynamic Media Classicのスピンセット手法をすぐに使い始められるように設計されています。 手順 1 ～ 7 に従ってください。各手順の最後で、トピックリンクを選択して詳細を確認できます。

## 1.画像の作成とアップロード

1 次元スピンセットを使用するには、少なくとも 8 ～ 12 枚の写真が必要で、2 次元スピンセットには 16 ～ 24 枚の写真が必要です。アイテムが回転および反転しているように見せるには、一定の角度間隔でアイテムを撮影する必要があります。例えば、1 次元スピンセットに 12 個の写真を含める場合、アイテムを 30 度ずつ（360/12）回転させながら写真を撮影します。

グローバルナビゲーションバーの **[!UICONTROL アップロード]** を選択して、コンピューターまたはネットワークからAdobe Dynamic Media Classicにスピンイメージをアップロードします。

詳しくは、[スピンセット画像のキャプチャに関するガイドライン](creating-spin-set.md#guidelines-for-shooting-spin-set-images)を参照してください。

## &#x200B;2. スピンセットの作成

スピンセットを作成するには、グローバルナビゲーションバーで **[!UICONTROL ビルド]**/**[!UICONTROL スピンセット]** を選択します。 スピンセットサイズ ダイアログボックスで、行とセルの数を選択して **[!UICONTROL OK]** を選択します。 次に、画像をスピンセットページのグリッドにドラッグします。

[ スピンセットの作成 ](creating-spin-set.md#creating-a-spin-set) を参照してください。

## &#x200B;3. スピンセットの編集

スピンセットを編集するには、グローバルナビゲーションバーで **[!UICONTROL 設定]**/**[!UICONTROL ビューアプリセット]** を選択します。 スピンセットを選択し、「**[!UICONTROL 編集]** を選択します。 画像の追加、削除、位置の変更を行います。2 次元スピンセットの行の位置を変更できます。

[ スピンセットの編集 ](creating-spin-set.md#editing-a-spin-set) を参照してください。

## &#x200B;4. スピンセットビューアプリセットのセットアップ

管理者はスピンセットビューアプリセットを作成できます。これらのプリセットは、スピンセットビューアの外観を決定します。新しいスピンセットビューアプリセットを設定するには、グローバルナビゲーションバーで **[!UICONTROL 設定]**/**[!UICONTROL ビューアプリセット]** に移動します。

ビューアプリセットページで「**[!UICONTROL 追加]**」を選択したあと、ドロップダウンリストから「**[!UICONTROL スピンセットビューア]**」を選択し、「**[!UICONTROL 追加]**」を選択します。 `Configure Viewer` のページでオプションを選択し、「**[!UICONTROL 保存]** を選択します。

[ スピンセットビューアプリセットのセットアップ ](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets) を参照してください。

## &#x200B;5. スピンセットのプレビュー

参照パネルでスピンセットを選択し、「プレビュー **[!UICONTROL を選択し]** す。 プレビューページで、マウスボタンを押しながらポインターを左右にドラッグして、項目を視覚的に「スピン」します。

[ スピンセットのプレビュー ](previewing-spin-set.md#previewing-a-spin-set) を参照してください。

## &#x200B;6. スピンセットの公開

スピンセットを公開すると、Adobe Dynamic Media Classic サーバーに配置されるので、web サイトやアプリケーションに動的に配信できます。 また、Dynamic Media Image Server から Web サイトまたはアプリケーションにスピンセットを呼び出す URL 文字列もアクティベートされます。

スピンセットを公開するには、参照パネルで名前の横にある **[!UICONTROL 公開用にマーク]** アイコンを選択して、公開用にマークします。 グローバルナビゲーションバーの「**[!UICONTROL 公開]**」を選択して公開を開始します。 公開ページで、「**[!UICONTROL 公開を送信]**」を選択します。

[ スピンセットの公開 ](publishing-spin-set.md#publishing-a-spin-set) を参照してください。

## &#x200B;7. Web ページへのスピンセットのリンク

Adobe Dynamic Media Classicは、スピンセットの URL コールアウト文字列を作成し、公開後にアクティブ化します。 これらの URL は、プレビューページからコピーできます。

スピンセットを選択し、「**[!UICONTROL プレビュー]** を選択します。 スピンセットビューアプリセットを選択し、次に、「**[!UICONTROL URL をコピー]**」を選択します。

[Web ページへのスピンセットのリンク ](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page) を参照してください。
