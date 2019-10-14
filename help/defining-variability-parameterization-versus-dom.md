---
title: '"可変性の定義：パラメータ化と DOM 操作について"'
seo-title: '"可変性の定義：パラメータ化と DOM 操作について"'
description: 'null'
seo-description: パラメータ化とDOM操作を使用して可変性を定義する方法を説明します。
uuid: dce424f2-07d8-4703-aa3a-40d2eee12f74
contentOwner: 管理者
content-type: 参照
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template-publishing
discoiquuid: 5b844afe-ac55-4dd2-8fe8-125a9c9af948
translation-type: tm+mt
source-git-commit: 6fff3699f8a08af433df3f3a7790a11bf9d05b00

---


# 可変性の定義：パラメータ化と DOM 操作について{#defining-variability-parameterization-versus-dom-manipulation}

Dynamic Media Classicには、テンプレート内の可変コンテンツを管理する2つの方法が用意されています。 どちらの方法でも、Illustratorで初期テンプレートを設計し、そのテンプレートをDynamic Media Classic FXGファイル形式に変換して、SPSにアップロードします。 ただし、これらの手順は可変要素に対する制御の度合いと方法の使用に必要なスキルが異なります。

* **Scene7 Publishing systemでのパラメータ化**&#x200B;この手法では、SPSの印刷テンプレートのビルド画面とプレビュー画面、またはWeb-to-Print向けAdobe Illustratorプラグインで可変性を定義する必要があります。 いずれの手順にも、パラメーターの作成、パラメーター値の割り当て、および結果のテストを行うためのツールが用意されています。

* **DOM操作の使用**&#x200B;この方法を使用すると、XMLレベルでデザインとテンプレートを制御できます。 ダイナミックMedia Classic FXGファイルはXMLです。 この手法では、XML DOM（表示オブジェクトモデル）を経由してデザインテンプレートを直接編集できます。Illustrator で、可変要素に s7:elementID でマークを付けて、URL コマンドを使用して後で操作します。

>[!MORELIKETHIS]
>
>* [ダイナミックメディアクラシックでのテンプレートのパラメータ化](parameterizing-template-scene7.md#parameterizing_a_template_in_scene7)
>* [DOM 操作](dom-manipulation.md#dom_manipulation)

