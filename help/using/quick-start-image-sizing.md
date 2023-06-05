---
title: "クイックスタート：画像サイズ変更"
description: Adobe Dynamic Media Classicの画像サイズ設定テクニックをすばやく習得して実行するのに役立つ、概要と画像サイズ変更のクイックスタートです。
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 38d7f8d6e5888e1c5ba9260ada45b79fb16b338f
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 22%

---

# クイックスタート：画像サイズ変更{#quick-start-image-sizing}

画像のサイズ設定とは、Adobe Dynamic Media Classicが単一の高解像度画像に基づいて複数の派生画像を作成する機能を指します。 Web サイトやアプリケーション用に、サムネールや拡大表示画像など、複数の画像を手動で作成する代わりに、1 つのプライマリ画像を提供します。 Adobe Dynamic Media Classicは、要求されたとおりに、変更されたすべての画像を生成します。 単一のプライマリイメージから動的にイメージを配信できることには、次のような多くの利点があります。

* 画像を様々なサイズで手動コピーする必要がありません。1 つのプライマリ画像をAdobe Dynamic Media Classicに指定すると、Adobe Dynamic Media Classicはプライマリ画像から異なるサイズの派生画像を生成します。
* Web サイトやアプリケーション全体に含まれている特定の形式の画像のサイズを簡単に変更することができます。例えば、すべてのサムネール画像を変更するには「サムネール」画像プリセットを変更します。画像プリセットは、マクロのようなサイズおよび形式の属性の集まりです。「サムネール」画像プリセットを変更して、Web サイトやアプリケーション全体に含まれているすべてのサムネール画像のサイズを変更することができます。
* 内部または外部のコンテンツ管理システムで、プライマリファイルと様々な派生ファイルを管理する必要はありません。

![同じ高解像度のプライマリファイルから、異なるサイズの複数の派生画像を作成できます。](/help/using/assets/is_derivative_sizes_popup.png)

詳しくは、 [画像サイズ：Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

次の画像サイズ設定クイックスタートは、Adobe Dynamic Media Classicの画像サイズ設定テクニックをすばやく習得および実行できるように設計されています。 手順 1 ～ 5 に従います。 各手順の後には、相互参照があり、必要に応じて詳細を確認できます。

## 1.プライマリ画像をアップロード

まず、プライマリ画像をAdobe Dynamic Media Classicにアップロードします。 Adobe Dynamic Media Classicでは、サイズに関して、Web サイトやアプリケーションで予想される最大サイズの画像を使用することをお勧めします。 例えば、ビューアで画像をズームする場合は、最大サイズが 2,000 ピクセル以上の画像をアップロードします。 Adobe Dynamic Media Classicでは多くの画像ファイル形式がサポートされますが、可逆TIFFおよび PNG 画像の使用が推奨されます。

グローバルナビゲーションバーで、 **[!UICONTROL アップロード]** お使いのコンピューターからAdobe Dynamic Media Classic上のフォルダーにファイルをアップロードする場合。 詳しくは、 [プライマリ画像のアップロード](uploading-master-images.md#uploading_master_images).

## 2.画像プリセットを設定する

画像プリセットは、マクロのような定義済みのサイズおよび形式に関するコマンドの集まりであり、特定の名前が付けられて保存されています。画像プリセットは、Dynamic Media Image Server から配信される画像のサイズと形式を管理します。 会社の管理者ステータスを持っているユーザは、独自の画像プリセットを設定できます。Adobe Dynamic Media Classicには、デフォルトの画像プリセットが付属しており、それらを使用して画像を動的に配信できます。

画像プリセットを作成するには（管理者の場合は）、グローバルナビゲーションバーでに移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 画像プリセット]**. 次に、 **[!UICONTROL 追加]** 画像プリセットを作成する場合は、「 **[!UICONTROL 編集]** をクリックして、既存の画像プリセットを変更します。

作成した画像プリセットは、プレビューページの画像プリセットメニューに追加されます。 新しい画像プリセットを使用して、Web サイトやアプリケーションで動的に画像を表示することができます。詳しくは、 [画像プリセットの設定](setting-image-presets.md#setting_up_image_presets).

## 3.画像プリセットをプレビュー

管理者が設定した様々なプリセットサイズの画像プリセットをプレビューします。

画像プリセットを参照するには、グローバルナビゲーションバーのに移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 画像プリセット]**&#x200B;をクリックし、画像プリセットを参照します。

様々な画像プリセットを試してみてください。画像が様々なサイズで Web サイトやアプリケーションに動的に配信された場合の画像の表示を確認します。

詳しくは、 [画像プリセットに基づいた画像アセットのプレビュー](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset).

## 4.プライマリ画像を公開する

プライマリ画像ファイルの公開は、次の 2 つの基本的な目的を果たします。

* Dynamic Media Image Server にプライマリ画像を公開して、Web サイトやアプリケーションに動的に画像を配信できるようにします。
* 公開すると、Dynamic Media Image Server から Web サイトまたはアプリケーションに画像を呼び出すための URL 文字列がアクティベートされます。 公開後、Adobe Dynamic Media Classicで生成した URL を必要に応じてコピーし、Web サイトやアプリケーションに配置できます。

グローバルナビゲーションバーで、 **[!UICONTROL 公開]** 公開ジョブを開始します。 [ パブリッシュ ] ダイアログボックスで、 **[!UICONTROL 公開を送信]**. 詳しくは、 [プライマリ画像を公開](publishing-master-images.md#publishing_master_images).

## 5. Web アプリケーションに URL をリンクする

Adobe Dynamic Media Classicは画像の URL 引き出し線文字列を作成します。 画像をDynamic Media Image Server に公開すると、URL がアクティブになります。 これらの URL 文字列は、参照パネル（詳細ビュー）またはプレビュー画面からコピーできます。 URL 文字列をコピーしたら、それらを Web サイトやアプリケーションで使用することができます。画像サイズ変更用の URL によって、Web ページコード内の静的な画像の名前への参照が置き換えられます。この URL はプライマリ画像名を参照します。この名前は、表示する新しい画像ごとにデータベースに置き換えられます。

画像プリセットとともに生成された URL 文字列には、画像プリセットの名前が含まれています。この名前はドル記号 (`$`) をクリックします。 例： `$thumbnail$` には、サムネールサイズでプライマリ画像を表示するように設計された画像プリセットを指定できます。 詳しくは、 [Web アプリケーションへの URL のリンク](linking-urls-web-application.md#linking_urls_to_your_web_application).
