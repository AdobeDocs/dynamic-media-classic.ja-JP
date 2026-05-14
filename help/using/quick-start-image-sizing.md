---
title: クイックスタート：画像サイズ変更
description: Adobe Dynamic Media Classicの画像サイズ変更テクニックを使用して素早く起動するための概要とクイックスタート画像サイズ変更について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
autotag-review: '2026-05-13T20:09:57.533Z'
TQID: 'https://experienceleague.adobe.com/VGp4OQ03iRiobXKWuUERNtFwUMQ4z7a19wyOgHWuv3w'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 926
ht-degree: 7%

---

# クイックスタート：画像サイズ変更{#quick-start-image-sizing}

画像のサイズ変更とは、Adobe Dynamic Media Classicが1つの高解像度画像に基づいて複数の派生画像を作成する機能を指します。 Web サイトやアプリケーション用に複数の画像（サムネールや拡大表示の画像など）を手動で作成するのではなく、1つのプライマリ画像を提供します。 Adobe Dynamic Media Classicは、リクエストと同様に、すべての変更された画像を生成します。 単一のプライマリ画像から画像を動的に配信できることには、多くの利点があります。

* 異なるサイズの画像の複数のコピーを手動で作成する必要はありません。 1つのプライマリ画像をAdobe Dynamic Media Classicに指定すると、Adobe Dynamic Media Classicはプライマリ画像から異なるサイズのアウトプットを生成します。
* Web サイトまたはアプリケーション全体で、画像タイプのサイズをすばやく変更できます。 例えば、すべてのサムネール画像を変更するには、「サムネール」画像プリセットを変更します。 画像プリセットは、マクロと似ています。サイズとフォーマット属性のコレクションです。 「サムネール」画像プリセットを変更して、Web サイトまたはアプリケーション全体のすべてのサムネール画像のサイズを変更できます。
* コンテンツ管理システムやアセット管理システム内のプライマリファイルや様々な派生ファイルを社内外で管理する必要はありません。

![同じ高解像度のプライマリファイルから異なるサイズの複数の派生画像を作成できます。](/help/using/assets/is_derivative_sizes_popup.png)

[画像サイズ：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS)のトレーニングビデオを参照してください。

次の画像サイズ変更クイックスタートは、Adobe Dynamic Media Classicの画像サイズ変更テクニックを使用して迅速に起動できるように設計されています。 手順1～5に従います。 各ステップの後には、必要に応じて詳細情報を見つけることができる相互参照があります。

## &#x200B;1. プライマリ画像のアップロード

まず、プライマリ画像をAdobe Dynamic Media Classicにアップロードします。 サイズに関しては、Adobe Dynamic Media Classicでは、Web サイトまたはアプリケーションで想定される最大サイズの画像を使用することをお勧めします。 例えば、ビューアに画像をズームさせたい場合は、最大サイズで2000 ピクセル以上の画像をアップロードします。 Adobe Dynamic Media Classicでは、多くの画像ファイル形式をサポートしていますが、TIFFやPNG画像は可逆です。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」を選択して、コンピューターからAdobe Dynamic Media Classicのフォルダーにファイルをアップロードします。 [ プライマリ画像のアップロード ](uploading-master-images.md#uploading_master_images)を参照してください。

## &#x200B;2. 画像プリセットの設定

画像プリセットは、マクロのような定義済みのサイズおよび形式に関するコマンドの集まりであり、特定の名前が付けられて保存されています。 画像プリセットは、Dynamic Media Image Serverから配信される画像のサイズと形式を制御します。 会社管理者ステータスがある場合は、独自に画像プリセットを設定できます。 Adobe Dynamic Media Classicに既に付属しているデフォルトの画像プリセットを使用して、画像を動的に配信できます。

画像プリセットを作成するには（管理者の場合）、グローバルナビゲーションバーで、**[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 画像プリセット]**&#x200B;に移動します。 次に、**[!UICONTROL 追加]**&#x200B;を選択して画像プリセットを作成するか、**[!UICONTROL 編集]**&#x200B;を選択して既存の画像プリセットを変更します。

作成した画像プリセットは、プレビューページの画像プリセットメニューに追加されます。 新しい画像プリセットを使用して、Web サイトやアプリケーションで画像を動的に表示できます。 [画像プリセットの設定](setting-image-presets.md#setting_up_image_presets)を参照してください。

## &#x200B;3. 画像プリセットのプレビュー

管理者が設定した様々なプリセットサイズの画像プリセットをプレビューします。

画像プリセットを検索するには、グローバルナビゲーションバーで、**[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**&#x200B;に移動し、画像プリセットを参照します。

様々な画像プリセットを試してみてください。 Web サイトやアプリケーションに異なるサイズで動的に配信される画像の表示方法を確認します。

[画像プリセットに基づく画像アセットのプレビュー](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)を参照してください。

## &#x200B;4. プライマリ画像の公開

プライマリ画像ファイルの公開には、次の2つの重要な目的があります。

* 画像をWeb サイトとアプリケーションに動的に配信できるように、プライマリ画像をDynamic Media Image Serverに公開します。
* 公開すると、Dynamic Media Image ServerからWeb サイトまたはアプリケーションに画像を呼び出すためのURL文字列がアクティブ化されます。 公開後、Adobe Dynamic Media Classicで生成したURLをコピーして、Web サイトまたはアプリケーションに必要に応じて配置できます。

グローバルナビゲーションバーで、**[!UICONTROL 公開]**&#x200B;を選択して公開ジョブを開始します。 公開ダイアログボックスで、**[!UICONTROL 公開を送信]**&#x200B;を選択します。 [ プライマリ画像の公開](publishing-master-images.md#publishing_master_images)を参照してください。

## &#x200B;5. Web アプリケーションへのURLのリンク

Adobe Dynamic Media Classicは、画像のURL コールアウト文字列を作成します。 Dynamic Media画像サーバーに画像を公開すると、URLがアクティブになります。 これらのURL文字列は、参照パネル（詳細ビュー）またはプレビュー画面からコピーできます。 URL文字列をコピーしたら、Web サイトとアプリケーションで使用できます。 画像サイズ変更のURLは、Web ページコード内の静的な画像名への参照に置き換わります。 URLは、表示する新しい画像ごとにデータベースが置き換えるプライマリ画像名を参照します。

画像プリセットとともに生成された URL 文字列には、画像プリセットの名前が含まれています。 この名前はドル記号（`$`）で囲まれています。 例えば、`$thumbnail$`は、サムネールサイズでプライマリ画像を表示するように設計された画像プリセットです。 「[Web アプリケーションへのURLのリンク ](linking-urls-web-application.md#linking_urls_to_your_web_application)」を参照してください。
