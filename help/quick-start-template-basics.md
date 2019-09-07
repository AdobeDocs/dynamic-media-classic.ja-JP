---
title: '"クイックスタート：基本テンプレート"'
seo-title: '"クイックスタート：基本テンプレート"'
description: 'null'
seo-description: すばやく習得できるように、概要と基本テンプレートの基本事項を紹介しています。
uuid: 16d78cbb- f762-4263- aea9-5712eb933693
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK_ PK/templates/template_ basics
discoiquuid: dd0fbb39-3f6a-496b- a9b6-63b11dcb823a
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# クイックスタート：基本テンプレート{#quick-start-template-basics}

基本テンプレートは、Adobe Photoshopなどの画像編集アプリケーションのレイヤーファイルと同じように、動的に作成され、アドレス指定可能なレイヤー画像ファイルです。PSD ファイルなどの、レイヤーが含まれている静的ファイルとは異なり、テンプレートにはパラメータを含めることができます。パラメータを使用して、画像の様々な要素をアドレス指定したりカスタマイズすることができます。

>[!NOTE]
>
>また、印刷テンプレートやAdobe IllustratorおよびAdobe InDesignのファイルを使用して、レイアウトベースのデザインからテンプレートを作成することもできます。詳しくは、[印刷テンプレート](quick-start-template-publishing.md)を参照してください。

テンプレートには、複数の画像レイヤーとテキストレイヤーを含めることができます。レイヤーPSDファイルなどのレイヤーを含んだ静的ファイルをテンプレートに変換したり、Dynamic Media Classicでテンプレートを作成したりできます。Scene7 Publishing System にアップロードしたフォントを使用して、テンプレート内にテキストレイヤーを作成することができます。テンプレートにテキストを追加した後に、テキストの配置、フォント、フォントサイズ、および色を変更して書式を設定することができます。

パラメータ画面を使用して、テンプレートのあらゆる要素をアドレス指定可能なパラメータに変換することができます。このようにして、テンプレートで使用するレイヤー画像やテキスト値を変更することができます。パラメータは URL 文字列で渡されるため、パラメータを変更することで Image Server で生成される返信画像を動的にカスタマイズすることができます。

**クイックスタート**

ここでは、基本テンプレートの操作方法をすばやく習得できるように、手順について簡潔に説明します。

**1. ファイルのアップロード**

最初に、テンプレート用の PSD ファイルまたは画像ファイルをアップロードします。Dynamic Media ClassicではPSDに加えて多くの画像ファイル形式がサポートされていますが、テンプレートには可逆圧縮形式のTIFFおよびPNG画像を使用することをお勧めします。これらの画像は、透明化が可能なテンプレートです。

PSD ファイルを使用してテンプレートを作成する場合は、PSD ファイルをアップロードするときに、アップロードオプションを設定ダイアログボックスで「テンプレートを作成」オプションを選択します。また、「レイヤー名」オプションを選択して、PSDレイヤーがScene7Publishing SystemにアップロードされたときにPSDレイヤーに名前を付ける方法を指定します。

画像ファイルを使用する場合は、画像をアップロードするときに、画像を切り抜いたり、画像内のクリッピングパスからマスクを作成することができます。

グローバルナビゲーションバーの「アップロード」ボタンを選択して、コンピュータから Scene7 Publishing System のフォルダに PSD ファイルまたはその他の画像ファイルをアップロードします。詳しくは、[テンプレートファイルのアップロード](uploading-template-files.md#uploading_template_files)を参照してください。

**2．テンプレートの作成**

PSD ファイルからテンプレートを作成するには、ファイルをアップロードするときに「テンプレートを作成」オプションを選択します。画像からテンプレートを作成するには、ビルド／基本テンプレートを選択し、カンバスの幅と高さを入力します。次に、「デザイナー」または「開発者」を選択して、画像をテンプレート画面にドラッグします。また、ビルド／基本テンプレートを選択する前に画像を選択することもできます。テンプレート画面には、次のことを行うためのツールがあります。:

* 画像レイヤーの追加。レイヤーを追加するには、テンプレート画面に画像をドラッグします。
* テキストレイヤーの追加。テキストツール  を選択し、ドラッグしてテキストレイヤー用のボックスを描画します。そして、テキスト画面上のツールを使用してテキストの形式を指定します。
* レイヤーのサイズと位置の変更。
* レイヤーの順序の変更。
* 画像およびテキストレイヤーへのシャドウ効果と光彩効果の適用。

詳しくは、[テンプレートの作成](creating-template.md#creating_a_template)を参照してください。

**3. テンプレートパラメータの作成**

次に、レイヤーのプロパティをパラメータ化して、URL 文字列に含めるレイヤープロパティを決定します。パラメータにより、最大限の柔軟性でテンプレートを使用できるようになります。レイヤープロパティをパラメータ化にした後に、それを動的に変更することができます。

レイヤーをパラメータ化するには、テンプレート画面でテンプレートを開いて、レイヤー名の隣にある「パラメータ」ボタンを選択します。パラメータ画面で、追加する各パラメータの隣にあるオプションを選択します。詳しくは、[テンプレートパラメータの作成](creating-template-parameters.md#creating_template_parameters)を参照してください。

**4.  テンプレートの公開**

テンプレートを公開すると、それがダイナミックメディアImage Serverに配置され、Webサイトやアプリケーションに動的に配信できるようになります。公開することで、ダイナミックメディアImage ServerからWebサイトやアプリケーションにテンプレートを呼び出すためのURLもアクティブになります。

必ず、テンプレートに関連付けられているすべての画像を公開してください。

テンプレートを公開するには、公開用にマークして、グローバルナビゲーションバーの「公開」ボタンを選択します。次に、「公開を開始」ボタンを選択します。詳しくは、[テンプレートの公開](publishing-templates.md#publishing_templates)を参照してください。

**5. Web ページへのテンプレートのリンク**

テンプレートのURLをダイナミックメディアImage Serverに公開すると、テンプレートのURLが作成され、アクティブになります。これらの URL 文字列は、テンプレートのプレビュー画面からコピーすることができます。

参照パネルでテンプレートを選択し、「プレビュー」ボタンをクリックして、テンプレートのプレビュー画面を開きます。テンプレートを配信するための画像プリセットを選択して、「URL をコピー」ボタンを選択します。プレビュー画面から URL をコピーして、その URL を Web サイトやアプリケーションで使用することができます詳しくは、[Web ページへのテンプレートのリンク](linking-template-web-page.md#linking_a_template_to_a_web_page)を参照してください。