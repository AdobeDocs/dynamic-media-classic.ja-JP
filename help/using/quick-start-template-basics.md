---
title: クイックスタート：基本テンプレート
description: Adobe Dynamic Media Classicを迅速に使い始めるための概要とクイックスタートのテンプレートの基本について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:10:57.394Z'
TQID: 'https://experienceleague.adobe.com/2DaWdJsCz9f5iXEkMi6N1L7s3eFdvpBc1ECrgbVAueo'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 853
ht-degree: 18%

---

# クイックスタート：基本テンプレート{#quick-start-template-basics}

テンプレートの基本は、Adobe Photoshopなどの画像編集アプリケーションで、レイヤーファイルなどのレイヤー化された画像ファイルを動的に作成し、アドレス可能なレイヤー化された画像ファイルとして扱うことができます。 PSD ファイルなどの、レイヤーが含まれている静的ファイルとは異なり、テンプレートにはパラメータを含めることができます。 パラメータを使用して、画像の様々な要素をアドレス指定したりカスタマイズすることができます。

テンプレートには、複数の画像レイヤーとテキストレイヤーを含めることができます。 レイヤー化されたPSD ファイルなどのレイヤーを含む静的ファイルをテンプレートに変換し、Adobe Dynamic Media Classicでテンプレートを作成できます。 Adobe Dynamic Media Classicにアップロードしたフォントを使用して、テンプレートにテキストレイヤーを作成できます。 テンプレートにテキストを追加したら、その位置、フォント、フォントサイズ、カラーを変更して書式を設定できます。

パラメーターページを使用すると、テンプレートのあらゆる側面をアドレス可能なパラメーターに変換できます。 これにより、使用するレイヤー画像やテンプレートで使用するテキスト値を変更できます。 パラメーターはURL文字列で渡され、任意のパラメーターを変更して、Image Serverから生成された返信画像を動的にカスタマイズできます。

[ テンプレートの基本](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS)のトレーニングビデオも参照してください。

このクイックスタートは、テンプレートの基本を素早く習得できるように設計されています。

## &#x200B;1. ファイルのアップロード

最初に、テンプレート用の PSD ファイルまたは画像ファイルをアップロードします。 Adobe Dynamic Media Classicは、PSDに加えて多くの画像ファイル形式をサポートしていますが、ロスレス TIFFとPNG画像は透明性を保つため、テンプレートに使用することをお勧めします。

PSD ファイルを使用してテンプレートを作成する場合は、PSD ファイルをアップロードするときに&#x200B;**[!UICONTROL Upload Job Options]** ダイアログボックスで「**[!UICONTROL テンプレートを作成]**」を選択します。 また、**[!UICONTROL レイヤーの命名]** オプションを選択して、Adobe Dynamic Media ClassicがPSD レイヤーをAdobe Dynamic Media Classicにアップロードするときに名前を付ける方法を認識できるようにします。

画像ファイルを使用している場合は、画像を切り抜くことができ、画像をアップロードするときに画像内のクリッピングパスからマスクを作成することもできます。

グローバルナビゲーションバーで、「**[!UICONTROL アップロード]**」を選択して、PSD ファイルまたはその他の画像ファイルをコンピューターからAdobe Dynamic Media Classicのフォルダーにアップロードします。 [ テンプレートファイルのアップロード ](uploading-template-files.md#uploading_template_files)を参照してください。

## &#x200B;2. テンプレートの作成

PSD ファイルからテンプレートを作成するには、ファイルをアップロードするときに「**[!UICONTROL テンプレートを作成]**」を選択します。 画像からテンプレートを作成するには、グローバルナビゲーションバーで、**[!UICONTROL ビルド]** > **[!UICONTROL テンプレートの基本]**&#x200B;に移動し、キャンバスの幅と高さの測定値を入力します。 ページの右上隅付近で、**[!UICONTROL Designer]**&#x200B;または&#x200B;**[!UICONTROL Developer]**&#x200B;のいずれかを選択し、画像をテンプレートページにドラッグします。 **[!UICONTROL ビルド]**/**[!UICONTROL テンプレートの基本]**&#x200B;に移動する前&#x200B;*の画像*&#x200B;を選択することもできます。 テンプレートページでは、次のツールを使用できます。

* 画像レイヤーの追加。 レイヤーを追加するには、画像をテンプレートページにドラッグします。
* テキストレイヤーの追加。 「**[!UICONTROL テキストツール]**」アイコンを選択します。 ポインターをドラッグしてテキストレイヤーのボックスを作成し、テキストページのツールでテキストを書式設定します。
* レイヤーのサイズと位置の変更。
* レイヤーの順序の変更。
* 画像およびテキストレイヤーへのシャドウ効果と光彩効果の適用。

[ テンプレートの作成](creating-template.md#creating_a_template)を参照してください。

## &#x200B;3. テンプレートパラメータの作成

次に、レイヤーのプロパティをパラメータ化して、URL 文字列に含めるレイヤープロパティを決定します。 パラメータにより、最大限の柔軟性でテンプレートを使用できるようになります。 レイヤープロパティをパラメータ化にした後に、それを動的に変更することができます。

レイヤーをパラメータ化するには、テンプレート ページでテンプレートを開き、レイヤー名の横にある&#x200B;**[!UICONTROL パラメーター]**&#x200B;を選択します。 「パラメーター」ページで、追加する各パラメーターの横にあるオプションを選択します。 [ テンプレートパラメーターの作成](creating-template-parameters.md#creating_template_parameters)を参照してください。

## &#x200B;4. テンプレートの公開

テンプレートを公開すると、Web サイトまたはアプリケーションに動的に配信できるように、Dynamic Media Image Serversに配置されます。 また、公開すると、URLがアクティブ化され、Dynamic Media Image ServerからWeb サイトまたはアプリケーションにテンプレートが呼び出されます。

必ず、テンプレートに関連付けられているすべての画像を公開してください。

テンプレートを公開するには、公開用にマークし、グローバルナビゲーションバーで「**[!UICONTROL 公開]**」を選択します。 次に、**[!UICONTROL 公開を送信]**&#x200B;を選択します。 [ テンプレートの公開](publishing-templates.md#publishing_templates)を参照してください。

## &#x200B;5. テンプレートをWeb ページにリンクする

Dynamic Media ClassicはテンプレートのURLを作成し、Dynamic Media Image Serverにテンプレートを公開するときにURLをアクティブにします。 これらのURL文字列は、テンプレートプレビューページからコピーできます。

参照パネルでテンプレートを選択し、**[!UICONTROL プレビュー]**&#x200B;を選択してテンプレートプレビューページを開きます。 テンプレートを配信するための画像プリセットを選択し、「**[!UICONTROL URLをコピー]**」ボタンをクリックします。 プレビューページからURLをコピーしたら、Web サイトまたはアプリケーションで使用できます。 「[ テンプレートをWeb ページにリンクする](linking-template-web-page.md#linking_a_template_to_a_web_page)」を参照してください。
