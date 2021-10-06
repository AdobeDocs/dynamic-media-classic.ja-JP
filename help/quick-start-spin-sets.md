---
title: '"クイックスタート：スピンセット"'
description: Adobe Dynamic Media Classicですばやく作業を始めるのに役立つ概要とスピンセットのクイックスタートです。
uuid: d0af9db6-cb6f-48f0-89f6-f3ab2da0659f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/spin_sets
discoiquuid: 282b8e83-b20f-43f7-b9f8-6eebd5b1c5a7
feature: Dynamic Media Classic,Viewers,Spin Sets
role: User
exl-id: 26e3cd5b-f070-4b92-af36-25631723460e
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 23%

---

# クイックスタート：スピンセット{#quick-start-spin-sets}

スピンセットを使用することで、現実と同じようにオブジェクトを回転させて確認することができます。つまり、アイテムをあらゆる角度から表示して、特徴的な部分を詳細に確認できるようになります。スピンセットは 360 °の表示エクスペリエンスをシミュレートします。 Adobe Dynamic Media Classicには、ビューアが項目を回転できる 1 次元スピンセットと、ビューアが項目を回転および反転できる 2 次元スピンセットが用意されています。 また、ユーザーは、数回のマウスクリックで任意のビューを「自由形式」でズームおよびパンできます。 これらの機能により、特定の方向からアイテムを詳細に確認することができます。

![スピンセット用の画像.](/help/assets/spin_set.png)

スピンセットでは画像マップも使用できます。画像マップとは、スピンセット内の画像上の、テキストを含んだロールオーバーパネルが表示される領域です。ユーザが画像マップをクリックすると、何らかのアクションがトリガされます。例えば、製品の詳細を説明した Web ページが起動します。スピンセット内の画像マップを指すには、ユーザーがマウスポインターを画像マップ上に移動すると、画像マップ自体の周囲にアウトラインが表示されます。

[ 画像マップの作成 ](creating-image-maps.md) を参照してください。

[ 画像とスピンセットを参照してください。Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

このスピンセットクイックスタートは、Adobe Dynamic Media Classicのスピンセットテクニックをすばやく習得できるように作られています。 手順 1 ～ 7 に従ってください。各手順の最後に、トピックのリンクを選択して詳細を確認できます。

## 1.画像を作成してアップロードする

少なくとも、1 次元のスピンセットの場合は 8 ～ 12 ショット、2 次元のスピンセットの場合は 16 ～ 24 ショットが必要です。 アイテムが回転および反転しているように見せるには、一定の角度間隔でアイテムを撮影する必要があります。例えば、1 次元スピンセットに 12 個のショットが含まれている場合は、各ショットごとにアイテムを 30° (360°/12) 回転します。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」を選択して、お使いのコンピューターまたはネットワークからAdobe Dynamic Media Classicにスピン画像をアップロードします。

詳しくは、[スピンセット画像のキャプチャに関するガイドライン](creating-spin-set.md#guidelines-for-shooting-spin-set-images)を参照してください。

## 2.スピンセットの作成

スピンセットを作成するには、グローバルナビゲーションバーで、**[!UICONTROL ビルド]** / **[!UICONTROL スピンセット]** に移動します。 スピンセットのサイズダイアログボックスで、必要な行数とセル数を選択し、「**[!UICONTROL OK]**」を選択します。 次に、画像をスピンセットページのグリッドにドラッグします。

[ スピンセットの作成 ](creating-spin-set.md#creating-a-spin-set) を参照してください。

## 3.スピンセットの編集

スピンセットを編集するには、グローバルナビゲーションバーで、**[!UICONTROL 設定]** / **[!UICONTROL ビューアプリセット]** に移動します。 スピンセットを選択し、「**[!UICONTROL 編集]**」を選択します。 画像の追加、削除、位置の変更を行います。2 次元スピンセットでは、行の位置を変更することもできます。

[ スピンセットの編集 ](creating-spin-set.md#editing-a-spin-set) を参照してください。

## 4.スピンセットビューアプリセットの設定

管理者はスピンセットビューアプリセットを作成できます。これらのプリセットは、スピンセットビューアの外観を決定します。新しいスピンセットビューアプリセットを設定するには、グローバルナビゲーションバーで、**[!UICONTROL 設定]**/**[!UICONTROL ビューアプリセット]** に移動します。

ビューアプリセットページで、「**[!UICONTROL 追加]**」を選択し、ドロップダウンリストから「**[!UICONTROL スピンセットビューア]**」を選択して、「**[!UICONTROL 追加]**」を選択します。 ビューアを設定ページでオプションを選択し、「**[!UICONTROL 保存]**」を選択します。

[ スピンセットビューアプリセットの設定 ](setting-spin-set-viewer-presets.md#setting-up-spin-set-viewer-presets) を参照してください。

## 5.スピンセットのプレビュー

参照パネルでスピンセットを選択し、「**[!UICONTROL プレビュー]**」を選択します。 プレビューページで、マウスボタンを押しながらポインターを左右にドラッグして、項目を視覚的に「スピン」します。

[ スピンセットのプレビュー ](previewing-spin-set.md#previewing-a-spin-set) を参照してください。

## 6.スピンセットの公開

スピンセットを公開すると、スピンセットがAdobe Dynamic Media Classicサーバーに配置され、Web サイトやアプリケーションに動的に配信できるようになります。 また、Dynamic Media Image Server から Web サイトまたはアプリケーションにスピンセットを呼び出す URL 文字列もアクティベートします。

スピンセットを公開するには、参照パネルで名前の横にある **[!UICONTROL 公開用にマーク]** アイコンを選択して、公開用にマークします。 グローバルナビゲーションバーで、「**[!UICONTROL 公開]**」を選択して公開を開始します。 公開画面で、「**[!UICONTROL 公開を送信]**」を選択します。

[ スピンセットの公開 ](publishing-spin-set.md#publishing-a-spin-set) を参照してください。

## 7.スピンセットを Web ページにリンクする

Adobe Dynamic Media Classicは、スピンセットの URL 引き出し線文字列を作成し、公開後にアクティベートします。 これらの URL は、プレビューページからコピーできます。

スピンセットを選択し、「**[!UICONTROL プレビュー]**」を選択します。 スピンセットビューアプリセットを選択し、次に、「**[!UICONTROL URL をコピー]**」を選択します。

[ スピンセットを Web ページにリンクする ](linking-spin-set-web-page.md#linking-a-spin-set-to-a-web-page) を参照してください。
