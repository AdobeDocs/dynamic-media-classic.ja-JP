---
title: '"クイックスタート：画像サイズ変更"'
description: Adobe Dynamic Media Classicの画像サイズ設定テクニックをすばやく習得できるようにするための、概要と画像サイズ変更のクイックスタートです。
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 29%

---

# クイックスタート：画像サイズ変更{#quick-start-image-sizing}

画像のサイズ設定とは、Adobe Dynamic Media Classicが単一の高解像度画像に基づいて複数の派生画像を作成する機能を指します。 Web サイトやアプリケーション用に、サムネールや拡大画像など、複数の画像を手動で作成する代わりに、1 つのマスター画像を提供します。 Adobe Dynamic Media Classicは、ユーザーが要求したとおりに、変更されたすべての画像を生成します。 1 つのマスター画像から動的に画像を配信できることには、次のような利点があります。

* 画像を様々なサイズで手動コピーする必要がありません。1 つのマスター画像をAdobe Dynamic Media Classicに提供すると、Adobe Dynamic Media Classicはマスター画像から異なるサイズの派生画像を生成します。
* Web サイトやアプリケーション全体に含まれている特定の形式の画像のサイズを簡単に変更することができます。例えば、すべてのサムネール画像を変更するには「サムネール」画像プリセットを変更します。画像プリセットは、マクロのようなサイズおよび形式の属性の集まりです。「サムネール」画像プリセットを変更して、Web サイトやアプリケーション全体に含まれているすべてのサムネール画像のサイズを変更することができます。
* 内部または外部のコンテンツ管理システムで、マスターと様々な派生物をすべて管理する必要はありません。

![同じ高解像度マスターファイルから、異なるサイズで複数の派生画像を作成できます。](/help/assets/is_derivative_sizes_popup.png)

[ 画像のサイズ変更を参照してください。Dynamic Imaging](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/557_Image%20Sizing_converted%20renamed_Dynamic%20Imaging-AVS) トレーニングビデオ。

次の画像サイズ設定クイックスタートは、Adobe Dynamic Media Classicの画像サイズ設定テクニックをすばやく習得できるように作られています。 手順 1 ～ 5 に従います。 各手順の最後に、それぞれの内容について詳しく説明している参照先を示しています。

## 1.マスター画像のアップロード

まず、マスター画像をAdobe Dynamic Media Classicにアップロードします。 サイズに関して、Adobe Dynamic Media Classicでは、Web サイトやアプリケーションで予想される最大サイズの画像の使用をお勧めします。 例えば、ビューアで画像をズームする場合は、最大サイズが 2,000 ピクセル以上の画像をアップロードします。 Adobe Dynamic Media Classicでは多くの画像ファイル形式をサポートしますが、可逆圧縮TIFFおよび PNG 画像の使用をお勧めします。

グローバルナビゲーションバーで、「**[!UICONTROL Upload]**」を選択して、コンピューターからAdobe Dynamic Media Classic上のフォルダーにファイルをアップロードします。 [ マスター画像のアップロード ](uploading-master-images.md#uploading_master_images) を参照してください。

## 2.画像プリセットの設定

画像プリセットは、マクロのような定義済みのサイズおよび形式に関するコマンドの集まりであり、特定の名前が付けられて保存されています。画像プリセットは、Dynamic Media Image Server から配信される画像のサイズと形式を管理します。 会社の管理者ステータスを持っているユーザは、独自の画像プリセットを設定できます。Adobe Dynamic Media Classicには、デフォルトの画像プリセットが付属しており、これらを使用して画像を動的に配信できます。

画像プリセットを作成するには（管理者の場合）、グローバルナビゲーションバーで、**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL 画像プリセット]** に移動します。 次に、「**[!UICONTROL 追加]**」を選択して画像プリセットを作成するか、「**[!UICONTROL 編集]**」を選択して既存の画像プリセットを変更します。

作成した画像プリセットが、プレビューページの画像プリセットメニューに追加されます。 新しい画像プリセットを使用して、Web サイトやアプリケーションで動的に画像を表示することができます。[ 画像プリセットの設定 ](setting-image-presets.md#setting_up_image_presets) を参照してください。

## 3.画像プリセットのプレビュー

管理者が設定した様々なプリセットサイズの画像プリセットをプレビューします。

画像プリセットを参照するには、グローバルナビゲーションバーで **[!UICONTROL 設定]** / **[!UICONTROL 画像プリセット]** に移動し、画像プリセットを参照します。

様々な画像プリセットを試してみてください。画像が異なるサイズで Web サイトやアプリケーションに動的に配信された場合の画像の表示方法を確認します。

[ 画像プリセットに基づく画像アセットのプレビュー ](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset) を参照してください。

## 4.マスター画像を公開します

マスター画像ファイルの公開には、主に 2 つの目的があります。

* マスター画像をDynamic Media Image Server に公開して、画像を Web サイトやアプリケーションに動的に配信できるようにします。
* 公開すると、Dynamic Media Image Server から Web サイトまたはアプリケーションに画像を呼び出すための URL 文字列がアクティベートされます。 公開後、必要に応じて、Adobe Dynamic Media Classicで生成した URL をコピーして Web サイトまたはアプリケーションに配置できます。

グローバルナビゲーションバーで、「**[!UICONTROL 公開]**」を選択して、公開ジョブを開始します。 [ パブリッシュ ] ダイアログボックスで、[**[!UICONTROL パブリッシュを送信]**] を選択します。 [ マスター画像の公開 ](publishing-master-images.md#publishing_master_images) を参照してください。

## 5. Web アプリケーションへの URL のリンク

Adobe Dynamic Media Classicは画像の URL 引き出し線文字列を作成します。 画像をDynamic Media Image Server に公開すると、URL がアクティブになります。 これらの URL 文字列は、参照パネル（詳細表示）またはプレビュー画面からコピーできます。 URL 文字列をコピーしたら、それらを Web サイトやアプリケーションで使用することができます。画像サイズ変更用の URL によって、Web ページコード内の静的な画像の名前への参照が置き換えられます。URL はマスター画像名を参照します。この画像名は、表示する新しい画像ごとにデータベースによって置き換えられます。

画像プリセットとともに生成された URL 文字列には、画像プリセットの名前が含まれています。この名前はドル記号 (`$`) で囲まれます。 例えば、`$thumbnail$` を画像プリセットにして、サムネールサイズでマスター画像を表示できます。 [Web アプリケーションへの URL のリンク ](linking-urls-web-application.md#linking_urls_to_your_web_application) を参照してください。
