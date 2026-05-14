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
autotag-review: '2026-05-13T17:40:29.070Z'
TQID: 'https://experienceleague.adobe.com/KjKdz4CAeSdJ3P-LKvdmsoGlkroeOZ60AvydF2FBHaI'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 248
ht-degree: 44%

---

# コンテンツのバリエーションの管理{#managing-content-variations}

テンプレートセットを使用して、アセットのバリエーションを公開する方法を管理します。

テンプレートのバリエーションを管理するために、テンプレートセットを作成します。 サイト上のコードを変更せずに、どのバリエーションが使用されるかを制御できます。 この方法は、コンテンツマネージャーが、IT部門にweb コードのURLを変更せずにコンテンツをローテーションするのに役立ちます。

ユニバーサル URLは、セットにリストされている順序に基づいて、ページに表示されるテンプレートのバリエーションを表示するために使用されます。 テンプレートセットリストの上端にあるテンプレートは、常に公開されます。

リストから任意の画像プリセット URLを使用できます。 画像プリセット URLは、ユニバーサル URLのようなものです。 複数の画像プリセット URLを指定できます。

1. **[!UICONTROL ビルド]** > **[!UICONTROL テンプレートセット]**&#x200B;に移動します。
1. ビルダーで、テンプレートを選択し、**[!UICONTROL 追加/プレビュー]**&#x200B;を選択します。
1. テンプレートのプロパティを変更し、**[!UICONTROL 別名で保存]**&#x200B;を選択して、別のバージョンを作成します。
1. 名前を入力し、**[!UICONTROL 保存]**&#x200B;を選択します。

   アセットとテンプレートの両方を公開する必要があります。

1. 詳細ページに移動して、「URL」セクションからコピー先 URL を取得します。

テンプレートを新しい位置までドラッグして、テンプレート順序の中で個別のテンプレートを移動する（例えば、リストの上端に移動する）ことができます。 もう一度公開して、新しい順序を送信します。

>[!NOTE]
>
>必要に応じて、キャッシュをクリアして変更を確認します。 Web サイトで変更結果が表示されるのは、キャッシュサイクルを通じて変更結果が伝達された後のみです。
