---
title: '"クイックスタート：画像サイズ変更"'
description: 画像サイズ設定のテクニックをすばやく習得できるようにするための、概要と画像のサイズ変更のクイックスタートです。
uuid: 6c4ad4b7-549d-4daa-b6b9-5997a8427af8
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/image_sizing
discoiquuid: dcaa9b21-b925-4dbb-865e-7918cdbda50c
feature: Dynamic Media Classic，アセット管理
role: Business Practitioner
exl-id: f1d46f03-57a1-43d8-a0ee-74b92b590736
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 37%

---

# クイックスタート：画像サイズ変更{#quick-start-image-sizing}

画像のサイズ設定とは、Dynamic Media Classicで、単一の高解像度画像に基づいて複数の派生画像を作成する機能を指します。 Webサイトやアプリケーション用に、サムネールや拡大表示画像など、複数の画像を手動で作成する代わりに、1つのマスター画像を提供します。 Dynamic Media Classicは、要求されたとおりに、変更されたすべての画像を生成します。 1 つのマスター画像から動的に画像を配信できることには、次のような利点があります。

* 画像を様々なサイズで手動コピーする必要がありません。1つのマスター画像をDynamic Media Classicに提供すると、Dynamic Media Classicはマスター画像から異なるサイズの派生画像を生成します。
* Web サイトやアプリケーション全体に含まれている特定の形式の画像のサイズを簡単に変更することができます。例えば、すべてのサムネール画像を変更するには「サムネール」画像プリセットを変更します。画像プリセットは、マクロのようなサイズおよび形式の属性の集まりです。「サムネール」画像プリセットを変更して、Web サイトやアプリケーション全体に含まれているすべてのサムネール画像のサイズを変更することができます。
* 内部または外部のコンテンツ管理システムのマスターおよび様々な派生物をすべて管理する必要はありません。

![同じ高解像度マスターファイルから、異なるサイズの複数の派生画像を作成できます。](/help/assets/is_derivative_sizes_popup.png)

この画像サイズ設定クイックスタートは、Dynamic Media Classicの画像サイズ設定テクニックをすばやく習得できるように設計されています。 手順1 ～ 5に従います。 各手順の最後に、それぞれの内容について詳しく説明している参照先を示しています。

## 1.マスター画像のアップロード

まず、マスター画像をDynamic Media Classicにアップロードします。 サイズに関しては、Dynamic Media Classicでは、Webサイトやアプリケーションで使用が予想される最大サイズの画像の使用をお勧めします。 例えば、ビューアで画像をズームする場合は、最大サイズが2,000ピクセル以上の画像をアップロードします。 Dynamic Media Classicは多くの画像ファイル形式をサポートしますが、可逆圧縮TIFFおよびPNG画像の使用をお勧めします。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」をクリックして、コンピューターからDynamic Media Classicのフォルダーにファイルをアップロードします。 詳しくは、[マスター画像のアップロード](uploading-master-images.md#uploading_master_images)を参照してください。

## 2.画像プリセットの設定

画像プリセットは、マクロのような定義済みのサイズおよび形式に関するコマンドの集まりであり、特定の名前が付けられて保存されています。画像プリセットは、Dynamic Media Image Serverから画像を配信する際に使用するサイズと形式を管理します。 会社の管理者ステータスを持っているユーザは、独自の画像プリセットを設定できます。Dynamic Media Classicには、デフォルトの画像プリセットが付属しており、これらを使用して画像を動的に配信することもできます。

画像プリセットを作成する（管理者の場合）には、グローバルナビゲーションバーで&#x200B;**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL 画像プリセット]**&#x200B;をクリックします。 次に、「**[!UICONTROL 追加]**」をクリックして画像プリセットを作成するか、「**[!UICONTROL 編集]**」をクリックして既存の画像プリセットを変更します。

作成した画像プリセットが、プレビューページの画像プリセットメニューに追加されます。 新しい画像プリセットを使用して、Web サイトやアプリケーションで動的に画像を表示することができます。詳しくは、[画像プリセットの設定](setting-image-presets.md#setting_up_image_presets)を参照してください。

## 3.画像プリセットのプレビュー

管理者が設定した様々なプリセットサイズの画像プリセットをプレビューします。

画像プリセットを表示するには、グローバルナビゲーションバーで&#x200B;**[!UICONTROL 設定]** / **[!UICONTROL 画像プリセット]**&#x200B;をクリックし、画像プリセットを参照します。

様々な画像プリセットを試してみてください。画像が異なるサイズでWebサイトやアプリケーションに動的に配信された場合の画像の表示方法を確認します。

詳しくは、[画像プリセットに基づいた画像アセットのプレビュー](previewing-asset.md#previewing_an_image_asset_based_on_its_image_preset)を参照してください。

## 4.マスター画像の公開

マスター画像ファイルの公開には、主に 2 つの目的があります。

* マスター画像をDynamic Media Image Serverに公開して、画像をWebサイトやアプリケーションに動的に配信できるようにします。
* 公開すると、Dynamic Media Image ServerからWebサイトやアプリケーションに画像を呼び出すためのURL文字列がアクティブ化されます。 公開後、必要に応じて、Dynamic Media Classicで生成したURLをコピーして、Webサイトやアプリケーションに配置できます。

グローバルナビゲーションバーで、「**[!UICONTROL 公開]**」をクリックして、公開ジョブを開始します。 パブリッシュダイアログボックスで、「**[!UICONTROL パブリッシュを送信]**」をクリックします。 詳しくは、[マスター画像の公開](publishing-master-images.md#publishing_master_images)を参照してください。

## 5. WebアプリケーションへのURLのリンク

Dynamic Media Classicは、画像のURL引き出し線文字列を作成します。 画像をDynamic Media Image Serverに公開すると、URLがアクティブになります。 これらの URL 文字列は、参照パネル（詳細ビュー）またはプレビュー画面からコピーすることができます。URL 文字列をコピーしたら、それらを Web サイトやアプリケーションで使用することができます。画像サイズ変更用の URL によって、Web ページコード内の静的な画像の名前への参照が置き換えられます。URL はマスター画像名を参照します。この画像名は、表示する新しい画像ごとにデータベースによって置き換えられます。

画像プリセットとともに生成された URL 文字列には、画像プリセットの名前が含まれています。この名前はドル記号(`$`)で囲まれます。 例えば、`$thumbnail$`を画像プリセットにして、サムネールサイズでマスター画像を表示できます。 詳しくは、[Web アプリケーションへの URL のリンク](linking-urls-web-application.md#linking_urls_to_your_web_application)を参照してください。
