---
title: '"クイックスタート：スピンセット"'
description: Adobe Dynamic Media Classicをすばやく使い始めるのに役立つ、概要とスピンセットのクイックスタートです。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 92a28b7868e03802f4ef1c113ec3f8b34f57ed56
workflow-type: tm+mt
source-wordcount: '838'
ht-degree: 22%

---

# クイックスタート：スピンセット{#quick-start-spin-sets}

スピンセットを使用することで、現実と同じようにオブジェクトを回転させて確認することができます。つまり、アイテムをあらゆる角度から表示して、特徴的な部分を詳細に確認できるようになります。スピンセットは、360°の表示エクスペリエンスをシミュレートします。 Adobe Dynamic Media Classicには、ビューアが項目を回転できる 1 次元スピンセットと、ビューアが項目を回転および反転できる 2 次元スピンセットが用意されています。 さらに、ユーザは、マウスで数回クリックするだけで、任意のビューを「自由形式」でズームおよびパンできます。 これらの機能により、特定の方向からアイテムを詳細に確認することができます。

![スピンセット用の画像.](/help/assets/spin_set.png)

スピンセットでは画像マップも使用できます。画像マップとは、スピンセット内の画像上の、テキストを含んだロールオーバーパネルが表示される領域です。ユーザが画像マップをクリックすると、何らかのアクションがトリガされます。例えば、製品の詳細を説明した Web ページが起動します。スピンセット内の画像マップを指すように、ユーザがマウスポインタを画像マップ上に移動すると、画像マップ自体の周囲にアウトラインが表示されます。

詳しくは、 [画像マップを作成](creating-image-maps.md).

詳しくは、 [画像およびスピンセット：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

スピンセットを作成する場合、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| スピンセットの制限の種類 | ベストプラクティス | 制限が適用されました |
| --- | --- | --- |
| 2D セットあたりの最大行数/列数 | 1 セットあたり 12～18 個の画像 | 1000 |

関連トピック [Dynamic Mediaの制限](/help/limitations.md).

このスピンセットのクイックスタートは、Adobe Dynamic Media Classicのスピンセットのテクニックをすばやく習得して実行できるように作られています。 手順 1 ～ 7 に従ってください。各手順の最後に、トピックリンクを選択して詳細を確認できます。

## 1.画像を作成してアップロードします

1 次元スピンセットの場合は 8 ～ 12 回、2 次元スピンセットの場合は 16 ～ 24 回の写真が必要です。 アイテムが回転および反転しているように見せるには、一定の角度間隔でアイテムを撮影する必要があります。例えば、1 次元のスピンセットに 12 個のショットが含まれている場合、各ショットのアイテムを 30° (360°/12) 回転します。

グローバルナビゲーションバーで、 **[!UICONTROL アップロード]** を使用して、お使いのコンピューターまたはネットワークからAdobe Dynamic Media Classicにスピン画像をアップロードします。

詳しくは、[スピンセット画像のキャプチャに関するガイドライン](creating-spin-set.md#guidelines-for-shooting-spin-set-images)を参照してください。

## 2.スピンセットを作成する

スピンセットを作成するには、グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL スピンセット]**. スピンセットのサイズダイアログボックスで、必要な行数とセル数を選択し、「 **[!UICONTROL OK]**. 次に、画像をスピンセットページのグリッドにドラッグします。

詳しくは、 [スピンセットの作成](creating-spin-set.md#creating-a-spin-set).

## 3.スピンセットを編集する

スピンセットを編集するには、グローバルナビゲーションバーで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**. スピンセットを選択し、「 」を選択します。 **[!UICONTROL 編集]**. 画像の追加、削除、位置の変更を行います。2 次元スピンセットでは、行の位置を変更することもできます。

詳しくは、 [スピンセットの編集](creating-spin-set.md#editing-a-spin-set).

## 4.スピンセットビューアプリセットを設定する

管理者はスピンセットビューアプリセットを作成できます。これらのプリセットは、スピンセットビューアの外観を決定します。新しいスピンセットビューアプリセットを設定するには、グローバルナビゲーションバーで次の場所に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.

ビューアプリセットページで、「 」を選択します **[!UICONTROL 追加]**&#x200B;を選択し、「 **[!UICONTROL スピンセットビューア]** ドロップダウンリストから、 **[!UICONTROL 追加]**. ビューアを設定ページでオプションを選択し、「 **[!UICONTROL 保存]**.

詳しくは、 [スピンセットビューアプリセットの設定](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets).

## 5.スピンセットのプレビュー

参照パネルでスピンセットを選択し、「 」を選択します。 **[!UICONTROL プレビュー]**. プレビューページで、マウスボタンを押しながらポインターを左右にドラッグして、項目を視覚的に「スピン」します。

詳しくは、 [スピンセットのプレビュー](previewing-spin-set.md#previewing-a-spin-set).

## 6.スピンセットの公開

スピンセットを公開すると、スピンセットがAdobe Dynamic Media Classicサーバーに配置され、Web サイトやアプリケーションに動的に配信できるようになります。 また、Dynamic Media Image Server から Web サイトまたはアプリケーションにスピンセットを呼び出す URL 文字列もアクティベートします。

スピンセットを公開するには、 **[!UICONTROL 公開用にマーク]** アイコンをクリックします。 グローバルナビゲーションバーで、 **[!UICONTROL 公開]** をクリックして公開を開始します。 公開画面で、「 」を選択します。 **[!UICONTROL 公開を送信]**.

詳しくは、 [スピンセットの公開](publishing-spin-set.md#publishing-a-spin-set).

## 7.スピンセットを Web ページにリンクする

Adobe Dynamic Media Classicは、スピンセット用の URL 引き出し線文字列を作成し、公開後にアクティベートします。 これらの URL は、プレビューページからコピーできます。

スピンセットを選択し、「 」を選択します。 **[!UICONTROL プレビュー]**. スピンセットビューアプリセットを選択し、次に、 **[!UICONTROL URL をコピー]**.

詳しくは、 [Web ページへのスピンセットのリンク](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page).
