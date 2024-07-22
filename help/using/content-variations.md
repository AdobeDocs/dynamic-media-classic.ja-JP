---
title: コンテンツのバリエーションの管理
description: Adobe Dynamic Media Classicでコンテンツのバリエーションを管理する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
feature: Dynamic Media Classic
role: User
exl-id: 65b8c314-7ec1-417f-8a7b-aa13762072a1
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 44%

---

# コンテンツのバリエーションの管理{#managing-content-variations}

テンプレートセットを使用して、アセットのバリエーションを公開する方法を管理します。

テンプレートのバリエーションを管理するために、テンプレートセットを作成します。サイト上のコードを変更せずに、どのバリエーションが使用されるかを制御できます。この方法は、IT 担当者が web コード内の URL を変更することなく、コンテンツ管理者がコンテンツを回転させるのに役立ちます。

ユニバーサル URL は、セットにリストされている順序に基づいて、ページに表示されるテンプレートバリエーションを表示するために使用されます。 テンプレートセットリストの上端にあるテンプレートは、常に公開されます。

リストの任意の画像プリセット URL を使用できます。 画像プリセット URL はユニバーサル URL に似ています。 複数の画像プリセット URL を指定できます。

1. **[!UICONTROL ビルド]**/**[!UICONTROL テンプレートセット]** に移動します。
1. ビルダーで、テンプレートを選択し、「**[!UICONTROL 追加/プレビュー]**」を選択します。
1. テンプレートのプロパティを変更し、「**[!UICONTROL 名前を付けて保存]**」を選択して別のバージョンを作成します。
1. 名前を入力し、「**[!UICONTROL 保存]**」を選択します。

   アセットとテンプレートの両方を公開する必要があります。

1. 詳細ページに移動して、「URL」セクションからコピー先 URL を取得します。

テンプレートを新しい位置までドラッグして、テンプレート順序の中で個別のテンプレートを移動する（例えば、リストの上端に移動する）ことができます。もう一度公開して、新しい順序を送信します。

>[!NOTE]
>
>必要に応じて、キャッシュをクリアして変更内容を確認します。 Web サイトで変更結果が表示されるのは、キャッシュサイクルを通じて変更結果が伝達された後のみです。
