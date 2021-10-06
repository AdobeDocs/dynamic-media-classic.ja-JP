---
title: '"クイックスタート：画像セット"'
description: Adobe Dynamic Media Classicの画像セットのテクニックをすばやく習得して実行するのに役立つ、画像セットの概要とクイックスタートを説明します。
uuid: daf17d13-9c06-41f0-8fc5-2e56d460d341
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
discoiquuid: 612a425f-2840-46c4-8e5a-c0bc5f738f4e
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 22%

---

# クイックスタート：画像セット{#quick-start-image-sets}

Adobe Dynamic Media Classic画像セットは、統合された表示エクスペリエンスを提供します。 動的な画像セットビューアでは、ユーザがサムネール画像をクリックすると、項目の様々なビューが表示されます。画像セットを使用すると、項目の高解像度の別のビューを表示できます。

画像セットビューアでは、ズームツールを使用して、詳細に画像を確認できます。また必要に応じて、画像セットのガイドズーム用のズームターゲットや画像マップを作成できます。画像セットによって、統合的で詳細な表示操作が可能になります。

[ 画像とスピンセットを参照してください。Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/556_Image%20&amp;%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

次の画像セットのクイックスタートは、Adobe Dynamic Media Classicの画像セットのテクニックをすばやく習得できるように設計されています。

## 1.複数のビューおよびスウォッチ用のマスター画像をアップロードします

まず、画像セット用の画像をアップロードします。ユーザーは画像セットビューアで画像をズームできるので、画像を選択する際はこの機能を考慮してください。 最大サイズで 2,000 ピクセル以上の画像を使用してください。 Adobe Dynamic Media Classicは多くの画像ファイル形式をサポートしますが、可逆TIFF、PNG、EPSの画像の使用をお勧めします。

グローバルナビゲーションバーで、「**[!UICONTROL Upload]**」を選択して、コンピューターからAdobe Dynamic Media Classic上のフォルダーにファイルをアップロードします。

[ アップロード用の画像セットアセットの準備 ](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload) および [ ファイルのアップロード ](uploading-files.md#uploading-your-files) を参照してください。

## 2.画像セットの作成

画像セットでは、ユーザーは画像セットビューアでサムネール画像を選択して、異なる辺や角度の画像を表示します。

画像セットを作成するには、グローバルナビゲーションバーで **[!UICONTROL ビルド]** を選択し、**[!UICONTROL 画像セット]** を選択します。 画像セットウィンドウで、画像をページにドラッグして画像セットを作成します。 必要に応じて、画像を整理、追加、および削除します。

[ 画像セットの作成 ](creating-image-set.md#creating-an-image-set) を参照してください。

[ 画像セットにズームターゲットと画像マップを含める ](/help/including-zoom-targets-image-maps-image-sets.md) も参照してください。

## 3.必要に応じて画像セットビューアプリセットを準備します

管理者は、画像セットビューアのプリセットを作成または変更できます。Adobe Dynamic Media Classicには、各リッチメディアタイプに対応するデフォルトのビューアプリセットが用意されています。 ズームビューアを使用します。**[!UICONTROL カスタム]** > **[!UICONTROL 画像]** または **[!UICONTROL 画像セット]**/**[!UICONTROL 複数のビュー]** プリセットを使用して画像セットを表示します。

ビューアプリセットは、アプリケーション設定画面で追加または編集できます。

[ ビューアプリセットの作成と編集 ](application-setup.md#adding-and-editing-viewer-presets) を参照してください。

## 4.画像セットのプレビュー

参照パネルで画像セットを選択し、「**[!UICONTROL プレビュー]**」を選択します。 プレビューページで、サムネールアイコンを選択して、選択したビューアでの画像セットの表示を確認します。 プリセットメニューから様々なビューアを選択できます。

[ アセットのプレビュー ](previewing-asset.md#previewing-an-asset) を参照してください。

## 5.画像セットの公開

画像セットを公開すると、Adobe Dynamic Media Classicサーバーに配置され、URL 文字列がアクティベートされます。

>[!NOTE]
>
>画像セットを作成して保存した際に「**[!UICONTROL 保存後に公開]**」を選択した場合は（初期設定）、この手順は不要です。

参照パネルで、名前の左側にある **[!UICONTROL 公開用にマーク]** アイコンを選択します。 次に、「**[!UICONTROL 公開]**」を選択します。 発行ページで、「**[!UICONTROL 発行を送信]**」を選択します。

[ ファイルの公開 ](publishing-files.md#publishing-files) を参照してください。

## 6. Web サイトへの画像セットのリンク

Adobe Dynamic Media Classicは画像セットの URL 呼び出しを作成し、公開後にアクティベートします。 これらの URL は、プレビュー画面からコピーすることができます。

画像セットを選択し、**[!UICONTROL プレビュー]** を選択します。 次に、画像セットビューアプリセットを選択し、「**[!UICONTROL URL をコピー]**」を選択します。

[ 画像セットを Web ページにリンクする ](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page) を参照してください。
