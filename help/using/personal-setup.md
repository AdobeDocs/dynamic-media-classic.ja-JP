---
title: 個人設定
description: Adobe Dynamic Media Classicの個人設定画面では、すべてのユーザーが設定を変更できます。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
autotag-review: '2026-05-13T20:06:35.284Z'
TQID: 'https://experienceleague.adobe.com/u57YFGIgu4AwlDGLqXRDdT2os-RBYCQK-voETH58Wt4'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 841
ht-degree: 19%

---

# 個人設定 {#personal-setup}

すべてのユーザが個人設定画面の設定を変更できます。 個人用セットアップ画面を開くには、**[!UICONTROL セットアップ]** > **[!UICONTROL 個人用セットアップ]**&#x200B;に移動します。

>[!NOTE]
>
>個人設定の画面には、Adobe Dynamic Media Classicで使用しているユーザーのロール（会社管理者、管理者、ユーザー）が一覧表示されます。

個人設定は、参照パネルのデフォルトの動作、電子メールの受信方法、パスワード設定を制御します。 これらの設定を変更した後、**[!UICONTROL 保存]**&#x200B;を忘れずに選択してください。

## マイアカウント情報

アカウント名、氏名、ユーザ名（電子メールアドレス）および割り当てられたユーザの役割が示されます。

## デスクトップ

* **画像キャッシュを消去**: Adobe Dynamic Mediaでキャッシュされたすべての画像ファイルをコンピューターから削除します。
* **アセットキャッシュをクリア**: Adobe Dynamic Mediaがコンピューターからアセットファイルをすべて削除します。

デスクトップアプリを使用して画像とアセットキャッシュをクリアするだけでなく、ファイルシステムから直接キャッシュを手動でクリアできます。 オペレーティングシステムに応じて、次の場所に移動します。

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## CREATIVE SUITE EXTENSION

**Adobe Dynamic Media Creative Suite拡張機能をインストールするには：**

1. Adobe Dynamic Media Classicのツールバーで、**[!UICONTROL Setup]** > **[!UICONTROL Personal Setup]**&#x200B;に移動し、Creative Suite Extensionで「**[!UICONTROL 今すぐダウンロード]**」を選択して`s7csxs.zxp` ファイルをダウンロードします。
1. 拡張機能に関する追加情報については、**[!UICONTROL インストール]**&#x200B;および&#x200B;**[!UICONTROL 必要システム構成]**&#x200B;のリンクを選択してください。

<!--    
A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: 
-->

<!--
#### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li>Select libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, select flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, select win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator's package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator's plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator.
-->

## ブラウザ

* **[!UICONTROL サムネールサイズ]**：参照パネルのグリッドビューで、サムネール画像のデフォルトサイズを指定します。
* **[!UICONTROL デフォルトのアセットライブラリビュー]**: ビルドセットのアセットライブラリ内のアセットがサムネールとして表示されるか、名前で表示されるかを指定します。 アセットライブラリで大量のアセットを操作する場合は、アセットを名前順に表示できます。 例えば、PDF ファイルを多く含む大規模な eCatalog を作成している場合は、アセットを名前順で表示してリストを短くすることができます。
* **[!UICONTROL デフォルトのブラウズ並べ替え順序]**：参照パネルにアセットがデフォルトで表示される順序を指定します。 メニューで並べ替え条件を選択して、昇順または降順のどちらで並べ替えるかを指定します。
* **[!UICONTROL 既定の参照の場所]**：参照の場所を既定、最後に参照したフォルダー、または移動して特定の場所に設定して特定できます。 また、ファイルやフォルダを昇順または降順に並べ替えるよう参照場所を設定できます。
* **[!UICONTROL 既定の参照ビュー]**：最初に参照パネルを開いたときに表示される既定のビューがグリッド ビューかリスト ビューかを指定します。
* **[!UICONTROL スプラッシュ スクリーン表示]**：ようこそスプラッシュ スクリーンを含むスプラッシュ スクリーンを表示するかどうかを指定します。
* **[!UICONTROL ツールヒントを表示]**: ボタン、メニュー、ナビゲーションリンクにポインターを移動したときにツールヒントが表示されるかどうかを指定します。 ツールヒントでは、画面上のユーザーインターフェイス項目について説明します。
* **[!UICONTROL チェッカーボードの背景]**：画像の背後にチェッカーボードレイヤーを表示し、アルファチャンネルを含む画像の透明部分を簡単に確認できます。
* **[!UICONTROL ファイルサイズを表示]**：閲覧中のアセットのファイルサイズを表示します。
* **[!UICONTROL 検索にUDFを含める]**：実行するほとんどのメタデータ検索のシステムパフォーマンスを向上させるには、選択を解除します（デフォルト）。

  メタデータ検索の多くの場合に、ユーザ定義フィールドを含めることで利点がある場合は、このオプションを選択して有効にすることができます。 代わりに、高度な検索を使用すると、ユーザー定義のフィールドを含めるよりも、より適切で高速な検索エクスペリエンスを提供できます。

  詳しくは、[詳細検索の実行](searching-assets.md#conducting_an_advanced_search)を参照してください。

  [ユーザ定義フィールド](application-setup.md#user_defined_fields)も参照してください。

* **[!UICONTROL 基本検索タイプ]**: 2つのオプションから選択できます：**[!UICONTROL 次の文字列を含む]**&#x200B;は、指定された値の全文字列を検索します。**[!UICONTROL 次の文字列の先頭から]**&#x200B;検索を開始し、**[!UICONTROL 次の文字列を含む]**&#x200B;よりも速く結果を返します。 いずれのオプションも、管理者が&#x200B;**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Application General Settings]**&#x200B;で設定したデフォルトを上書きします。
* **[!UICONTROL コマンドフィードバックを表示]**: サーバーへのコマンドリクエストの表示をオンにするには選択します。オフにするには選択解除します。
* **[!UICONTROL 書き出し中にダイアログを表示]**：書き出し中にポップアップダイアログボックスを表示する場合に選択します。 このオプションの選択を解除（オフ）した場合でも、ジョブページに移動して書き出しの結果を取得できます。

## 電子メール

* **[!UICONTROL 電子メールオプション]**: アップロードと公開のジョブが完了したときに、Adobe Dynamic Media Classicから電子メールで通知する方法を選択します。 ジョブ完了通知は、警告またはエラーが発生した場合のみ受信することができます。
* **[!UICONTROL メール範囲]**：会社のすべてのジョブの電子メールを受信するか、開始するジョブのアップロードと公開に関する電子メールのみを受信するかを指定します。
* **[!UICONTROL 電子メールの種類]**: アップロード ジョブと公開ジョブが完了したときに通知を受け取るかどうかを指定します。

## 言語

* **[!UICONTROL 優先言語]**: インターフェイスに使用する言語を決定します。

## パスワード

* **[!UICONTROL 現在のパスワード]**：現在のパスワードを入力します。
* **[!UICONTROL 新しいパスワード]**：新しい有効なパスワードを入力します。 パスワードは次の要件を満たしている必要があります。
   * 8～25文字の範囲で指定してください。
   * 1つ以上の小文字を含みます。
   * 大文字を少なくとも1つ含みます。
   * 1つ以上の数値を含めてください。
   * 次のいずれかの特殊文字が含まれています：`# $ &: _ : { }`
* **[!UICONTROL パスワードを再入力]**：新しいパスワードを再入力して、正しく入力していることを確認します。
* **[!UICONTROL パスワードの有効期限]**：セキュリティ対策として、パスワードの有効期限が72日後に切れるかどうかを指定します。 「はい」を選択した場合は、72日後にパスワードを作成するように求められます。
