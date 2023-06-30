---
title: コンテンツのバリエーションを管理
description: Adobe Dynamic Media Classicでコンテンツのバリエーションを管理する方法を説明します。
uuid: 1e40a526-02f8-41d9-886f-6d094546bc13
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/template_basics
discoiquuid: aa129b0e-fc73-4fc2-a894-4560b3f46c4f
feature: Dynamic Media Classic
role: User
exl-id: 65b8c314-7ec1-417f-8a7b-aa13762072a1
topic: Content Management
level: Intermediate
source-git-commit: d82f816553f807b514f4690827dab672a6baf690
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 55%

---

# コンテンツのバリエーションを管理{#managing-content-variations}

テンプレートセットを使用して、アセットのバリエーションを公開する方法を管理します。

テンプレートのバリエーションを管理するために、テンプレートセットを作成します。サイト上のコードを変更せずに、どのバリエーションが使用されるかを制御できます。この方法を使用すると、コンテンツ管理者は、Web コード内の URL を変更する必要なく、コンテンツを回転できます。

ユニバーサル URL は、セット内にリストされている順序に基づいて、ページに表示されるテンプレートのバリエーションを表示するために使用されます。 テンプレートセットリストの上端にあるテンプレートは、常に公開されます。

リスト内にある任意の画像プリセットを使用できます。画像プリセット URL はユニバーサル URL に似ています。これらは、複数の画像プリセット URL にすることもできます。

1. に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL テンプレートセット]**.
1. ビルダーで、テンプレートを選択し、「 **[!UICONTROL 追加/プレビュー]**.
1. テンプレートのプロパティを変更し、「 」を選択します。 **[!UICONTROL 名前を付けて保存]** をクリックして別のバージョンを作成します。
1. 名前を入力し、「 」を選択します。 **[!UICONTROL 保存]**.

   アセットとテンプレートの両方を公開する必要があります。

1. 詳細ページに移動して、「URL」セクションからコピー先 URL を取得します。

テンプレートを新しい位置までドラッグして、テンプレート順序の中で個別のテンプレートを移動する（例えば、リストの上端に移動する）ことができます。もう一度公開して、新しい順序を送信します。

>[!NOTE]
>
>必要に応じて、キャッシュをクリアして変更を確認します。 Web サイトで変更結果が表示されるのは、キャッシュサイクルを通じて変更結果が伝達された後のみです。
