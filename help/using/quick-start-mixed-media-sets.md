---
title: 「クイックスタート：混在メディアセット」
description: Adobe Dynamic Media Classicをすぐに使い始めるのに役立つ混在メディアセットの概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/mixed_media_sets
feature: Dynamic Media Classic,Viewers,Mixed Media Sets
role: User
exl-id: 757893ae-7507-42a0-a67b-f6542e7231c7
topic: Content Management
level: Beginner
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 16%

---

# クイックスタート：混在メディアセット{#quick-start-mixed-media-sets}

混在メディアセットは、ユーザーに対して統一された視聴エクスペリエンスを提供します。 混在メディアセットには、画像、画像セット、スウォッチセット、スピンセットおよびビデオを含めることができます。ユーザーは混在メディアビューア内の様々なタブを選択して、様々なビューアの項目を表示できます。 タブを指定しなかった場合、すべてのアセットがスウォッチ行に表示されます。

混在メディアセットビューアプリセットには、エンドユーザーがコードを埋め込んだり、URL をコピーしたり、メイン Web サイトにリンクしたりするためのコミュニティオプションが含まれています。 ユーザーは、これらのオプションを使用して、製品に関する情報を個人の Web サイトやソーシャルネットワーキングサイトで共有できます。

この混在メディアセットのクイックスタートは、Adobe Dynamic Media Classicの混在メディアセット手法をすぐに使い始めることを目的としています。

## 1.画像、見本ファイルおよびビデオをアップロードする

まず、混在メディアセット用の画像、スウォッチファイルおよびビデオをアップロードします。ユーザーは混在メディアセットビューアで画像をズームできるので、画像を選択する際には必ずこの機能を考慮してください。 最大サイズで 2,000 ピクセル以上の画像を使用してください。

グローバルナビゲーションバーで、を選択します。 **[!UICONTROL Upload]** （コンピューターからAdobe Dynamic Media Classicのフォルダーにファイルをアップロードする場合）

参照： [ファイルをアップロード](uploading-files.md#uploading-your-files).

## 2.混在メディアセット内で使用するメディアセットを作成する

画像、画像セット、見本セット、スピンセットおよびビデオを混在メディアセットに追加できます。 混在メディアセットに追加する前に、メディアセットを準備します。

参照： [画像セットを作成](creating-image-set.md#creating-an-image-set), [スウォッチセットの作成](creating-swatch-set.md#creating-a-swatch-set)、および [スピンセットの作成](creating-spin-set.md#creating-a-spin-set).

## 3.混在メディアセットの作成

グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL 混在メディアセット]**. 画像、見本セット、画像セットおよびビデオを混在メディアセットページにドラッグします。 サウンドトラックを追加するには、「サウンドトラック」ボックスにオーディオファイルをドラッグします。

参照： [混在メディアセットの作成](creating-mixed-media-set.md#creating-a-mixed-media-set).

## 4.混在メディアビューアプリセットの設定

Adobe Dynamic Media Classicには、混在メディアセット用のデフォルトのビューアプリセットが付属しています。 管理者は、混在メディアセットビューアプリセットを作成または変更できます。

混在メディアセットビューアプリセットを設定する場合、セット内の他のすべてのアセットのビューアプリセットを追加します。 例えば、混在メディアセットにビデオが含まれている場合、混在メディアセットビューアプリセットにビデオビューアプリセットを追加します。 ビューアにサウンドトラックを追加することもできます。サウンドトラックはビューアが開いていると再生されますが、ビデオがアクティブなときには再生されません。

参照： [混在メディアセットビューアプリセットの設定](setting-mixed-media-set-viewer.md#setting-up-a-mixed-media-set-viewer-preset) および [ビューアプリセットの作成と編集](application-setup.md#adding-and-editing-viewer-presets).

関連トピック [ビューアプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

## 5.混在メディアセットのプレビュー

混在メディアセットの選択 **[!UICONTROL プレビュー]** ボタン。 混在メディアセットビューアで混在メディアセットを確認するには、サムネールアイコンとスウォッチアイコンを選択します。 プリセットメニューから様々なビューアを選択できます。

参照： [アセットのプレビュー](previewing-asset.md#previewing-an-asset).

## 6.混在メディアセットの公開

混在メディアセットを公開すると、そのセットはAdobe Dynamic Media Classic サーバーに配置され、URL 文字列がアクティベートされます。

混在メディアセットは、**ビデオサーバー**&#x200B;にも **Image Server** にも公開する必要があります。使用方法 **ビデオ サーバー** 公開用にマークした実際のビデオを公開します。 また、を使用します **Image Server** 関連アセット（ビデオサムネールなど）を公開し、アダプティブビデオセットの情報を設定します。

参照： [混在メディアセットの公開](publishing-mixed-media-set.md#publishing-a-mixed-media-set).

## 7. Web ページへの混在メディアセットのリンク

混在メディアセットの URL 呼び出しは、Adobe Dynamic Media Classicによって公開後にアクティベートされます。 これらの URL は、プレビューページからコピーできます。

混在メディアセットを選択し、 **[!UICONTROL プレビュー]**. プレビューページで、混在メディアセットビューアプリセットを選択し、次に **[!UICONTROL URL をコピー]**. 参照： [混在メディアセットの Web ページへのリンク](linking-mixed-media-set-web.md#linking-a-mixed-media-set-to-a-web-page).
