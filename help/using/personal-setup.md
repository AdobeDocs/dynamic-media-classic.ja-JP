---
title: 個人設定
description: すべてのユーザーが、Adobe Dynamic Media Classicの個人設定画面で設定を変更できます。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 8dc990a1fb1355b00fa4839e14b92bb6562d40b4
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 19%

---

# 個人設定 {#personal-setup}

すべてのユーザが個人設定画面の設定を変更できます。個人設定画面を開くには、**[!UICONTROL 設定]**/**[!UICONTROL 個人設定]** に移動します。

>[!NOTE]
>
>個人設定画面には、Adobe Dynamic Media Classicで自分が持っているユーザーロールが一覧表示されます。会社管理者、管理者またはユーザーです。

個人用セットアップの設定は、参照パネルの既定の動作、電子メールの受信方法、およびパスワードの設定を制御します。 これらの設定を変更したら、必ず **[!UICONTROL 保存]** を選択してください。

## マイアカウント情報

アカウント名、氏名、ユーザ名（電子メールアドレス）および割り当てられたユーザの役割が示されます。

## デスクトップ

* **画像キャッシュをクリア**:AdobeのDynamic Mediaでキャッシュされたすべての画像ファイルをコンピューターから削除します。
* **アセットキャッシュをクリア**:Dynamic MediaがアセットファイルをキャッシュするすべてのAdobeーをコンピューターから削除します。

デスクトップアプリケーションを使用して画像とアセットのキャッシュをクリアする以外に、ファイルシステムから直接キャッシュを手動でクリアすることもできます。 オペレーティングシステムに応じて、次に移動します。

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## CREATIVE SUITE EXTENSION

**Adobe Dynamic Media Creative Suite拡張機能をインストールするには：**

1. Adobe Dynamic Media Classicのツールバーで、**[!UICONTROL 設定]**/**[!UICONTROL 個人設定]** に移動し、「Creative Suiteの拡張子」の下の **[!UICONTROL 今すぐダウンロード]** を選択して、`s7csxs.zxp` ファイルをダウンロードします。
1. **[!UICONTROL インストール]** リンクおよび **[!UICONTROL システム要件]** リンクを選択すると、拡張機能に関する追加情報が表示されます。

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

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

The plug-in is now available for you to use in Adobe Illustrator. -->

## ブラウザ

* **[!UICONTROL サムネールサイズ]**：参照パネルのグリッド表示のサムネール画像のデフォルトサイズを決定します。
* **[!UICONTROL デフォルトのアセットライブラリ表示]**：ビルドセット用のアセットライブラリ内のアセットをサムネールとして表示するか名前で表示するかを決定します。 アセットライブラリで大量のアセットを操作する場合は、アセットを名前順に表示できます。例えば、PDF ファイルを多く含む大規模な eCatalog を作成している場合は、アセットを名前順で表示してリストを短くすることができます。
* **[!UICONTROL デフォルトの参照の並べ替え順序]**：参照パネルでデフォルトに表示されるアセットの順序を指定します。 メニューで並べ替え条件を選択して、昇順または降順のどちらで並べ替えるかを指定します。
* **[!UICONTROL デフォルトの参照場所]**：参照場所をデフォルト、最後に参照されたフォルダー、または移動先で識別できる特定の場所に設定できます。 また、ファイルやフォルダを昇順または降順に並べ替えるよう参照場所を設定できます。
* **[!UICONTROL デフォルトの参照表示]**：最初に参照パネルを開いたときに表示されるデフォルトの表示を、グリッド表示またはリスト表示のいずれにするかを指定します。
* **[!UICONTROL スプラッシュ画面の表示]**:「ようこそ」スプラッシュ画面を含む、スプラッシュ画面を表示するかどうかを決定します。
* **[!UICONTROL ツールチップを表示]**：ボタン、メニュー、およびナビゲーション リンク上にポインタを移動したときにツールチップを表示するかどうかを決定します。 ツールチップは、画面上のユーザ インタフェース項目を記述します。
* **[!UICONTROL チェッカーボードの背景]**：画像の背後にチェッカーボードレイヤーを表示し、アルファチャネルを持つ画像の透明領域を簡単に確認できます。
* **[!UICONTROL ファイルサイズを表示]**：参照中のアセットのファイルサイズを表示します。
* **[!UICONTROL 検索に UDF を含める]**：実行するほとんどのメタデータ検索でシステムパフォーマンスを向上させるには、選択を解除（デフォルト）します。

  メタデータ検索の多くの場合に、ユーザ定義フィールドを含めることで利点がある場合は、このオプションを選択して有効にすることができます。別の方法として、ユーザー定義のフィールドを含めることで、よりダイレクトで高速な検索を実現する詳細検索を使用してください。

  詳しくは、[詳細検索の実行](searching-assets.md#conducting_an_advanced_search)を参照してください。

  [ユーザ定義フィールド](application-setup.md#user_defined_fields)も参照してください。

* **[!UICONTROL 基本検索タイプ]**：次の 2 つのオプションから選択できます。**[!UICONTROL 次を含む]** 文字列全体で指定された値を検索します。**[!UICONTROL StartsWith]** 文字列の先頭から検索し、**[!UICONTROL 次を含む]** よりも高速に結果を返します。 どちらのオプションでも、管理者によって **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL アプリケーション一般設定]** で設定されたデフォルトが上書きされます。
* **[!UICONTROL コマンドのフィードバックを表示]**：サーバーへのコマンドリクエストの表示をオンにする場合は選択し、オフにする場合は選択を解除します。
* **[!UICONTROL 書き出し時にダイアログを表示]**：書き出し時にポップアップダイアログボックスを表示する場合に選択します。 このオプションの選択を解除（オフ）した場合でも、「ジョブ」ページに移動して書き出しの結果を取得できます。

## 電子メール

* **[!UICONTROL メールオプション]**：アップロードジョブと公開ジョブが完了したときにAdobe Dynamic Media Classicからメールで通知する方法を選択します。 ジョブ完了通知は、警告またはエラーが発生した場合のみ受信することができます。
* **[!UICONTROL メールの範囲]**：会社のすべてのジョブのメールを受信するか、開始するアップロードジョブや公開ジョブに関するメールのみを受信するかを決定します。
* **[!UICONTROL メールのタイプ]**：アップロードジョブと公開ジョブが完了した際に通知を受け取るかどうかを決定します。

## 言語

* **[!UICONTROL 優先言語]**: インターフェイスに使用する言語を決定します。

## パスワード

* **[!UICONTROL 現在のパスワード]**：現在のパスワードのパスワードを入力します。
* **[!UICONTROL 新しいパスワード]**：新しい有効なパスワードを入力します。 パスワードは次の要件を満たす必要があります。
   * 長さは 8 ～ 25 文字にする必要があります。
   * 1 つ以上の小文字を含めます。
   * 1 つ以上の大文字を含めます。
   * 1 つ以上の数字を含めます。
   * 次の特殊文字を少なくとも 1 つ含めます。`# $ &: _ : { }`
* **[!UICONTROL パスワードの再入力]**：新しいパスワードを再入力して、正しく入力されていることを確認します。
* **[!UICONTROL パスワードの有効期限]**：セキュリティ対策として、パスワードの有効期限が 72 日後に切れるかどうかを決定します。 [ はい ] を選択した場合は、72 日後にパスワードを作成するように求められます。
