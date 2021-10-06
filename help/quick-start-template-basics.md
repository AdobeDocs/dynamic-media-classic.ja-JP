---
title: '"クイックスタート：基本テンプレート"'
description: Adobe Dynamic Media Classicですばやく作業を始めるのに役立つ概要とクイックスタートの基本を紹介します。
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 28%

---

# クイックスタート：基本テンプレート{#quick-start-template-basics}

Template Basics は、動的に作成され、Adobe Photoshopなどの画像編集アプリケーションのレイヤーファイルのような、アドレス指定可能なレイヤー画像ファイルです。 PSD ファイルなどの、レイヤーが含まれている静的ファイルとは異なり、テンプレートにはパラメータを含めることができます。パラメータを使用して、画像の様々な要素をアドレス指定したりカスタマイズすることができます。

テンプレートには、複数の画像レイヤーとテキストレイヤーを含めることができます。レイヤーを含む静的ファイル ( レイヤーPSDファイルなど ) をテンプレートに変換し、Adobe Dynamic Media Classicでテンプレートを作成できます。 Adobe Dynamic Media Classicにアップロードしたフォントを使用して、テンプレートでテキストレイヤーを作成できます。 テンプレートにテキストを追加した後に、テキストの配置、フォント、フォントサイズ、および色を変更して書式を設定することができます。

「パラメーター」ページを使用して、テンプレートのあらゆる側面をアドレス可能なパラメーターに変換できます。 このようにして、テンプレートで使用するレイヤー画像やテキスト値を変更することができます。パラメータは URL 文字列で渡されるため、パラメータを変更することで Image Server で生成される返信画像を動的にカスタマイズすることができます。

[ テンプレートの基本 ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) トレーニングビデオも参照してください。

このクイックスタートは、テンプレートの基本をすばやく習得できるように作られています。

## 1.ファイルをアップロードします

最初に、テンプレート用の PSD ファイルまたは画像ファイルをアップロードします。Adobe Dynamic Media Classicでは、PSDに加えて多くの画像ファイル形式をサポートしていますが、テンプレートでは可逆TIFFと PNG 画像の使用が推奨されています。これらの画像は透明性が確保されるからです。

PSDファイルを使用してPSDを作成する場合は、テンプレートファイルのアップロード時に **[!UICONTROL Upload Job Options]** ダイアログボックスで「**[!UICONTROL Create Template]**」を選択します。 また、「**[!UICONTROL レイヤーの命名]**」オプションを選択して、Adobe Dynamic Media ClassicがPSDレイヤーをAdobe Dynamic Media Classicにアップロードする際に、レイヤーに名前を付ける方法を把握できるようにします。

画像ファイルを使用する場合は、画像をアップロードするときに、画像を切り抜いたり、画像内のクリッピングパスからマスクを作成することができます。

グローバルナビゲーションバーで、「**[!UICONTROL Upload]**」を選択して、PSDファイルまたは他の画像ファイルをコンピューターからAdobe Dynamic Media Classic上のフォルダーにアップロードします。 [ テンプレートファイルのアップロード ](uploading-template-files.md#uploading_template_files) を参照してください。

## 2.テンプレートを作成する

PSDファイルからテンプレートを作成するには、ファイルをアップロードする際に「**[!UICONTROL テンプレートを作成]**」を選択します。 画像からテンプレートを作成するには、グローバルナビゲーションバーで **[!UICONTROL ビルド]** / **[!UICONTROL テンプレートの基本]** に移動し、キャンバスの幅と高さの測定値を入力します。 ページの右上隅付近で、「**[!UICONTROL Designer]**」または「**[!UICONTROL 開発者]**」を選択し、画像をテンプレートページにドラッグします。 ** の前に **[!UICONTROL ビルド]** / **[!UICONTROL テンプレートの基本]** に移動して、画像を選択することもできます。 テンプレートページには、次のためのツールが用意されています。

* 画像レイヤーの追加。レイヤーを追加するには、画像をテンプレートページにドラッグします。
* テキストレイヤーの追加。**[!UICONTROL テキストツール]** アイコンを選択します。 ポインタをドラッグして、テキストレイヤー用のボックスを作成する。次に、テキストページのツールでテキストを書式設定します。
* レイヤーのサイズと位置の変更。
* レイヤーの順序の変更。
* 画像およびテキストレイヤーへのシャドウ効果と光彩効果の適用。

[ テンプレートの作成 ](creating-template.md#creating_a_template) を参照してください。

## 3.テンプレートパラメータを作成する

次に、レイヤーのプロパティをパラメータ化して、URL 文字列に含めるレイヤープロパティを決定します。パラメータにより、最大限の柔軟性でテンプレートを使用できるようになります。レイヤープロパティをパラメータ化にした後に、それを動的に変更することができます。

画層をパラメータ化するには、[ テンプレート ] ページでテンプレートを開き、画層名の横にある [**[!UICONTROL パラメータ]**] を選択します。 [ パラメータ ] ページで、追加する各パラメータの横にあるオプションを選択します。 [ テンプレートパラメーターの作成 ](creating-template-parameters.md#creating_template_parameters) を参照してください。

## 4.テンプレートを公開する

テンプレートをパブリッシュすると、Dynamic Media Image Server に配置され、Web サイトやアプリケーションに動的に配信できるようになります。 公開すると、URL がアクティベートされ、Dynamic Media Image Server から Web サイトやアプリケーションにテンプレートを呼び出すことができます。

必ず、テンプレートに関連付けられているすべての画像を公開してください。

テンプレートを公開するには、公開用にマークし、グローバルナビゲーションバーで「**[!UICONTROL 公開]**」を選択します。 次に、「**[!UICONTROL 公開を送信]**」を選択します。 [ テンプレートの公開 ](publishing-templates.md#publishing_templates) を参照してください。

## 5. Web ページへのテンプレートのリンク

Dynamic Media Classicは、テンプレートの URL を作成し、Dynamic Media Image Server にテンプレートを公開する際に、その URL をアクティベートします。 これらの URL 文字列は、テンプレートのプレビューページからコピーできます。

参照パネルでテンプレートを選択し、「**[!UICONTROL プレビュー]**」を選択して、テンプレートのプレビューページを開きます。 テンプレートを配信するための画像プリセットを選択し、「**[!UICONTROL URL をコピー]**」を選択します。 プレビューページから URL をコピーすると、その URL を Web サイトまたはアプリケーションで使用できます。 詳しくは、[Web ページへのテンプレートのリンク](linking-template-web-page.md#linking_a_template_to_a_web_page)を参照してください。
