---
title: 画像の調整
description: Adobe Dynamic Media Classicで画像を調整する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/master_files
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 880ee6d0-cb0a-4d53-9056-f0b8b292136e
topic: Content Management
level: Intermediate
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 41%

---

# 画像の調整{#adjusting-an-image}

Adobe Dynamic Media Classicには、画像の外観を調整するための様々なコマンドが用意されています。 画像の反転、回転、ブラー、カラーバランスの変更、カラー化を行うことができます。 これらのコマンドを試すと、操作対象の画像に対するそれぞれの効果が確認できます。

関連トピック [画像のエイリアスの作成](adjusting-image.md#creating_an_alias_for_an_image).

**画像を調整するには：**

1. 画像のロールオーバー編集ボタンを選択して、「調整」を選択します。または、参照パネルで画像をダブルクリックして、詳細表示で開きます。
1. ウィンドウ下部で、サイズと画像プリセットを選択します。
1. の右側にあるコマンドを使用します。 `Adjust Editor` 画像を調整できるウィンドウ：

   * 「反転」オプションは、画像を水平または垂直方向に反転します。
   * 回転スライダを使用して画像を回転します。「回転」フィールドに値を入力すると、画像が回転します。正の値を入力すると、時計回りに回転し、負の値を入力すると、反時計回りに回転します。
   * ぼかしスライダまたはそれに対応するボックスは、画像のぼかしに使用します。値が大きいほど、画像のぼかしが強くなります。
   * コントラスト、明るさ、彩度、色相およびカラーバランスの各オプションを使用して、色と明るさを調整します。これらの効果は累積的に作用します。例えば、「マゼンタ」や「グリーン」の設定に対する変更は、「色相」設定の変更に追加されます。
   * の使用 `Colorize` シャドウとハイライトを保持しながら画像を色付けするオプション。 「色彩の統一」オプションに対する変更もまた、累積的です。[ 明るさ ] メニューから、 **[!UICONTROL 報酬なし]** そのため、自動輝度補正を無効にします。 コントラスト値を 0 に設定して、元の画像のコントラストの範囲を維持するか、0 を超える数値を使用して、コントラストの範囲を指定します。値を 100 に設定すると、コントラストが最大になります。一般的な値は、30 ～ 70 の範囲です。

1. 画像の調整が完了したら、次のいずれかの操作を行います。

   * を選択 **[!UICONTROL 保存]**.

   * 画像のオリジナルを置き換えるには、次を選択します **[!UICONTROL 名前を付けて保存]**.

     ドロップダウンリストで「」を選択します。 **[!UICONTROL オリジナルを置換]**&#x200B;を選択してから、 **[!UICONTROL 保存]**.

   * 画像を新しいプライマリ画像として保存するには、以下を選択します。 **[!UICONTROL 名前を付けて保存]**.

     ドロップダウンリストで「」を選択します。 **[!UICONTROL 新しいプライマリとして保存]**.
が含まれる **[!UICONTROL フォルダー名]** リストボックスで、新しいプライマリ画像を保存するフォルダーを選択します。
を選択 **[!UICONTROL 保存]**.

   * プライマリ・イメージの別のビューとしてイメージを保存するには、次の手順に従います。 画像のエイリアスを作成できます。を選択 **[!UICONTROL 名前を付けて保存]**.

     のドロップダウンリストから **[!UICONTROL 名前を付けて保存]** ダイアログ ボックスで、を選択します。 **[!UICONTROL プライマリの別のビューとして保存]**.
が含まれる **[!UICONTROL フォルダー名]** リストボックスで、新しいプライマリ画像を保存するフォルダーを選択します。
を選択 **[!UICONTROL 保存]**.

## 画像のエイリアスの作成 {#creating-an-alias-for-an-image}

画像を調整したら、プライマリ画像の別のビューとして保存できます。 これを行うには、を使用して画像のエイリアスを作成します **[!UICONTROL プライマリの別のビューとして保存]** 機能

**画像のエイリアスを作成するには：**

1. グリッド表示またはリスト表示で、 **[!UICONTROL 編集]** エイリアスを作成する画像の隣にあるドロップダウンリストを選択します。 **[!UICONTROL 調整]**.
1. ページの右下隅にあるを選択します。 **[!UICONTROL 名前を付けて保存]**.
1. のドロップダウンリストから **[!UICONTROL 名前を付けて保存]** ダイアログ ボックスで、を選択します。 **[!UICONTROL プライマリの別のビューとして保存]**.
1. **[!UICONTROL フォルダー名]**&#x200B;リストボックスで、エイリアス画像を保存するフォルダーを選択します。
1. **[!UICONTROL ファイル名]**&#x200B;フィールドに、エイリアスに使用する名前を入力します。
1. を選択 **[!UICONTROL 保存]**.
