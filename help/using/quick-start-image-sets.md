---
title: クイックスタート：画像セット
description: Adobe Dynamic Media Classicの画像セットのテクニックを使用して、すばやく起動して実行するのに役立つ概要と画像セットのクイックスタート。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sets
feature: Dynamic Media Classic,Viewers,Image Sets
role: User
exl-id: 280e7201-84d6-46b1-94bb-0499beca2992
topic: Content Management
level: Beginner
autotag-review: '2026-05-13T20:09:40.553Z'
TQID: 'https://experienceleague.adobe.com/s3cXJgoACODCKQ8oMlykXjLAVmx6yWw9F2EC-3EbR0k'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 719
ht-degree: 11%

---

# クイックスタート：画像セット{#quick-start-image-sets}

Adobe Dynamic Media Classicの画像セットを使用すると、視聴体験を統合できます。 動的画像セットビューアでは、サムネール画像を選択して、項目の様々なビューを表示できます。 画像セットを使用すると、アイテムの高解像度の代替ビューを表示できます。

画像セットビューアでは、ズームツールを使用して、詳細に画像を確認できます。 必要に応じて、画像セットの一部にガイド付きズームターゲットと画像マップを作成できます。 画像セットによって、統合的で詳細な表示操作が可能になります。

[画像とスピンセット：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/556_Image%20&%20Spin%20Sets_converted%20renamed_Dynamic%20Imaging-AVS)のトレーニングビデオを参照してください。

画像セットを作成する場合、Adobeでは次のベストプラクティスを推奨し、次の制限を適用します。

| 制限タイプ | ベストプラクティス | 制限が適用されました |
| --- | --- | --- |
| セットあたりの重複アセットの数 | 重複なし | 20‡ |
| 1 セットあたりの最大画像数 | 5～10枚/セット | 1000 |

‡ベストプラクティスは、セット内に重複するアセットを含めないことです。 1つのアセットに対する重複の数は20件までです。 そのセット内で、そのアセットに別の重複を追加すると、リクエストはエラーを与えるか、重複を無視します。

[Dynamic Mediaの制限](/help/using/limitations.md)も参照してください。

次の画像セットクイックスタートは、Adobe Dynamic Media Classicの画像セットのテクニックを使用して迅速に起動できるように設計されています。

## &#x200B;1. 複数のビューとスウォッチ用にプライマリ画像をアップロード

まず、画像セット用の画像をアップロードします。 ユーザーは画像セットビューアで画像をズームできるので、画像を選択する際は、この機能を考慮してください。 画像が最大サイズの2000 ピクセル以上であることを確認します。 Adobe Dynamic Media Classicでは、多くの画像ファイル形式をサポートしていますが、TIFF、PNG、EPSの各画像は可逆です。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」を選択して、コンピューターからAdobe Dynamic Media Classicのフォルダーにファイルをアップロードします。

[画像セットアセットのアップロード準備](preparing-image-set-assets-upload.md#preparing-image-set-assets-for-upload)および[&#x200B; ファイルのアップロード &#x200B;](uploading-files.md#uploading-your-files)を参照してください。

## &#x200B;2. 画像セットの作成

画像セットでは、ユーザーは画像セットビューアでサムネイル画像を選択して、異なる側または角度から画像を表示します。

画像セットを作成するには、グローバルナビゲーションバーで「**[!UICONTROL ビルド]**」を選択し、「**[!UICONTROL 画像セット]**」を選択します。 画像セットウィンドウで、画像をページにドラッグして画像セットを作成します。 必要に応じて、画像を整理、追加、および削除します。

[画像セットの作成](creating-image-set.md#creating-an-image-set)を参照してください。

[画像セットにズームターゲットと画像マップを含める](/help/using/including-zoom-targets-image-maps-image-sets.md)も参照してください

## &#x200B;3. 必要に応じて、画像セットビューアプリセットを準備します

管理者は、画像セットビューアのプリセットを作成または変更できます。 Adobe Dynamic Media Classicには、各リッチメディアタイプのデフォルトのビューアプリセットが用意されています。 ズームビューアを使用します。**[!UICONTROL カスタム]** > **[!UICONTROL 画像]**&#x200B;または&#x200B;**[!UICONTROL 画像セット]**/**[!UICONTROL 複数ビュー]** プリセットを使用して、画像セットを表示します。

アプリケーションの設定画面からビューアプリセットを追加または編集できます。

[&#x200B; ビューアプリセットの作成と編集](application-setup.md#adding-and-editing-viewer-presets)を参照してください。

## &#x200B;4. 画像セットのプレビュー

参照パネルで画像セットを選択し、**[!UICONTROL プレビュー]**&#x200B;を選択します。 プレビューページで、サムネールアイコンを選択し、選択したビューアで画像セットを確認します。 プリセットメニューから様々なビューアを選択できます。

[&#x200B; アセットのプレビュー](previewing-asset.md#previewing-an-asset)を参照してください。

## &#x200B;5. 画像セットの公開

画像セットを公開すると、Adobe Dynamic Media Classic サーバーに配置され、URL文字列がアクティブ化されます。

>[!NOTE]
>
>この手順は、画像セットの作成時および保存時に保存&#x200B;**（デフォルト）の後に**&#x200B;公開を選択した場合は不要です。

参照パネルで、名前の左側にある「**[!UICONTROL 公開用にマーク]**」アイコンを選択します。 次に、**[!UICONTROL 公開]**&#x200B;を選択します。 公開ページで、**[!UICONTROL 公開を送信]**&#x200B;を選択します。

[&#x200B; ファイルの公開](publishing-files.md#publishing-files)を参照してください。

## &#x200B;6. 画像セットをWeb サイトにリンクする

Adobe Dynamic Media Classicは、画像セットのURL呼び出しを作成し、公開後にそれらをアクティブ化します。 これらの URL は、プレビュー画面からコピーすることができます。

画像セットを選択し、**[!UICONTROL プレビュー]**&#x200B;を選択します。 次に、画像セットビューアプリセットを選択し、「**[!UICONTROL URLをコピー]**」ボタンをクリックします。

「[画像セットをWeb ページにリンクする](linking-image-set-web-page.md#linking-an-image-set-to-a-web-page)」を参照してください。
