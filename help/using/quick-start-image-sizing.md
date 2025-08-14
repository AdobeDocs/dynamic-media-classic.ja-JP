---
title: クイックスタート：画像サイズ変更
description: Adobe Dynamic Media Classicの画像サイズ変更手法をすぐに開始する際に役立つ、画像サイズ設定の概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
feature: Dynamic Media Classic,Asset Management
role: User
topic: Content Management
level: Beginner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 7%

---

# クイックスタート：画像サイズ変更{#quick-start-image-sizing}

画像サイズとは、1 枚の高解像度画像に基づいて複数の派生画像を作成する、Adobe Dynamic Media Classicの機能のことです。 Web サイトやアプリケーションに対して、サムネールや拡大表示の画像などの複数の画像を手動で作成するのではなく、単一のプライマリ画像を提供します。 Adobe Dynamic Media Classicは、変更された画像を要求したとおりに、すべて生成します。 単一のプライマリ画像から画像を動的に配信できることには、次のような多くの利点があります。

* 異なるサイズで画像の複数のコピーを手動で作成する必要はありません。 Adobe Dynamic Media Classicに 1 つのプライマリ画像を提供すると、Adobe Dynamic Media Classicがそのプライマリ画像から異なるサイズの派生物を生成します。
* Web サイト全体またはアプリケーション全体で、画像タイプのサイズをすばやく変更できます。 例えば、すべてのサムネイル画像を変更するには、「サムネール」画像プリセットを変更します。 画像プリセットは、マクロに似ており、サイズ属性とフォーマット属性のコレクションです。 「サムネール」画像プリセットを変更すると、web サイトまたはアプリケーション全体のすべてのサムネール画像のサイズを変更できます。
* コンテンツやアセット管理システムのプライマリファイルやあらゆる派生物を内部または外部で管理する必要はありません。

![ 同じ高解像度のプライマリファイルから、異なるサイズで複数の派生画像を作成できます。](/help/using/assets/is_derivative_sizes_popup.png)

[ 画像サイズ：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) のトレーニングビデオを参照してください。

次の画像サイズ設定のクイックスタートは、Adobe Dynamic Media Classicで画像サイズ設定テクニックをすぐに使い始めることを目的としたものです。 手順 1～5 に従います。 各手順に続いて、必要に応じて詳細情報を見つけることができる相互参照があります。

## &#x200B;1. プライマリ画像のアップロード

まず、プライマリ画像をAdobe Dynamic Media Classicにアップロードします。 サイズについては、Adobe Dynamic Media Classicでは、web サイトまたはアプリケーションで使用する予想最大のサイズの画像を使用することをお勧めします。 例えば、ビューアに画像をズームさせる場合は、最大サイズが 2,000 ピクセル以上の画像をアップロードします。 Adobe Dynamic Media Classicは多くの画像ファイル形式をサポートしていますが、可逆圧縮TIFFおよび PNG 画像の使用が推奨されます。

グローバルナビゲーションバーの **[!UICONTROL アップロード]** を選択して、コンピューターからAdobe Dynamic Media Classic上のフォルダーにファイルをアップロードします。 [ プライマリ画像のアップロード ](uploading-master-images.md#uploading_master_images) を参照してください。

## 2.画像プリセットのセットアップ

画像プリセットは、マクロのような定義済みのサイズおよび形式に関するコマンドの集まりであり、特定の名前が付けられて保存されています。画像プリセットは、Dynamic Media Image Server から配信される画像のサイズと形式を制御します。 会社管理者ステータスの場合は、画像プリセットを自分で設定できます。 既にAdobe Dynamic Media Classicに付属しているデフォルトの画像プリセットを使用して、画像を動的に配信できます。

画像プリセットを作成するには（管理者の場合）、グローバルナビゲーションバーで **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 画像プリセット]** に移動します。 次に、「**[!UICONTROL 追加]**」を選択して画像プリセットを作成するか、「**[!UICONTROL 編集]** を選択して既存の画像プリセットを変更します。

作成した画像プリセットは、プレビューページの画像プリセットメニューに追加されます。 新しい画像プリセットを使用すると、Web サイトやアプリケーションに画像を動的に表示できます。 [ 画像プリセットの設定 ](setting-image-presets.md#setting_up_image_presets) を参照してください。

## 3.画像プリセットのプレビュー

管理者が設定した様々なプリセットサイズの画像プリセットをプレビューします。

画像プリセットを参照するには、グローバルナビゲーションバーで **[!UICONTROL 設定]**/**[!UICONTROL 画像プリセット]** に移動し、画像プリセットを参照します。

様々な画像プリセットを試してみてください。Web サイトやアプリケーションに異なるサイズで動的に配信された画像の表示方法を確認します。

[ 画像プリセットに基づいた画像アセットのプレビュー ](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset) を参照してください。

## &#x200B;4. プライマリ画像を公開する

プライマリ画像ファイルを公開すると、次の 2 つの重要な目的を果たします。

* プライマリ画像を Dynamic Media Image Server に公開して、画像を Web サイトやアプリケーションに動的に配信できるようにします。
* 公開すると、Dynamic Media Image Server から web サイトまたはアプリケーションに画像を呼び出すための URL 文字列がアクティブ化されます。 公開後、Adobe Dynamic Media Classicで生成された URL をコピーして、必要に応じて web サイトやアプリケーションに配置できます。

グローバルナビゲーションバーの「**[!UICONTROL 公開]**」を選択して、公開ジョブを開始します。 公開ダイアログボックスで、「**[!UICONTROL 公開を送信]**」を選択します。 [ プライマリ画像の公開 ](publishing-master-images.md#publishing_master_images) を参照してください。

## &#x200B;5. Web アプリケーションに URL をリンクする

Adobe Dynamic Media Classicは、画像の URL コールアウト文字列を作成します。 画像を Dynamic Media Image Server に公開すると、URL がアクティブになります。 これらの URL 文字列は、参照パネル（詳細ビュー）またはプレビュー画面からコピーできます。 URL 文字列をコピーすると、Web サイトやアプリケーションで使用できます。 画像サイズ設定の URL は、web ページのコード内の静的な画像名への参照に代わるものです。 URL は、表示する新しい画像ごとにデータベースで置き換えられるプライマリ画像名を参照します。

画像プリセットとともに生成された URL 文字列には、画像プリセットの名前が含まれています。この名前は、ドル記号（`$`）で囲まれています。 例え `$thumbnail$`、サムネールサイズでプライマリ画像を表示するように設計された画像プリセットを使用できます。 [Web アプリケーションに URL をリンクする ](linking-urls-web-application.md#linking_urls_to_your_web_application) を参照してください。
