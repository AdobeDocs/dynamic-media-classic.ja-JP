---
title: クイックスタート：ズーム
description: すぐに使い始めるのに役立つズームの概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
topic: Content Management
level: Beginner
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 19%

---

# クイックスタート：ズーム{#quick-start-zoom}

ズームを使用すると、画像の高解像度の詳細をインタラクティブに表示できます。 例えば、画像の色、オプション、角度およびディテールを、動的な詳細設定が可能な統合ビューアで表示できます。このビューアは、web ページに埋め込んだり、ポップアップウィンドウに表示したりできます。 近距離の画像を監査したり、高解像度の画像をパンして詳細に調べたりできます。 ズーム機能を使用すれば、お客様に魅力的で価値のあるインタラクティブな画像を見ていただけます。

Adobe Dynamic Media Classicには、ガイド付きズームも用意されています。ガイド付きズームは、画像の重要な機能を強調表示するための手段です。 例えば、ロゴのズームターゲットを作成して、ロゴに注目させることができます。ユーザーがこのズームターゲットを選択すると、ロゴにズームします。

すべてのズーム画像は、単一のプライマリ画像、グラフィックおよびデータベース駆動属性から作成および提供されます。 Adobe Dynamic Media Classicのズーム機能により、画像の作成と配信に要する時間とコストが大幅に削減されます。 ズームビューアを使用して、画像のズームインおよびズームアウトを行うことができます。 ズームビューアには、ズームおよびパン用に選択できるボタンがあります。画面をドラッグしてパンすることもできます。 ズームビューアプリセットを使用して、画像をズームするためのズームビューアを設定できます。

[Zoom Target:Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/559_Zoom%20Target%20Tool_converted%20renamed_Dynamic%20Imaging-AVS) および [Zoom:Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/560_Zoom_converted%20renamed_Dynamic%20Imaging-AVS) のトレーニングビデオを参照してください。

次のズームクイックスタートは、Adobe Dynamic Media Classicでのズームテクニックをすぐに使い始められるように設計されています。 手順 1 ～ 6 に従ってください。各手順に続いて、詳細な情報を見つけることができるトピックの見出しへの相互参照があります。

## &#x200B;1. ズーム画像のアップロード

まず、ズーム画像をAdobe Dynamic Media Classicにアップロードします。 最適なズームを行うために、Adobe Dynamic Media Classicでは、画像を最長サイズで 2,000 ピクセル以上にすることをお勧めしています。

グローバルナビゲーションバーの **[!UICONTROL アップロード]** を選択して、コンピューターまたはネットワークからAdobe Dynamic Media Classicのフォルダーに画像をアップロードします。 [&#x200B; ズーム画像のアップロード &#x200B;](uploading-zoom-images.md#uploading_zoom_images) を参照してください。

## &#x200B;2. ガイド付きズームのズームターゲットの作成

ズームターゲットにより、画像の特定の部分を強調して表示できます。例えば、画像の特長的な部分に注目させることができます。Zoom Viewer ウィンドウで、ズーム ターゲットがサムネール画像の形で画像の横に表示されます。 いずれかのズームターゲットサムネールを選択すると、画像の指定した部分が自動的にズームされます。

ズームターゲットを作成するには、「**[!UICONTROL 編集]**」を選択して「ズームターゲット」を選択するか、詳細ビューの参照パネルで画像を開いて「**[!UICONTROL ズームターゲット]**」を選択します。 次に、ズームターゲットエディターページのズームツールを使用して、画像の一部をターゲットとして分離します。 [&#x200B; ガイドズームのズームターゲットの作成 &#x200B;](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom) を参照してください。

## &#x200B;3. ズームビューアプリセットの設定

ズームビューアプリセットによって、ズームビューアのスタイルと動作が決まります。管理者は、ズームビューアプリセットを設定できます。Adobe Dynamic Media Classicには、デフォルトの「ベストプラクティス」ズームビューアプリセットも付属しています。

ズームビューアプリセットを作成するには、グローバルナビゲーションバーで **[!UICONTROL 設定]**/**[!UICONTROL ビューアプリセット]** に移動します。 ビューアプリセットページで「**[!UICONTROL 追加]**」を選択し、プラットフォーム、ズームビューアを選択して、「**[!UICONTROL 追加]**」を選択します。 次に、`Configure Viewer` ページでオプションを選択します。

Adobe Dynamic Media Classicでは、ボタンのスタイルとビューア全体の外観を選択できる **[!UICONTROL ズームビューアプリセット]** オプションが用意されています。 Web サイトのズーム設定をカスタマイズすることもできます。 [&#x200B; ズームビューアプリセットの設定 &#x200B;](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets) を参照してください。

## &#x200B;4. ズームビューアでの画像のプレビュー

ズームビューアで画像をプレビューして、画像をズームしたときのズーム効果を確認することができます。

様々なズームビューアプリセットを探索し、ズームエクスペリエンスがどのように表示されるかを確認するには、参照パネルで画像を選択して **[!UICONTROL プレビュー]** を選択します。 **[!UICONTROL プリセット]** / **[!UICONTROL ズーム]** に移動し、ズーム メニューでプリセットを選択します。

ズームボタンが表示されます。Web サイトでズーム画像がどのように表示されるかを確認できます。 「ズーム」ボタン（および「ズームターゲット」）を選択して、選択したズームビューアプリセットの設定をテストできます。 [&#x200B; 様々なズームビューアで画像をプレビュー &#x200B;](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers) を参照してください。

## &#x200B;5. ズーム画像の公開

ズーム画像を公開すると、Web サイトやアプリケーションに配信できるように、Dynamic Media 画像サーバーに配置されます。 公開プロセスの一環として、Adobe Dynamic Media Classicは URL 文字列をアクティブ化します。 これらの URL 文字列は、Dynamic Media Image Server から Web サイトまたはアプリケーションにズーム画像を呼び出します。

グローバルナビゲーションバーの「**[!UICONTROL 公開]**」を選択します。 公開ダイアログボックスで、「**[!UICONTROL 公開を送信]**」を選択します。 詳しくは、[ズーム画像の公開](publishing-zoom-images.md#publishing_zoom_images)を参照してください。

## &#x200B;6. ズームビューアを web ページにリンクする

Adobe Dynamic Media Classicは、画像のズームに必要な URL コールアウト文字列を作成し、Dynamic Media Image Server に画像を公開するときにそれらをアクティブにします。 これらの URL 文字列は、「**[!UICONTROL プレビュー]**」ページからコピーできます。 URL 文字列をコピーすると、Web サイトやアプリケーションで使用できるようになります。 [Web ページへのズームビューアのリンク &#x200B;](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages) を参照してください。
