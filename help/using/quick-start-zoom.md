---
title: クイックスタート：ズーム
description: 概要とクイックスタートを使用してZoomを素早く起動する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
topic: Content Management
level: Beginner
autotag-review: '2026-05-13T20:11:12.792Z'
TQID: 'https://experienceleague.adobe.com/0ilSf9rbFcvh2-AVdVnifjNi7bOa5AjCqBFCUC95I5Q'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 934
ht-degree: 18%

---

# クイックスタート：ズーム{#quick-start-zoom}

ズームでは、画像内の高解像度の詳細をインタラクティブに表示できます。 例えば、画像の色、オプション、角度およびディテールを、動的な詳細設定が可能な統合ビューアで表示できます。 このビューアは、Web ページに埋め込むことも、ポップアップウィンドウに表示することもできます。 近い範囲で画像を監査し、高解像度で画像をパンして、それらを詳細に調べることができます。 ズーム機能を使用すれば、お客様に魅力的で価値のあるインタラクティブな画像を見ていただけます。

Adobe Dynamic Media Classicでは、画像の重要な特徴を強調するためのガイド付きズームも提供されています。 例えば、ロゴのズームターゲットを作成して、ロゴに注目させることができます。 ユーザーがこのズームターゲットを選択すると、ロゴがズームされます。

すべてのズーム画像は、単一のプライマリ画像、グラフィック、データベース駆動属性から作成および提供されます。 Adobe Dynamic Media Classicのズーム機能は、画像の作成と配信にかかる時間とコストを大幅に削減します。 ズームビューアを使用して、画像のズームインとズームアウトを行うことができます。 ズームビューアには、ズームとパンを選択できるボタンがあります。また、画面をドラッグしてパンすることもできます。 ズームビューアプリセットを使用して、画像をズームするためのズームビューアを設定できます。

[Zoom Target: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/559_Zoom%20Target%20Tool_converted%20renamed_Dynamic%20Imaging-AVS)および[Zoom: Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/560_Zoom_converted%20renamed_Dynamic%20Imaging-AVS)のトレーニングビデオを参照してください。

次のZoom クイックスタートは、Adobe Dynamic Media ClassicのZoom テクニックを使用して素早く起動できるように設計されています。 手順 1 ～ 6 に従ってください。 各ステップの後、トピック見出しへの相互参照があり、詳細を確認できます。

## &#x200B;1. ズーム画像をアップロード

まず、ズーム画像をAdobe Dynamic Media Classicにアップロードします。 最適なズームを行うには、Adobe Dynamic Media Classicでは、画像の長さが2000 ピクセル以上であることを推奨しています。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」を選択して、コンピューターまたはネットワークからAdobe Dynamic Media Classicのフォルダーに画像をアップロードします。 [ ズーム画像のアップロード ](uploading-zoom-images.md#uploading_zoom_images)を参照してください。

## &#x200B;2. ガイド付きズーム用のズームターゲットの作成

ズームターゲットにより、画像の特定の部分を強調して表示できます。 例えば、画像の特長的な部分に注目させることができます。 Zoom Viewer ウィンドウでは、ズームターゲットがサムネール画像の形式で画像の横に表示されます。 いずれかのズームターゲットサムネールを選択すると、画像の指定した部分が自動的にズームされます。

ズームターゲットを作成するには、**[!UICONTROL 編集]**&#x200B;を選択してズームターゲットを選択するか、詳細表示の参照パネルで画像を開いて、**[!UICONTROL ズームターゲット]**&#x200B;を選択します。 次に、ズームターゲットエディターページでズームツールを使用して、画像の一部をターゲットとして分離します。 ガイド付きズーム ](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom)のズームターゲットを[作成するを参照してください。

## &#x200B;3. ズームビューアプリセットの設定

ズームビューアプリセットによって、ズームビューアのスタイルと動作が決まります。 管理者の場合は、Zoom ビューアプリセットを設定できます。Adobe Dynamic Media Classicには、デフォルトの「ベストプラクティス」 Zoom ビューアプリセットも用意されています。

ズームビューアプリセットを作成するには、グローバルナビゲーションバーで、**[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**&#x200B;に移動します。 ビューアプリセットページで、**[!UICONTROL 追加]**&#x200B;を選択し、プラットフォームとズームビューアを選択してから、**[!UICONTROL 追加]**&#x200B;を選択します。 次に、`Configure Viewer` ページでオプションを選択します。

Adobe Dynamic Media Classicでは、**[!UICONTROL Zoom Viewer Preset]** オプションを使用して、ビューアのボタンスタイルと全体的な外観を選択できます。 Web サイトのズーム設定をカスタマイズすることもできます。 [ ズームビューアプリセットの設定](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets)を参照してください。

## &#x200B;4. ズームビューアによる画像のプレビュー

ズームビューアで画像をプレビューして、画像をズームしたときのズーム効果を確認することができます。

様々なズームビューアプリセットとそのズームエクスペリエンスの表示方法を確認するには、参照パネルで画像を選択し、**[!UICONTROL プレビュー]**&#x200B;を選択します。 **[!UICONTROL プリセット]** > **[!UICONTROL ズーム]**&#x200B;に移動し、ズームメニューでプリセットを選択します。

ズームボタンが表示されます。 Web サイトでのズーム画像の表示を確認できます。 ズームボタン（およびズームターゲット）を選択して、選択したズームビューアプリセットの設定をテストします。 異なるズームビューアを使用した画像の[ プレビュー](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers)を参照してください。

## &#x200B;5. ズーム画像を公開

ズーム画像を公開すると、Web サイトやアプリケーションに配信できるように、Dynamic Media画像サーバーに配置されます。 公開プロセスの一環として、Adobe Dynamic Media ClassicはURL文字列をアクティベートします。 これらのURL文字列は、Dynamic Media Image ServerからWeb サイトまたはアプリケーションにズーム画像を呼び出します。

グローバルナビゲーションバーで、**[!UICONTROL 公開]**&#x200B;を選択します。 公開ダイアログボックスで、**[!UICONTROL 公開を送信]**&#x200B;を選択します。 詳しくは、[ズーム画像の公開](publishing-zoom-images.md#publishing_zoom_images)を参照してください。

## &#x200B;6. Web ページへのZoom ビューアのリンク

Adobe Dynamic Media Classicは、画像のズームに必要なURL引き出し文字列を作成し、Dynamic Media Image Serverに画像を公開するときにアクティブにします。 これらのURL文字列は、**[!UICONTROL プレビュー]** ページからコピーできます。 URL文字列をコピーすると、Web サイトとアプリケーションで使用できるようになります。 「[Zoom ビューアをWeb ページにリンクする](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages)」を参照してください。
