---
title: クイックスタート：基本テンプレート
description: Adobe Dynamic Media Classicをすぐに使い始めるのに役立つ、テンプレートの基本の概要とクイックスタートです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 17%

---

# クイックスタート：基本テンプレート{#quick-start-template-basics}

テンプレートの基本は、Adobe Photoshopなどの画像編集アプリケーションで、レイヤーファイルなどのアドレス指定可能なレイヤー化された画像ファイルを動的に作成するものです。 PSD ファイルなどの、レイヤーが含まれている静的ファイルとは異なり、テンプレートにはパラメータを含めることができます。パラメータを使用して、画像の様々な要素をアドレス指定したりカスタマイズすることができます。

テンプレートには、複数の画像レイヤーとテキストレイヤーを含めることができます。レイヤーPSD ファイルなどのレイヤーを含んだ静的ファイルをテンプレートに変換し、Adobe Dynamic Media Classicでテンプレートを作成できます。 Adobe Dynamic Media Classicにアップロードしたフォントを使用して、テンプレート内にテキストレイヤーを作成できます。 テンプレートにテキストを追加した後、その位置揃え、フォント、フォントサイズ、カラーを変更して、テキストの書式を設定できます。

パラメーターページを使用すると、テンプレートのあらゆる側面をアドレス可能なパラメーターに変換できます。 その際に、使用するレイヤー化された画像や、テンプレートで使用するテキスト値を変更できます。 パラメーターは URL 文字列と共に渡され、任意のパラメーターを変更できるので、Image Server から生成された返信画像を動的にカスタマイズできます。

[ テンプレートの基本 ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) トレーニングビデオも参照してください。

このクイックスタートは、テンプレートの基本をすぐに使い始められるように設計されています。

## &#x200B;1. ファイルをアップロードする

最初に、テンプレート用の PSD ファイルまたは画像ファイルをアップロードします。Adobe Dynamic Media Classicは、PSDに加えて多くの画像ファイル形式をサポートしていますが、テンプレートには透明度が高い可逆圧縮TIFFおよび PNG 画像を使用することをお勧めします。

PSD ファイルを使用してテンプレートを作成する場合は、PSD ファイルをアップロードする際に、**[!UICONTROL アップロードジョブオプション]** ダイアログボックスで **[!UICONTROL テンプレートを作成]** を選択します。 また、「**[!UICONTROL レイヤーの名前]**」オプションを選択すると、Adobe Dynamic Media Classicにアップロードされる際に、PSD レイヤーの命名方法をAdobe Dynamic Media Classicが把握できます。

画像ファイルを使用している場合は、画像を切り抜くことも、画像のアップロード時に画像のクリッピングパスからマスクを作成することもできます。

グローバルナビゲーションバーの **[!UICONTROL アップロード]** を選択して、PSD ファイルまたは他の画像ファイルをコンピューターからAdobe Dynamic Media Classicのフォルダーにアップロードします。 [ テンプレートファイルのアップロード ](uploading-template-files.md#uploading_template_files) を参照してください。

## &#x200B;2. テンプレートの作成

PSD ファイルからテンプレートを作成するには、ファイルをアップロードする際に「**[!UICONTROL テンプレートを作成]**」を選択します。 画像からテンプレートを作成するには、グローバルナビゲーションバーで **[!UICONTROL 作成]**/**[!UICONTROL テンプレートの基本]** に移動し、キャンバスの幅と高さの値を入力します。 ページの右上隅付近にある **[!UICONTROL Designer]** または **[!UICONTROL デベロッパー]** を選択して、画像をテンプレートページにドラッグします。 また、画像を選択することもできます *前に***[!UICONTROL 作成]**/**[!UICONTROL テンプレートの基本]** に移動します。 テンプレートページには、次の用途に使用できるツールが用意されています。

* 画像レイヤーの追加。レイヤーを追加するには、画像をテンプレートページにドラッグします。
* テキストレイヤーの追加。**[!UICONTROL テキストツール]** アイコンを選択します。 ポインターをドラッグしてテキストレイヤーのボックスを作成し、「テキスト」ページのツールを使用してテキストの書式を設定します。
* レイヤーのサイズと位置の変更。
* レイヤーの順序の変更。
* 画像およびテキストレイヤーへのシャドウ効果と光彩効果の適用。

[ テンプレートの作成 ](creating-template.md#creating_a_template) を参照してください。

## &#x200B;3. テンプレートパラメーターの作成

次に、レイヤーのプロパティをパラメータ化して、URL 文字列に含めるレイヤープロパティを決定します。パラメータにより、最大限の柔軟性でテンプレートを使用できるようになります。レイヤープロパティをパラメータ化にした後に、それを動的に変更することができます。

レイヤーをパラメーター化するには、テンプレートページでテンプレートを開き、レイヤー名の横にある **[!UICONTROL パラメーター]** を選択します。 パラメーターページで、追加する各パラメーターの横にあるオプションを選択します。 [ テンプレートパラメーターの作成 ](creating-template-parameters.md#creating_template_parameters) を参照してください。

## &#x200B;4. テンプレートの公開

テンプレートを公開すると、Web サイトやアプリケーションに動的に配信できるように、テンプレートが Dynamic Media 画像サーバーに配置されます。 公開すると、Dynamic Media Image Server から Web サイトまたはアプリケーションにテンプレートを呼び出す URL もアクティブ化されます。

必ず、テンプレートに関連付けられているすべての画像を公開してください。

テンプレートを公開するには、公開用にマークを付け、グローバルナビゲーションバーで「**[!UICONTROL 公開]**」を選択します。 次に、「**[!UICONTROL 公開を送信]**」を選択します。 [ テンプレートの公開 ](publishing-templates.md#publishing_templates) を参照してください。

## &#x200B;5. Web ページにテンプレートをリンクする

Dynamic Media Classicはテンプレートの URL を作成し、Dynamic Media Image Server にテンプレートを公開する際に URL をアクティベートします。 これらの URL 文字列は、テンプレートのプレビューページからコピーできます。

参照パネルでテンプレートを選択し、「**[!UICONTROL プレビュー]** を選択して、テンプレートプレビューページを開きます。 テンプレートを配信するための画像プリセットを選択し、「**[!UICONTROL URL をコピー]**」ボタンをクリックします。 プレビューページから URL をコピーすると、web サイトやアプリケーションで使用できます。 [Web ページへのテンプレートのリンク ](linking-template-web-page.md#linking_a_template_to_a_web_page) を参照してください。
