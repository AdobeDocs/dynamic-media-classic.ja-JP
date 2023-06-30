---
title: "クイックスタート：画像セット"
description: Adobe Dynamic Media Classicの画像セットのテクニックをすばやく習得して実行するのに役立つ、画像セットの概要とクイックスタートです。
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 21%

---

# クイックスタート：画像セット{#quick-start-image-sets}

Adobe Dynamic Media Classicの画像セットは、統合された表示エクスペリエンスを提供します。 動的な画像セットビューアでは、ユーザがサムネール画像をクリックすると、項目の様々なビューが表示されます。画像セットを使用すると、項目の別の高解像度ビューを表示できます。

画像セットビューアでは、ズームツールを使用して、詳細に画像を確認できます。また必要に応じて、画像セットのガイドズーム用のズームターゲットや画像マップを作成できます。画像セットによって、統合的で詳細な表示操作が可能になります。

詳しくは、 [画像およびスピンセット：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

画像セットを作成する際、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| 制限タイプ | ベストプラクティス | 制限が適用されました |
| --- | --- | --- |
| セットあたりの重複アセット数 | 重複なし | 20 |
| 1 セットあたりの最大画像数 | 1 セットあたり 5～10 個の画像 | 1000 |

関連トピック [Dynamic Mediaの制限](/help/using/limitations.md).

次に示す画像セットのクイックスタートは、Adobe Dynamic Media Classicの画像セットのテクニックをすぐに使い始めることを目的としています。

## 1.複数のビューおよびスウォッチ用のプライマリ画像をアップロードします。

まず、画像セット用の画像をアップロードします。ユーザーは画像セットビューアで画像をズームできるので、画像を選択する際は、この機能を考慮してください。 最大サイズで 2,000 ピクセル以上の画像を使用してください。 Adobe Dynamic Media Classicでは多くの画像ファイル形式がサポートされますが、可逆TIFF、PNG、EPS画像の使用が推奨されます。

グローバルナビゲーションバーで、 **[!UICONTROL アップロード]** お使いのコンピューターからAdobe Dynamic Media Classic上のフォルダーにファイルをアップロードする場合。

詳しくは、 [アップロード用の画像セットアセットの準備](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) および [ファイルをアップロード](uploading-files.md#uploading-your-files).

## 2.画像セットの作成

画像セットでは、ユーザーは画像セットビューアでサムネール画像を選択して、異なる側面や角度から画像を表示します。

画像セットを作成するには、グローバルナビゲーションバーで **[!UICONTROL ビルド]**&#x200B;を選択して、 **[!UICONTROL 画像セット]**. 画像セットウィンドウで、画像をページにドラッグして画像セットを作成します。 必要に応じて、画像を整理、追加、および削除します。

詳しくは、 [画像セットの作成](creating-image-set.md#creating-an-image-set).

関連トピック [画像セットにズームターゲットと画像マップを含める](/help/using/including-zoom-targets-image-maps-image-sets.md)

## 3.必要に応じて画像セットビューアプリセットを準備する

管理者は、画像セットビューアのプリセットを作成または変更できます。Adobe Dynamic Media Classicには、各リッチメディアタイプ用のデフォルトのビューアプリセットが用意されています。 ズームビューアを使用します。 **[!UICONTROL カスタム]** > **[!UICONTROL 画像]** または **[!UICONTROL 画像セット]**/**[!UICONTROL 複数ビュー]** プリセットを使用して画像セットを表示できます。

ビューアプリセットは、アプリケーション設定画面で追加または編集できます。

詳しくは、 [ビューアプリセットの作成と編集](application-setup.md#adding-and-editing-viewer-presets).

## 4.画像セットのプレビュー

参照パネルで画像セットを選択し、「 」を選択します。 **[!UICONTROL プレビュー]**. プレビューページで、サムネールアイコンを選択して、選択したビューアでの画像セットの表示を確認します。 プリセットメニューから様々なビューアを選択できます。

詳しくは、 [アセットのプレビュー](previewing-asset.md#previewing-an-asset).

## 5.画像セットの公開

画像セットを公開すると、その画像セットがAdobe Dynamic Media Classicサーバーに配置され、URL 文字列がアクティベートされます。

>[!NOTE]
>
>画像セットを作成して保存した際に「**[!UICONTROL 保存後に公開]**」を選択した場合は（初期設定）、この手順は不要です。

選択 **[!UICONTROL 公開用にマーク]** アイコンをクリックします。 次に、 **[!UICONTROL 公開]**. 公開ページで、「 」を選択します。 **[!UICONTROL 公開を送信]**.

詳しくは、 [ファイルを公開](publishing-files.md#publishing-files).

## 6. Web サイトに画像セットをリンクする

Adobe Dynamic Media Classicは画像セットの URL 呼び出しを作成し、公開後にアクティベートします。 これらの URL は、プレビュー画面からコピーすることができます。

画像セットを選択し、「 」を選択します。 **[!UICONTROL プレビュー]**. 次に、画像セットビューアプリセットを選択し、「 」を選択します。 **[!UICONTROL URL をコピー]**.

詳しくは、 [Web ページへの画像セットのリンク](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page).
