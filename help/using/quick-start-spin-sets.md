---
title: 「クイックスタート：スピンセット」
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
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 25%

---

# クイックスタート：スピンセット{#quick-start-spin-sets}

スピンセットを使用することで、現実と同じようにオブジェクトを回転させて確認することができます。つまり、アイテムをあらゆる角度から表示して、特徴的な部分を詳細に確認できるようになります。スピンセットでは、360°の方向からアイテムを表示することができます。Adobe Dynamic Media Classicには、ビューアがアイテムを回転できる 1 次元スピンセットと、ビューアがアイテムを回転および反転できる 2 次元スピンセットが用意されています。 さらに、ユーザーは「フリーフォーム」ズームを使用し、マウスを数回クリックするだけで任意のビューをパンできます。 これらの機能により、特定の方向からアイテムを詳細に確認することができます。

![スピンセットの画像。](/help/using/assets/spin_set.png)

スピンセットでは画像マップも使用できます。画像マップとは、スピンセット内の画像上の、テキストを含んだロールオーバーパネルが表示される領域です。ユーザーが画像マップを選択すると、何らかのアクションがトリガーされます。 例えば、製品の詳細を説明した Web ページが起動します。スピンセット内の画像マップを示すために、ユーザーがマウスポインターを画像マップ上に移動すると、画像マップ自体の周囲にアウトラインが表示されます。

参照： [画像マップの作成](creating-image-maps.md).

参照： [画像およびスピンセット：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

スピンセットを作成する場合、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| スピンセットの制限タイプ | ベストプラクティス | 適用される制限 |
| --- | --- | --- |
| 2D セットあたりの最大行数/列数 | 1 セットあたり 12～18 個の画像 | 1000 |

関連トピック [Dynamic Mediaの制限](/help/using/limitations.md).

このスピンセットクイックスタートは、Adobe Dynamic Media Classicのスピンセット手法をすぐに使い始められるように設計されています。 手順 1 ～ 7 に従ってください。各手順の最後で、トピックリンクを選択して詳細を確認できます。

## 1.画像の作成とアップロード

1 次元スピンセットを使用するには、少なくとも 8 ～ 12 枚の写真が必要で、2 次元スピンセットには 16 ～ 24 枚の写真が必要です。アイテムが回転および反転しているように見せるには、一定の角度間隔でアイテムを撮影する必要があります。例えば、1 次元スピンセットに 12 個の写真を含める場合、アイテムを 30 度ずつ（360/12）回転させながら写真を撮影します。

グローバルナビゲーションバーで、を選択します。 **[!UICONTROL Upload]** （コンピューターまたはネットワークからAdobe Dynamic Media Classicにスピンイメージをアップロードする場合）

詳しくは、[スピンセット画像のキャプチャに関するガイドライン](creating-spin-set.md#guidelines-for-shooting-spin-set-images)を参照してください。

## 2. スピンセットの作成

スピンセットを作成するには、グローバルナビゲーションバーで以下に移動します **[!UICONTROL ビルド]** > **[!UICONTROL スピンセット]**. スピンセットサイズ ダイアログボックスで、行とセルの数を選択して選択します **[!UICONTROL OK]**. 次に、スピンセットページ上のグリッドに画像をドラッグします。

参照： [スピンセットの作成](creating-spin-set.md#creating-a-spin-set).

## 3. スピンセットの編集

スピンセットを編集するには、グローバルナビゲーションバーで以下に移動します **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**. スピンセットを選択してから、を選択します **[!UICONTROL 編集]**. 画像の追加、削除、位置の変更を行います。2 次元スピンセットでは、行の位置を変更することもできます。

参照： [スピンセットの編集](creating-spin-set.md#editing-a-spin-set).

## 4. スピンセットビューアプリセットのセットアップ

管理者はスピンセットビューアプリセットを作成できます。これらのプリセットは、スピンセットビューアの外観を決定します。新しいスピンセットビューアプリセットを設定するには、グローバルナビゲーションバーで以下に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.

ビューアプリセットページで、次のオプションを選択します **[!UICONTROL 追加]**&#x200B;を選択してから、 **[!UICONTROL スピンセットビューア]** ドロップダウンリストから「」を選択し、 **[!UICONTROL 追加]**. でオプションを選択します `Configure Viewer` ページを選択してから、を選択します **[!UICONTROL 保存]**.

参照： [スピンセットビューアプリセットの設定](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5. スピンセットのプレビュー

参照パネルでスピンセットを選択してから、選択します **[!UICONTROL プレビュー]**. プレビューページで、マウスボタンを押しながらポインターを左右にドラッグして、項目を視覚的に「スピン」します。

参照： [スピンセットのプレビュー](previewing-spin-set.md#previewing-a-spin-set).

## 6. スピンセットの公開

スピンセットを公開すると、Adobe Dynamic Media Classic サーバーに配置されるので、web サイトやアプリケーションに動的に配信できます。 また、Dynamic Media Image Server から Web サイトまたはアプリケーションにスピンセットを呼び出す URL 文字列もアクティベートされます。

スピンセットを公開するには、スピンセットに公開用のマークを付けます **[!UICONTROL 公開用にマーク]** 参照パネルで名前の横にあるアイコン。 グローバルナビゲーションバーで、を選択します。 **[!UICONTROL 公開]** をクリックして公開を開始します。 公開ページで、を選択します。 **[!UICONTROL 公開を送信]**.

参照： [スピンセットの公開](publishing-spin-set.md#publishing-a-spin-set).

## 7. Web ページへのスピンセットのリンク

Adobe Dynamic Media Classicは、スピンセットの URL コールアウト文字列を作成し、公開後にアクティブ化します。 これらの URL は、プレビューページからコピーできます。

スピンセットを選択してから、を選択します **[!UICONTROL プレビュー]**. スピンセットビューアプリセットを選択し、次に、を選択します **[!UICONTROL URL をコピー]**.

参照： [Web ページへのスピンセットのリンク](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
