---
title: 「クイックスタート：画像セット」
description: Adobe Dynamic Media Classicの画像セット手法をすぐに使い始めるのに役立つ画像セットの概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 10%

---

# クイックスタート：画像セット{#quick-start-image-sets}

Adobe Dynamic Media Classic画像セットを使用すると、ユーザーに統一された視聴エクスペリエンスを提供できます。 動的画像セットビューアでは、サムネール画像を選択して項目の様々なビューを表示できます。 画像セットを使用すると、項目の代替の高解像度ビューを表示できます。

画像セットビューアでは、ズームツールを使用して、詳細に画像を確認できます。必要に応じて、ガイド付きズームターゲットと画像マップを画像セットの一部にすることができます。 画像セットによって、統合的で詳細な表示操作が可能になります。

[ 画像およびスピンセット：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) のトレーニングビデオを参照してください。

画像セットを作成する場合、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| 制限タイプ | ベストプラクティス | 適用される制限 |
| --- | --- | --- |
| 1 セットあたりの重複アセット数 | 重複なし | 20‡ |
| 1 セットあたりの最大画像数 | 1 セットあたり 5～10 個の画像 | 1000 |

‡セットに重複したアセットを含めないでください。 1 つのアセットに対する重複の上限は 20 個です。 そのアセットに対して別の重複を（そのセット内で）追加した場合、リクエストでエラーが発生するか、重複が無視されます。

[Dynamic Mediaの制限事項 ](/help/using/limitations.md) も参照してください。

次の画像セットのクイックスタートは、Adobe Dynamic Media Classicの画像セット手法をすぐに使い始められるように設計されています。

## 1.複数のビューおよびスウォッチ用のプライマリ画像をアップロードする

まず、画像セット用の画像をアップロードします。ユーザーは画像セットビューアで画像をズームできるので、画像を選択する際には必ずこの機能を考慮してください。 最大サイズで 2,000 ピクセル以上の画像を使用してください。 Adobe Dynamic Media Classicは多くの画像ファイル形式をサポートしていますが、可逆圧縮TIFF、PNG およびEPSの画像の使用をお勧めします。

グローバルナビゲーションバーの **[!UICONTROL アップロード]** を選択して、コンピューターからAdobe Dynamic Media Classic上のフォルダーにファイルをアップロードします。

[ アップロード用の画像セットアセットの準備 ](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) および [ ファイルのアップロード ](uploading-files.md#uploading-your-files) を参照してください。

## 2.画像セットを作成する

画像セットで、ユーザーは画像セットビューアでサムネール画像を選択して、画像を別の方向または角度から表示できます。

画像セットを作成するには、グローバルナビゲーションバーで「**[!UICONTROL ビルド]**」を選択し、「**[!UICONTROL 画像セット]**」を選択します。 画像セットウィンドウで、画像をページにドラッグして画像セットを作成します。 必要に応じて、画像を整理、追加、および削除します。

[ 画像セットの作成 ](creating-image-set.md#creating-an-image-set) を参照してください。

[ 画像セットにズームターゲットと画像マップを含める ](/help/using/including-zoom-targets-image-maps-image-sets.md) も参照してください。

## 3.必要に応じて画像セットビューアプリセットを準備する

管理者は、画像セットビューアのプリセットを作成または変更できます。Adobe Dynamic Media Classicには、リッチメディアタイプごとにデフォルトのビューアプリセットが用意されています。 画像セットを表示するには、ズームビューアの **[!UICONTROL カスタム]**/**[!UICONTROL 画像]** または **[!UICONTROL 画像セット]**/**[!UICONTROL 複数ビュー]** プリセットを使用します。

アプリケーション設定画面で、ビューアプリセットを追加または編集できます。

[ ビューアプリセットの作成と編集 ](application-setup.md#adding-and-editing-viewer-presets) を参照してください。

## 4.画像セットのプレビュー

参照パネルで画像セットを選択し、「**[!UICONTROL プレビュー]**」を選択します。 プレビューページで、サムネールアイコンを選択し、選択したビューアでの画像セットの表示を確認します。 プリセットメニューから様々なビューアを選択できます。

[ アセットのプレビュー ](previewing-asset.md#previewing-an-asset) を参照してください。

## 5.画像セットのPublish

画像セットを公開すると、Adobe Dynamic Media Classic サーバーに配置され、URL 文字列がアクティベートされます。

>[!NOTE]
>
>画像セットの作成および保存時に、保存後に **[!UICONTROL Publish]** （デフォルト）を選択した場合、この手順は不要です。

参照パネルで、名前の左側にある **[!UICONTROL Publish用にマーク]** アイコンを選択します。 次に、「**[!UICONTROL Publish]**」を選択します。 公開ページで、「**[!UICONTROL Publishを送信]**」を選択します。

[Publish ファイル ](publishing-files.md#publishing-files) を参照してください。

## 6.画像セットの Web サイトへのリンク

Adobe Dynamic Media Classicによって画像セットの URL 呼び出しが作成され、公開後にアクティベートされます。 これらの URL は、プレビュー画面からコピーすることができます。

画像セットを選択し、「**[!UICONTROL プレビュー]**」を選択します。 ここで、画像セットビューアプリセットを選択し、「**[!UICONTROL URL をコピー]**」ボタンをクリックします。

[Web ページへの画像セットのリンク ](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page) を参照してください。
