---
title: '"クイックスタート：ズーム"'
description: 概要とクイックスタートのズームを参照してください。
uuid: 31eda632-3469-4f90-885b-e90c6a2e5e75
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
discoiquuid: 559c986d-313d-46df-a5ff-0b49316ad3a7
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: eae35207-000c-4ced-b9ab-714c2384a9e7
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '944'
ht-degree: 28%

---

# クイックスタート：ズーム{#quick-start-zoom}

ズームを使用すると、画像の高解像度の詳細をインタラクティブに表示できます。 例えば、画像の色、オプション、角度およびディテールを、動的な詳細設定が可能な統合ビューアで表示できます。このビューアは、Web ページに埋め込んだり、ポップアップウィンドウに表示したりすることができます。近い範囲で画像を監査し、高解像度で画像をパンして、画像を詳細に調べることができます。 ズーム機能を使用すれば、お客様に魅力的で価値のあるインタラクティブな画像を見ていただけます。

Adobe Dynamic Media Classicには、画像内の重要な機能を強調表示するガイド付きズーム機能もあります。 例えば、ロゴのズームターゲットを作成して、ロゴに注目させることができます。このズームターゲットを選択すると、ロゴがズームされます。

すべてのズーム画像は、1 つのマスター画像、グラフィック、データベース連動型の属性から作成され、供給されます。Adobe Dynamic Media Classicのズームにより、画像の生成と配信にかかる時間とコストが大幅に削減されます。 ズームビューアを使用して、画像をズームインまたはズームアウトできます。 ズームビューアには、ズームとパンを選択できるボタンがあります。画面上でドラッグしてパンすることもできます。 ズームビューアプリセットを使用して、画像をズームするためのズームビューアを設定できます。

[ ズームターゲットを参照してください。Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/559_Zoom%20Target%20Tool_converted%20renamed_Dynamic%20Imaging-AVS) と [ ズーム：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/560_Zoom_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

次のズームクイックスタートは、Adobe Dynamic Media Classicのズームテクニックをすばやく習得できるように設計されています。 手順 1 ～ 6 に従ってください。各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

## 1.ズーム画像のアップロード

まず、ズーム画像をAdobe Dynamic Media Classicにアップロードします。 最適なズームを実現するために、Adobe Dynamic Media Classicでは、画像の最長サイズを 2,000 ピクセル以上にすることをお勧めします。

グローバルナビゲーションバーで、「**[!UICONTROL Upload]**」を選択して、お使いのコンピューターまたはネットワークからAdobe Dynamic Media Classic上のフォルダーに画像をアップロードします。 [ ズーム画像のアップロード ](uploading-zoom-images.md#uploading_zoom_images) を参照してください。

## 2.ガイド付きズーム用のズームターゲットを作成する

ズームターゲットにより、画像の特定の部分を強調して表示できます。例えば、画像の特長的な部分に注目させることができます。ズームターゲットは、ズームビューアウィンドウ内で画像の隣にサムネール画像の形式で表示されます。いずれかのズームターゲットサムネールを選択すると、画像の指定した部分が自動的にズームされます。

ズームターゲットを作成するには、**[!UICONTROL 「]** 編集」を選択して「ズームターゲット」を選択するか、詳細ビューの参照パネルで画像を開いて「**[!UICONTROL ズームターゲット]**」を選択します。 次に、ズームターゲットエディタページのズームツールを使用して、画像の一部をターゲットとして選択表示できます。 [ ガイド付きズームのズームターゲットの作成 ](creating-zoom-targets-guided-zoom.md#creating_zoom_targets_for_guided_zoom) を参照してください。

## 3.ズームビューアプリセットの設定

ズームビューアプリセットによって、ズームビューアのスタイルと動作が決まります。ズームビューアプリセットは、管理者が設定できます。Adobe Dynamic Media Classicには、初期設定の「ベストプラクティス」ズームビューアプリセットも用意されています。

ズームビューアプリセットを作成するには、グローバルナビゲーションバーで **[!UICONTROL 設定]** / **[!UICONTROL ビューアプリセット]** に移動します。 ビューアプリセットページで、「**[!UICONTROL 追加]**」を選択し、プラットフォームを選択して、ズームビューアを選択し、「**[!UICONTROL 追加]**」を選択します。 次に、ビューアを設定ページでオプションを選択します。

Adobe Dynamic Media Classicには、ボタンのスタイルとビューアの全体的な外観を選択できる **[!UICONTROL ズームビューアプリセット]** オプションが用意されています。 また、各自の Web サイト用にズーム設定をカスタマイズすることもできます。[ ズームビューアプリセットの設定 ](setting-zoom-viewer-presets.md#setting_up_zoom_viewer_presets) を参照してください。

## 4.ズームビューアで画像をプレビューする

ズームビューアで画像をプレビューして、画像をズームしたときのズーム効果を確認することができます。

様々なズームビューアプリセットとそのズーム効果を確認するには、参照パネルで画像を選択し、「**[!UICONTROL プレビュー]**」を選択します。 **[!UICONTROL プリセット]** / **[!UICONTROL ズーム]** に移動し、ズームメニューでプリセットを選択します。

ズームボタンが表示されます。Web サイト上でズーム画像がどのように表示されるかを確認することができます。「ズーム」ボタン（およびズームターゲット）を選択して、選択したズームビューアプリセットの設定をテストできます。 [ 様々なズームビューアでの画像のプレビュー ](previewing-image-assets-different-zoom.md#previewing_image_assets_with_different_zoom_viewers) を参照してください。

## 5.ズーム画像の公開

ズーム画像を公開すると、それらがDynamic Media Image Server に配置され、Web サイトやアプリケーションに配信できるようになります。 公開プロセスの一環として、Adobe Dynamic Media Classicは URL 文字列をアクティベートします。 これらの URL 文字列は、Dynamic Media Image Server から Web サイトまたはアプリケーションにズーム画像を呼び出します。

グローバルナビゲーションバーで、「**[!UICONTROL 発行]**」を選択します。 [ パブリッシュ ] ダイアログボックスで、[**[!UICONTROL パブリッシュを送信]**] を選択します。 詳しくは、[ズーム画像の公開](publishing-zoom-images.md#publishing_zoom_images)を参照してください。

## 6. Web ページへのズームビューアのリンク

Adobe Dynamic Media Classicは、画像のズームに必要な URL 引き出し線文字列を作成し、画像をDynamic Media Image Server に公開する際にアクティベートします。 これらの URL 文字列は、**[!UICONTROL プレビュー]** ページからコピーできます。 URL 文字列をコピーしたら、それらを Web サイトやアプリケーションで使用することができます。[Web ページへのズームビューアのリンク ](linking-zoom-viewers-web-pages.md#linking_zoom_viewers_to_your_web_pages) を参照してください。
