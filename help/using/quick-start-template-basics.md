---
title: "クイックスタート：基本テンプレート"
description: Adobe Dynamic Media Classicをすばやく使い始めるのに役立つ概要とクイックスタートの基本事項です。
uuid: 16d78cbb-f762-4263-aea9-5712eb933693
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: dd0fbb39-3f6a-496b-a9b6-63b11dcb823a
feature: Dynamic Media Classic
role: User
exl-id: bf695fee-821c-4396-829a-d57ccf475b0c
topic: Content Management
level: Intermediate
source-git-commit: 1b90beb99b161b76da81403f5aed9755b3a92c8b
workflow-type: tm+mt
source-wordcount: '852'
ht-degree: 20%

---

# クイックスタート：基本テンプレート{#quick-start-template-basics}

Template Basics は、Adobe Photoshopなどの画像編集アプリケーションのレイヤーファイルと同様に、動的に作成され、アドレス指定可能なレイヤー画像ファイルです。 PSD ファイルなどの、レイヤーが含まれている静的ファイルとは異なり、テンプレートにはパラメータを含めることができます。パラメータを使用して、画像の様々な要素をアドレス指定したりカスタマイズすることができます。

テンプレートには、複数の画像レイヤーとテキストレイヤーを含めることができます。レイヤーを含んだ静的ファイル ( レイヤーPSDファイルなど ) をテンプレートに変換し、Adobe Dynamic Media Classicでテンプレートを作成することができます。 Adobe Dynamic Media Classicにアップロードしたフォントを使用して、テンプレートでテキストレイヤーを作成できます。 テンプレートにテキストを追加した後、テキストの位置揃え、フォント、フォントサイズ、色を変更して書式を設定できます。

「パラメーター」ページを使用すると、テンプレートのあらゆる側面をアドレス可能なパラメーターに変換できます。 その際に、使用するレイヤー画像や、テンプレートで使用するテキスト値を変更できます。 パラメータは URL 文字列で渡されるため、パラメータを変更することで Image Server で生成される返信画像を動的にカスタマイズすることができます。

関連トピック [基本テンプレート](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/553_Template%20Basics_converted%20renamed_Dynamic%20Banners-AVS) トレーニングビデオ。

このクイックスタートは、基本テンプレートをすぐに使い始めるためのものです。

## 1.ファイルをアップロードします。

最初に、テンプレート用の PSD ファイルまたは画像ファイルをアップロードします。Adobe Dynamic Media ClassicではPSDに加えて多くの画像ファイル形式をサポートしていますが、テンプレートの場合は可逆TIFFおよび PNG 画像の使用が推奨されます。これは、透明性が確保されるためです。

テンプレートファイルを使用してPSDを作成する場合は、 **[!UICONTROL テンプレートを作成]** の **[!UICONTROL アップロードジョブオプション]** ダイアログボックスに表示されるPSDファイル。 また、 **[!UICONTROL レイヤーの命名]** オプションを使用することで、Adobe Dynamic Media Classicは、Adobe Dynamic Media Classicにアップロードする際にPSDレイヤーに名前を付ける方法を認識できます。

画像ファイルを使用している場合は、画像を切り抜くことができ、アップロード時に画像内のクリッピングパスからマスクを作成することもできます。

グローバルナビゲーションバーで、 **[!UICONTROL アップロード]** をクリックして、PSDファイルまたは他の画像ファイルをコンピューターからAdobe Dynamic Media Classic上のフォルダーにアップロードします。 詳しくは、 [テンプレートファイルのアップロード](uploading-template-files.md#uploading_template_files).

## 2.テンプレートを作成する

テンプレートファイルからPSDを作成するには、 **[!UICONTROL テンプレートを作成]** ファイルをアップロードする際に使用します。 画像からテンプレートを作成するには、グローバルナビゲーションバーで、に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL 基本テンプレート]**&#x200B;に値を入力し、キャンバスの幅と高さの単位を入力します。 ページの右上隅にある、次のいずれかを選択します。 **[!UICONTROL Designer]** または **[!UICONTROL 開発者]**&#x200B;をクリックし、画像をテンプレートページにドラッグします。 また、画像を選択することもできます *前* 次に進みます。 **[!UICONTROL ビルド]** > **[!UICONTROL 基本テンプレート]**. テンプレートページには、次のためのツールが用意されています。

* 画像レイヤーの追加。レイヤーを追加するには、画像をテンプレートページにドラッグします。
* テキストレイヤーの追加。を選択します。 **[!UICONTROL テキストツール]** アイコン。 ポインターをドラッグしてテキストレイヤー用のボックスを作成し、テキストページ上のツールでテキストを書式設定します。
* レイヤーのサイズと位置の変更。
* レイヤーの順序の変更。
* 画像およびテキストレイヤーへのシャドウ効果と光彩効果の適用。

詳しくは、 [テンプレートの作成](creating-template.md#creating_a_template).

## 3.テンプレートパラメーターを作成する

次に、レイヤーのプロパティをパラメータ化して、URL 文字列に含めるレイヤープロパティを決定します。パラメータにより、最大限の柔軟性でテンプレートを使用できるようになります。レイヤープロパティをパラメータ化にした後に、それを動的に変更することができます。

レイヤーをパラメータ化するには、テンプレートページでテンプレートを開き、「 」を選択します。 **[!UICONTROL パラメーター]** 画層名の横に表示されます。 [ パラメータ ] ページで、追加する各パラメータの横にあるオプションを選択します。 詳しくは、 [テンプレートパラメーターの作成](creating-template-parameters.md#creating_template_parameters).

## 4.テンプレートを公開する

テンプレートをパブリッシュすると、そのテンプレートがDynamic Media Image Server に配置され、Web サイトやアプリケーションに動的に配信できるようになります。 公開すると、URL がアクティベートされ、Dynamic Media Image Server から Web サイトまたはアプリケーションにテンプレートを呼び出します。

必ず、テンプレートに関連付けられているすべての画像を公開してください。

テンプレートを公開するには、公開用にマークし、グローバルナビゲーションバーで、 **[!UICONTROL 公開]**. 次に、 **[!UICONTROL 公開を送信]**. 詳しくは、 [テンプレートを公開](publishing-templates.md#publishing_templates).

## 5. Web ページへのテンプレートのリンク

Dynamic Media Classicは、テンプレートの URL を作成し、テンプレートをDynamic Media Image Server に公開する際に、その URL をアクティベートします。 これらの URL 文字列は、テンプレートプレビューページからコピーできます。

参照パネルでテンプレートを選択し、「 」を選択します。 **[!UICONTROL プレビュー]** をクリックして、「テンプレートプレビュー」ページを開きます。 テンプレートを配信するための画像プリセットを選択し、「 」を選択します。 **[!UICONTROL URL をコピー]**. プレビューページから URL をコピーした後、その URL を Web サイトまたはアプリケーションで使用できます。 詳しくは、[Web ページへのテンプレートのリンク](linking-template-web-page.md#linking_a_template_to_a_web_page)を参照してください。
