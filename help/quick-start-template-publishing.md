---
title: '"Quick Start: Template publishing"'
seo-title: 「クイックスタート:印刷テンプレート」
description: 'null'
seo-description: すばやく習得できるように、はじめにおよびテンプレートの公開について簡潔に説明します。
uuid: 101b6211-2421-4565-8635-944315a5c512
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/template- publishing
discoiquuid: 03671fc1- ce3b-4fae- ad1f-53c99abcabde
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# Quick Start: Template publishing{#quick-start-template-publishing}

Adobe Dynamic Media Classic Web- to- Printを使用すると、顧客、クライアントおよびスタッフが簡単にカスタマイズしたりパーソナライズしたりできるブランド化されたプロ仕様のプリントコンテンツを作成できます。公開プロセス全体を通して、企業のコンテンツとブランドのアイデンティティを維持できます。エンドユーザは、プリントコンテンツのカスタマイズが許可された部分をカスタマイズすることができます。配信可能なカスタマイズされたプリント製品の例として、パーソナライズされたステーショナリ、名刺、ポスター、グリーティングカード、ラベル、伝票、ギフト、衣類、カレンダー、スクラップブックおよびフォトアルバムなどがあります。企業は、共通のブランドアイデンティティを維持した上で、様々な地域、フランチャイズ、店舗および支店向けにサイネージをカスタマイズすることができます。

まず、Adobe Illustratorでテンプレートを設計します。テンプレートでは、不変コンポーネントと可変コンポーネントが明確に定義され、可変コンポーネントがカスタマイズ可能なコンポーネントになります。例えば、Illustrator ファイル内のテキストをパラメータ化すると、エンドユーザは独自のテキストを入力できるようになります。同様に、背景色を可変コンポーネントとしてパラメータ化した場合は、異なる背景色と入れ替えることができます。

Dynamic Media Classicには、基本用途と高度な用途向けの2つの印刷テンプレートワークフローがあります。基本用途では、Adobe Illustratorでデザインを作成し、Dynamic Media Classicにアップロードして、SPSでパラメーターを使用して可変要素を定義します。高度な用途では、より包括的な可変性定義を行う必要があります。高度な使用例では、Adobe Illustratorで可変要素を作成し、ファイルをDynamic Media Classicにアップロードし、URL呼び出しを使用してXMLレベルでこれらの要素を直接操作します。このシナリオが呼び出さ *`*DOM manipulation*`*&#x200B;れます。

>[!NOTE]
>
>For more information about Dynamic Media Classic web-to-print workflows, template creation, parameterization, DOM manipulation, and more, see the Web-to-Print Workflow Guide here: [www.adobe.com/go/learn_s7_webtoprint_en](https://www.adobe.com/go/learn_s7_webtoprint_en) . Zipファイルをローカルハードドライブにダウンロードし、その内容（Dynamic Media Classic Web- To- Print Workflow Tutorialドキュメントおよびチュートリアルアセット）を抽出します。

**クイックスタート**

このクイックスタートでは、Illustrator ファイルを使用して高品質でカスタマイズ可能なプリント製品を作成するための基本的なワークフローについて説明します。

**1. 印刷テンプレート用の Illustrator ファイルを設計する**

Illustrator でテンプレートを設計します。高度な DOM 操作方法を使用してテンプレートをカスタマイズするには、Illustrator で可変要素の s7:elementID を定義します。

詳しくは、[Illustrator での初期テンプレートの作成](create-initial-template-illustrator.md#create_the_initial_template_in_illustrator)および[DOM 操作](dom-manipulation.md#dom_manipulation)を参照してください。

**2．Convert your template to Dynamic Media Classic FXG and upload it to Scene7 Publishing System**

Adobe Creative Cloud ユーザーは Web-to-Print 向け Adobe Illustrator プラグインを使用できます。このプラグインは、テンプレートをDynamic Media Classic FXGに変換します。テンプレートにフォントが含まれている場合は、FXG ファイルをアップロードする前に、対応するフォントファイルを Scene7 Publishing System にアップロードする必要があります。

[印刷テンプレート用のファイルのアップロード](upload-files-template-publishing.md#upload_files_for_template_publishing)を参照してください。

**3. Dynamic Media Classicでのパラメータの表示、定義、調整**

印刷テンプレートのプレビュー画面またはビルド画面で、パラメータを使って可変要素を定義および調整したり、結果をプレビューしたり、結果をテストすることができます。これらの画面では、次のことが可能です。

* パラメータを作成および変更する。
* パラメータのプロパティおよび属性の初期設定値を指定する。
* 「URL をコピー」をクリックして、プレビュー URL をクリップボードにコピーして、ブラウザウィンドウで結果をプレビューする。

Dynamic Media Classicでのテンプレート [のパラメータ化を参照](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)してください。

**4. FXG テンプレートの公開**

パラメータと属性の定義とテストが完了したら、ファイルを公開します。FXGテンプレートを公開すると、それがダイナミックメディアImage Serverに配置され、URLがアクティブになります。

必ず、FXG テンプレートに関連付けられているすべての画像とフォントを公開してください。

詳しくは、[FXG テンプレートの公開](dom-manipulation.md#publish_fxg_templates)を参照してください。

**5. URL を取得する**

URL 経由でテンプレートを Web サイトに埋め込んで、エンドユーザが可変コンテンツをパーソナライズできるようにすることができます。

詳しくは、[FXG テンプレートの Web ページへのリンク](linking-fxg-template-web-page.md#linking_an_fxg_template_to_a_web_page)を参照してください。