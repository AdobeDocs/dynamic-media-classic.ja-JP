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
source-git-commit: de6997fda88c4471625242ee9cca59b344cee945
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 13%

---

# クイックスタート：画像セット{#quick-start-image-sets}

Adobe Dynamic Media Classic画像セットを使用すると、ユーザーに統一された視聴エクスペリエンスを提供できます。 動的画像セットビューアでは、サムネール画像を選択して項目の様々なビューを表示できます。 画像セットを使用すると、項目の代替の高解像度ビューを表示できます。

画像セットビューアでは、ズームツールを使用して、詳細に画像を確認できます。また必要に応じて、画像セットのガイドズーム用のズームターゲットや画像マップを作成できます。画像セットによって、統合的で詳細な表示操作が可能になります。

参照： [画像およびスピンセット：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

画像セットを作成する場合、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| 制限タイプ | ベストプラクティス | 適用される制限 |
| --- | --- | --- |
| 1 セットあたりの重複アセット数 | 重複なし | 20‡ |
| 1 セットあたりの最大画像数 | 1 セットあたり 5～10 個の画像 | 1000 |

‡セットに重複したアセットを含めないでください。 1 つのアセットに対する重複の上限は 20 個です。 そのアセットに対して別の重複を（そのセット内で）追加した場合、リクエストでエラーが発生するか、重複が無視されます。

関連トピック [Dynamic Mediaの制限](/help/using/limitations.md).

次の画像セットのクイックスタートは、Adobe Dynamic Media Classicの画像セット手法をすぐに使い始められるように設計されています。

## 1.複数のビューおよびスウォッチ用のプライマリ画像をアップロードする

まず、画像セット用の画像をアップロードします。ユーザーは画像セットビューアで画像をズームできるので、画像を選択する際には必ずこの機能を考慮してください。 最大サイズで 2,000 ピクセル以上の画像を使用してください。 Adobe Dynamic Media Classicは多くの画像ファイル形式をサポートしていますが、可逆圧縮TIFF、PNG およびEPSの画像の使用をお勧めします。

グローバルナビゲーションバーで、を選択します。 **[!UICONTROL Upload]** （コンピューターからAdobe Dynamic Media Classicのフォルダーにファイルをアップロードする場合）

参照： [アップロード用の画像セットアセットの準備](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) および [ファイルをアップロード](uploading-files.md#uploading-your-files).

## 2.画像セットを作成する

画像セットで、ユーザーは画像セットビューアでサムネール画像を選択して、画像を別の方向または角度から表示できます。

画像セットを作成するには、グローバルナビゲーションバーで以下を選択します。 **[!UICONTROL ビルド]**&#x200B;を選択してから、 **[!UICONTROL 画像セット]**. 画像セットウィンドウで、画像をページにドラッグして画像セットを作成します。 必要に応じて、画像を整理、追加、および削除します。

参照： [画像セットを作成](creating-image-set.md#creating-an-image-set).

関連トピック [画像セットにズームターゲットと画像マップを含める](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3.必要に応じて画像セットビューアプリセットを準備する

管理者は、画像セットビューアのプリセットを作成または変更できます。Adobe Dynamic Media Classicには、リッチメディアタイプごとにデフォルトのビューアプリセットが用意されています。 ズームビューアの使用： **[!UICONTROL カスタム]** > **[!UICONTROL 画像]** または **[!UICONTROL 画像セット]**/**[!UICONTROL 複数ビュー]** 画像セットを表示するプリセット。

アプリケーション設定画面で、ビューアプリセットを追加または編集できます。

参照： [ビューアプリセットの作成と編集](application-setup.md#adding-and-editing-viewer-presets).

## 4.画像セットのプレビュー

参照パネルで画像セットを選択し、を選択します。 **[!UICONTROL プレビュー]**. プレビューページで、サムネールアイコンを選択し、選択したビューアでの画像セットの表示を確認します。 プリセットメニューから様々なビューアを選択できます。

参照： [アセットのプレビュー](previewing-asset.md#previewing-an-asset).

## 5.画像セットを公開する

画像セットを公開すると、Adobe Dynamic Media Classic サーバーに配置され、URL 文字列がアクティベートされます。

>[!NOTE]
>
>を選択した場合、この手順は不要です **[!UICONTROL 保存後に公開]** （デフォルト）画像セットを作成して保存した時点。

を選択 **[!UICONTROL 公開用にマーク]** 参照パネル内の名前の左側にあるアイコン。 次に、を選択します **[!UICONTROL 公開]**. 公開ページで、を選択します。 **[!UICONTROL 公開を送信]**.

参照： [ファイルを公開](publishing-files.md#publishing-files).

## 6.画像セットの Web サイトへのリンク

Adobe Dynamic Media Classicによって画像セットの URL 呼び出しが作成され、公開後にアクティベートされます。 これらの URL は、プレビュー画面からコピーすることができます。

画像セットを選択してから、を選択します **[!UICONTROL プレビュー]**. ここで、画像セットビューアプリセットを選択し、 **[!UICONTROL URL をコピー]** ボタン。

参照： [画像セットの Web ページへのリンク](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
