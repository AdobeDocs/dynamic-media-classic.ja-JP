---
title: 個人設定
description: すべてのユーザーが、Adobe Dynamic Media Classicの個人設定画面で設定を変更できます。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
topic: Administration, Collaboration
level: Intermediate
source-git-commit: 5d8b7cb8b4616a998346675d7324b568634698fb
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 25%

---

# 個人設定 {#personal-setup}

すべてのユーザが個人設定画面の設定を変更できます。個人設定画面を開くには、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.

>[!NOTE]
>
>個人設定画面には、Adobe Dynamic Media Classicでのユーザーの役割が一覧表示されます。会社管理者、管理者、またはユーザー。

個人設定では、参照パネルの初期設定の動作、電子メールの受信方法およびパスワードの設定を管理します。必ず選択してください **[!UICONTROL 保存]** 設定を変更した後。

## マイアカウント情報

アカウント名、氏名、ユーザ名（電子メールアドレス）および割り当てられたユーザの役割が示されます。

## デスクトップ

* **画像キャッシュをクリア** - Dynamic MediaがキャッシュしたAdobeファイルをすべてコンピューターから削除します。
* **アセットキャッシュをクリア**  — コンピューターからすべてのAdobeDynamic Mediaキャッシュアセットファイルを削除します。

デスクトップアプリケーションを使用して画像とアセットのキャッシュをクリアする以外に、ファイルシステムから直接キャッシュを手動でクリアすることもできます。 ご使用のオペレーティングシステムに応じて、次の場所に移動します。

* macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## CREATIVE SUITE EXTENSION

**AdobeDynamic MediaCreative Suite拡張機能をインストールするには：**

1. Adobe Dynamic Media Classicのツールバーで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**、「Creative Suite拡張」で、「 **[!UICONTROL 今すぐダウンロード]** をダウンロードするには `s7csxs.zxp` ファイル。
1. を選択します。 **[!UICONTROL インストール]** および **[!UICONTROL 必要システム構成]** リンクを参照してください。

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
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, select CC-2014 > mac64.</li><li>Select libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-select on the Adobe illustrator CC 2014 icon and select Show Package Contents from context menu).</li><li>Return to the same libraries folder, select `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, select CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, select 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## ブラウザ

* **[!UICONTROL サムネールサイズ]**  — 参照パネルのグリッド表示でのサムネール画像のデフォルトサイズを決定します。
* **[!UICONTROL 初期設定のアセットライブラリビュー]**  — ビルドセットのアセットライブラリ内のアセットをサムネールとして表示するか、名前で表示するかを指定します。 アセットライブラリで大量のアセットを操作する場合は、アセットを名前順に表示できます。例えば、PDF ファイルを多く含む大規模な eCatalog を作成している場合は、アセットを名前順で表示してリストを短くすることができます。
* **[!UICONTROL 初期設定の参照の並べ替え順]**  — 参照パネルでのアセットのデフォルトの表示順を決定します。 メニューで並べ替え条件を選択して、昇順または降順のどちらで並べ替えるかを指定します。
* **[!UICONTROL デフォルトの参照場所]**  — 参照場所を、デフォルト、最後に参照したフォルダー、または移動して指定した特定の場所に設定できます。 また、ファイルやフォルダを昇順または降順に並べ替えるよう参照場所を設定できます。
* **[!UICONTROL デフォルトの参照ビュー]** - [ 参照 ] パネルを最初に開いたときに表示される既定のビューは、[ グリッド表示 ] と [ リスト表示 ] のどちらかです。
* **[!UICONTROL スプラッシュスクリーンの表示]**  — ようこそスプラッシュ画面を含むスプラッシュ画面を表示するかどうかを指定します。
* **[!UICONTROL ツールチップを表示]**  — ボタン、メニュー、ナビゲーションリンクの上にポインタを移動したときにツールチップを表示するかどうかを指定します。 ツールチップは、画面上のユーザインタフェース項目を説明します。
* **[!UICONTROL 市松模様の背景]**  — 画像の背後に市松模様のレイヤーを表示し、アルファチャンネルを持つ画像の透明部分を簡単に確認できます。
* **[!UICONTROL ファイルサイズを表示]**  — 参照時にアセットのファイルサイズを表示します。
* **[!UICONTROL 検索に UDF を含める]**  — 実行するほとんどのメタデータ検索のシステムパフォーマンスを向上させるには、選択を解除します（デフォルト）。

  メタデータ検索の多くの場合に、ユーザ定義フィールドを含めることで利点がある場合は、このオプションを選択して有効にすることができます。別の方法として、詳細検索を使用すると、ユーザ定義フィールドを含める場合よりも的を絞った高速な検索ができます。

  詳しくは、[詳細検索の実行](searching-assets.md#conducting_an_advanced_search)を参照してください。

  [ユーザ定義フィールド](application-setup.md#user_defined_fields)も参照してください。

* **[!UICONTROL 基本検索タイプ]**  — 次の 2 つのオプションから選択できます。 **[!UICONTROL 次を含む]** 指定した値の文字列全体を検索します。 **[!UICONTROL StartsWith]** 文字列の先頭から検索し、より早く結果を返す **[!UICONTROL 次を含む]**. どちらのオプションでも、 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL アプリケーションの一般設定]** 管理者から。
* **[!UICONTROL コマンドフィードバックを表示]**  — サーバーに対するコマンド要求の表示を有効にする場合に選択します。オフにするには、選択を解除します。
* **[!UICONTROL 書き出し中にダイアログを表示]**  — エクスポート中にポップアップダイアログボックスを表示する場合に選択します。 このオプションの選択を解除（オフ）した場合でも、ジョブページに移動して、エクスポートの結果を取得できます。

## 電子メール

* **[!UICONTROL メールオプション]**  — アップロードジョブと公開ジョブが完了したときにAdobe Dynamic Media Classicから電子メールで通知する方法を選択します。 ジョブ完了通知は、警告またはエラーが発生した場合のみ受信することができます。
* **[!UICONTROL メール範囲]**  — 会社のすべてのジョブの電子メールを受け取るか、開始したアップロードジョブと公開ジョブに関する電子メールのみを受け取るかを決定します。
* **[!UICONTROL E メールタイプ]**  — アップロードジョブと公開ジョブが完了したときに通知を受けるかどうかを指定します。

## 言語

* **[!UICONTROL 優先言語]**  — インターフェイスで使用する言語を決定します。

## パスワード

* **[!UICONTROL 現在のパスワード]**  — 現在のパスワードを入力します。
* **[!UICONTROL 新しいパスワード]**  — 新しい有効なパスワードを入力します。 パスワードは次の要件を満たす必要があります。
   * 8 ～ 25 文字の長さにする必要があります。
   * 少なくとも 1 つの小文字を含める。
   * 大文字を少なくとも 1 文字含める。
   * 少なくとも 1 つの数字を含める。
   * 次の特殊文字を少なくとも 1 つ含める。 `# $ & - _ : { }`
* **[!UICONTROL パスワードの再入力]**  — 新しいパスワードを再入力し、正しく入力していることを確認します。
* **[!UICONTROL パスワードの有効期限]**  — セキュリティ対策として、パスワードの有効期限が 72 日後に切れるかどうかを指定します。 「はい」を選択すると、72 日間が経過した後にパスワードを指定するように求められます。
