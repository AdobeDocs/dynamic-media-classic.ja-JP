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
source-git-commit: 202f477d78272c66d0ac490e3a5041839b3e4f4d
workflow-type: tm+mt
source-wordcount: 870
ht-degree: 6%

---

# クイックスタート：画像サイズ変更{#quick-start-image-sizing}

画像のサイズ変更とは、Adobe Dynamic Media Classicが1つの高解像度画像に基づいて複数の派生画像を作成する機能を指します。 web サイトやアプリケーション用に複数の画像を手動で作成するのではなく、1つのプライマリ画像を提供します。 Adobe Dynamic Media Classicでは、リクエスト時に変更されたすべての画像が生成されます。 単一のプライマリ画像から画像を動的に配信するメリットは数多くあります。

* 異なるサイズの画像の複数のコピーを手動で作成する必要はありません。 1つのプライマリ画像をAdobe Dynamic Media Classicに供給すると、プライマリ画像から異なるサイズのアウトプットが生成されます。
* web サイトやアプリケーション全体で、画像のサイズをすばやく変更できます。 例えば、すべてのサムネール画像を変更するには、「サムネール」画像プリセットを変更します。 画像プリセットは、サイズとフォーマット属性のコレクションです。 Web サイトまたはアプリケーション全体のすべてのサムネール画像のサイズを変更するには、「サムネール」画像プリセットを変更します。
* コンテンツ管理システムやアセット管理システムで、プライマリファイルや様々な派生ファイルをすべて管理する必要はありません。

![同じ高解像度のプライマリファイル ](/help/using/assets/is_derivative_sizes_popup.png)から異なるサイズの複数の派生画像を作成できます。

[画像サイズ：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS)のトレーニングビデオを参照してください。

次の画像サイズ変更クイックスタートは、Adobe Dynamic Media Classicで画像サイズ変更テクニックを使用する際に役立つように設計されています。 手順1～5を完了します。 各ステップの後には、必要に応じて詳細情報を見つけることができる相互参照があります。

## &#x200B;1. プライマリ画像のアップロード

メイン画像をAdobe Dynamic Media Classicにアップロードします。 Adobe Dynamic Media Classicでは、web サイトまたはアプリケーションで使用できる最大サイズの画像を使用することをお勧めします。 例えば、ビューアに画像をズームさせたい場合は、最大サイズで2000 ピクセル以上の画像をアップロードします。 Adobe Dynamic Media Classicでは、多くの画像ファイル形式をサポートしていますが、TIFFやPNG画像は可逆です。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」を選択して、コンピューターからAdobe Dynamic Media Classicのフォルダーにファイルをアップロードします。 [ プライマリ画像のアップロード ](uploading-master-images.md#uploading_master_images)を参照してください。

## &#x200B;2. 画像プリセットの設定

画像プリセットは、名前の下に保存された、定義済みのサイズと書式コマンドのコレクションです。 画像プリセットは、Dynamic Media Image Serverから配信される画像のサイズと形式を制御します。 会社管理者ステータスがある場合は、画像プリセットを個別に設定できます。 Adobe Dynamic Media Classicに含まれているデフォルトの画像プリセットを使用して、画像を動的に配信できます。

画像プリセットを作成するには（管理者の場合）、グローバルナビゲーションバーで、**[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 画像プリセット]**&#x200B;に移動します。 次に、**[!UICONTROL 追加]**&#x200B;を選択して画像プリセットを作成するか、**[!UICONTROL 編集]**&#x200B;を選択して既存の画像プリセットを変更します。

作成した画像プリセットは、プレビューページの画像プリセットメニューに追加されます。 新しい画像プリセットを使用して、Web サイトやアプリケーションで動的に画像を表示することができます。 [画像プリセットの設定](setting-image-presets.md#setting_up_image_presets)を参照してください。

## &#x200B;3. 画像プリセットのプレビュー

管理者が設定した様々なプリセットサイズの画像プリセットをプレビューします。

画像プリセットを検索するには、グローバルナビゲーションバーで、**[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**&#x200B;に移動し、画像プリセットを参照します。

様々な画像プリセットをテストします。 web サイトやアプリケーションに異なるサイズで動的に配信する際に、画像がどのように表示されるかを決定します。

[画像プリセットに基づく画像アセットのプレビュー](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)を参照してください。

## &#x200B;4. プライマリ画像の公開

プライマリ画像ファイルの公開には、次の2つの重要な目的があります。

* プライマリ画像をDynamic Media画像サーバーに公開して、画像をweb サイトやアプリケーションに動的に配信できるようにします。
* 公開すると、Dynamic Media Image Serverからweb サイトまたはアプリケーションに画像を呼び出すためのURL文字列がアクティブ化されます。 公開後、Adobe Dynamic Media Classicで生成したURLをコピーして、web サイトまたはアプリケーションで必要に応じて配置できます。

グローバルナビゲーションバーで、**[!UICONTROL 公開]**&#x200B;を選択して公開ジョブを開始します。 公開ダイアログボックスで、**[!UICONTROL 公開を送信]**&#x200B;を選択します。 [ プライマリ画像の公開](publishing-master-images.md#publishing_master_images)を参照してください。

## &#x200B;5. Web アプリケーションへのURLのリンク

Adobe Dynamic Media Classicは、画像のURL コールアウト文字列を作成します。 Dynamic Media画像サーバーに画像を公開すると、URLがアクティブになります。 これらのURL文字列は、参照パネル（詳細ビュー）またはプレビュー画面からコピーできます。 URL文字列をコピーしたら、web サイトまたはアプリケーションで使用できます。 画像サイズ変更のURLは、web ページコード内の静的画像名への参照に置き換わります。 URLは、表示される新しい画像ごとにデータベースが置き換えるプライマリ画像名を参照します。

画像プリセットとともに生成された URL 文字列には、画像プリセットの名前が含まれています。 この名前はドル記号（`$`）で囲まれています。 例えば、`$thumbnail$`は、サムネールサイズでプライマリ画像を表示するように設計された画像プリセットです。 「[Web アプリケーションへのURLのリンク ](linking-urls-web-application.md#linking_urls_to_your_web_application)」を参照してください。
