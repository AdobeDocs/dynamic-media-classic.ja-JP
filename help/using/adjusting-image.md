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
autotag-review: '2026-05-13T17:38:08.783Z'
TQID: 'https://experienceleague.adobe.com/Gze3kMTnn5xWFZ4uUW-aNo5VASF2ncV7T1jvcsRadaQ'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 578
ht-degree: 35%

---

# 画像の調整{#adjusting-an-image}

Adobe Dynamic Media Classicには、画像の外観を調整するための様々なコマンドが用意されています。 反転、回転、ぼかし、カラーバランスの変更、画像の色付けを行うことができます。 これらのコマンドを試すと、操作対象の画像に対するそれぞれの効果が確認できます。

[画像のエイリアスの作成](adjusting-image.md#creating_an_alias_for_an_image)も参照してください。

**画像を調整するには：**

1. 画像のロールオーバー編集ボタンを選択して「調整」を選択するか、参照パネルで画像をダブルクリックして詳細表示で開きます。
1. ウィンドウ下部で、サイズと画像プリセットを選択します。
1. `Adjust Editor` ウィンドウの右側にあるコマンドを使用して、画像を調整できます。

   * 「反転」オプションは、画像を水平または垂直方向に反転します。
   * **[!UICONTROL 回転子]** スライダーを使用して、画像を回転します。 **[!UICONTROL Rotator]** フィールドに値を入力して、画像を回転させることができます。 正の値を入力すると、時計回りに回転し、負の値を入力すると、反時計回りに回転します。
   * ぼかしスライダまたはそれに対応するボックスは、画像のぼかしに使用します。 値が大きいほど、画像のぼかしが強くなります。
   * コントラスト、明るさ、彩度、色相およびカラーバランスの各オプションを使用して、色と明るさを調整します。 これらの効果は累積的に作用します。 例えば、「マゼンタ」や「グリーン」の設定に対する変更は、「色相」設定の変更に追加されます。
   * シャドウとハイライトを保持しながら、`Colorize` オプションを使用して画像を色付けします。 「色彩の統一」オプションに対する変更もまた、累積的です。 明るさメニューから、**[!UICONTROL 補正なし]**&#x200B;を選択して、自動輝度補正を無効にします。 コントラスト値を 0 に設定して、元の画像のコントラストの範囲を維持するか、0 を超える数値を使用して、コントラストの範囲を指定します。 値を 100 に設定すると、コントラストが最大になります。 一般的な値は30～70の範囲です。

1. 画像の調整が完了したら、次のいずれかの操作を行います。

   * **[!UICONTROL 保存]**&#x200B;を選択します。

   * 画像の元の画像を置き換えるには、**[!UICONTROL 別名で保存]**&#x200B;を選択します。

     ドロップダウンリストで「**[!UICONTROL オリジナルを置換]**」を選択し、「**[!UICONTROL 保存]**」を選択します。

   * 画像を新しいプライマリ画像として保存するには、**[!UICONTROL 別名で保存]**&#x200B;を選択します。

     ドロップダウンリストで、**[!UICONTROL 新しいプライマリとして保存]**&#x200B;を選択します。
**[!UICONTROL フォルダー名]** リストボックスで、新しいプライマリイメージを保存するフォルダーを選択します。
**[!UICONTROL 保存]**&#x200B;を選択します。

   * プライマリ画像の別のビューとして画像を保存します。 画像のエイリアスを作成できます。 **[!UICONTROL 別名で保存]**&#x200B;を選択します。

     **[!UICONTROL 別名で保存]** ダイアログボックスのドロップダウンリストから、**[!UICONTROL プライマリ]**&#x200B;の別のビューとして保存を選択します。
**[!UICONTROL フォルダー名]** リストボックスで、新しいプライマリイメージを保存するフォルダーを選択します。
**[!UICONTROL 保存]**&#x200B;を選択します。

## 画像のエイリアスの作成 {#creating-an-alias-for-an-image}

画像を調整した場合は、プライマリ画像の別のビューとして保存できます。 これを行うには、**[!UICONTROL プライマリ]**&#x200B;機能の別のビューとして保存を使用して、画像のエイリアスを作成します。

**画像のエイリアスを作成するには：**

1. グリッド表示またはリスト表示で、エイリアスを作成する画像の横にある&#x200B;**[!UICONTROL 編集]** ドロップダウンリストで、**[!UICONTROL 調整]**&#x200B;を選択します。
1. ページの右下隅にある「**[!UICONTROL 別名で保存]**」を選択します。
1. **[!UICONTROL 別名で保存]** ダイアログボックスのドロップダウンリストから、**[!UICONTROL プライマリ]**&#x200B;の別のビューとして保存を選択します。
1. **[!UICONTROL フォルダー名]**&#x200B;リストボックスで、エイリアス画像を保存するフォルダーを選択します。
1. **[!UICONTROL ファイル名]**&#x200B;フィールドに、エイリアスに使用する名前を入力します。
1. **[!UICONTROL 保存]**&#x200B;を選択します。
