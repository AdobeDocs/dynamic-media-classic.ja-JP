---
title: 個人設定
description: すべてのユーザーが、Dynamic Media Classicの個人設定画面で設定を変更できます。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Media Classic
role: Admin,User
exl-id: a019f973-7647-466f-8af3-5312e9225e89
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 28%

---

# 個人設定 {#personal-setup}

すべてのユーザが個人設定画面の設定を変更できます。個人設定画面を開くには、設定／個人設定をクリックします。

>[!NOTE]
>
>個人設定画面には、Dynamic Media Classicでのユーザーの役割が一覧表示されます。会社管理者、管理者、またはユーザー。

個人設定では、参照パネルの初期設定の動作、電子メールの受信方法およびパスワードの設定を管理します。これらの設定を変更したら、必ず「保存」をクリックしてください。

## マイアカウント情報

アカウント名、氏名、ユーザ名（電子メールアドレス）および割り当てられたユーザの役割が示されます。

## デスクトップ

* **画像キャッシュをクリア**  - Dynamic MediaでキャッシュされたAdobeファイルをすべてコンピューターから削除します。
* **アセットキャッシュをクリア**  - Dynamic MediaがAdobeー内のアセットファイルをすべて削除します。

デスクトップアプリケーションを使用して画像とアセットのキャッシュをクリアする以外に、ファイルシステムから直接キャッシュを手動でクリアできます。 ご使用のオペレーティングシステムに応じて、次の場所に移動します。

* macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## CREATIVE SUITE EXTENSION

**Dynamic MediaAdobe拡張機能をインストールするには：**

1. Dynamic Media Classicのツールバーで、**[!UICONTROL Setup]** / **[!UICONTROL Personal Setup]**&#x200B;をクリックし、「Creative Suite拡張機能」で、「**[!UICONTROL Download Now]**」をクリックして`s7csxs.zxp`ファイルをダウンロードします。
1. 拡張機能に関する追加情報については、「**[!UICONTROL インストール]** 」と「**[!UICONTROL 必要システム構成]** 」のリンクをクリックします。

<!--    A readme file is included at the root of the unzipped file to provide you with additional information about the extension.

1. Depending on your installed operating system, do one of the following: -->

<!-- #### Windows

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014.</li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li>Click libraries > flame, and then copy `aflame.dll` to Adobe Illustrator's executable folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead. <br/><ul><li>Return to the same libraries folder, click flamingo, and then copy `aflamingo.dll` to the same Adobe Illustrator executable folder that you used in the previous step. </li><li>Return to the win32 or win64 folder that you selected in step 2, and then copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64.</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0. </li><li>Depending on the bit version of Adobe Illustrator that you are using, click win32 or win64. </li><li>Copy AdobeS7FXGFileFormat.aip to Adobe Illustrator's plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**Note**: This example path is for the 64-bit location; the 32-bit location may fall under Program Files (x86) instead.|

#### Mac

|If you are running|Do this|
|--- |--- |
|Adobe Illustrator 18 in Adobe Creative Cloud 2014|<ul><li>From the root of the unzipped folder, click CC-2014 > mac64.</li><li>Click libraries > flame, and then copy the `aflame.framework` folder to Adobe Illustrator package contents folder. For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. (To open Adobe Illustrator’s package contents folder, right-click on the Adobe illustrator CC 2014 icon and click Show Package Contents from context menu).</li><li>Return to the same libraries folder, click `flamingo`, and then copy the `aflamingo.framework` folder to the same Adobe Illustrator package contents folder that you used in the previous step.</li><li>Return to the mac64 folder that you selected in step 1, and then copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 17 in Adobe Creative Cloud|<ul><li>From the root of the unzipped folder, click CC > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/>|
|Adobe Illustrator 16 in Adobe Creative Suite 6|<ul><li>From the root of the unzipped folder, click 6.0 > mac64</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul>|

The plug-in is now available for you to use in Adobe Illustrator. -->

## ブラウザ

* **サムネールのサイズ**  — 参照パネルのグリッドビューでのサムネール画像のデフォルトサイズを決定します。
* **デフォルトのアセットライブラリ表示**  — ビルドセットのアセットライブラリ内のアセットをサムネールとして表示するか、名前で表示するかを指定します。アセットライブラリで大量のアセットを操作する場合は、アセットを名前順に表示できます。例えば、PDF ファイルを多く含む大規模な eCatalog を作成している場合は、アセットを名前順で表示してリストを短くすることができます。
* **デフォルトの参照の並べ替え順**  — 参照パネルにデフォルトで表示されるアセットの順序を決定します。メニューで並べ替え条件を選択して、昇順または降順のどちらで並べ替えるかを指定します。
* **デフォルトの参照場所**  — 参照場所を、デフォルト、最後に参照したフォルダー、または移動して指定した特定の場所に設定できます。また、ファイルやフォルダを昇順または降順に並べ替えるよう参照場所を設定できます。
* **デフォルトの参照表示**  — 参照パネルを初めて開いたときに表示されるデフォルトの表示を、グリッド表示とリスト表示のどちらにするかを指定します。
* **スプラッシュスクリーンの表示**  — ようこそスプラッシュスクリーンを含むスプラッシュスクリーンを表示するかどうかを指定します。
* **ツールヒントを表示**  — ボタン、メニュー、ナビゲーションリンクの上にポインターを移動したときに、ツールチップを表示するかどうかを指定します。画面上のユーザインターフェイス項目を説明するツールチップ。
* **市松模様の背景**  — 画像の背後に市松模様のレイヤーを表示し、アルファチャンネルを持つ画像の透明部分を簡単に確認できます。
* **ファイルサイズを表示**  — 参照時にアセットのファイルサイズを表示します。
* **検索にUDFを含める**  — 実行するほとんどのメタデータ検索のシステムパフォーマンスを向上させるために、選択を解除（デフォルト）。

   メタデータ検索の多くの場合に、ユーザ定義フィールドを含めることで利点がある場合は、このオプションを選択して有効にすることができます。別の方法として、詳細検索を使用すると、ユーザ定義フィールドを含める場合よりも的を絞った高速な検索ができます。

   詳しくは、[詳細検索の実行](searching-assets.md#conducting_an_advanced_search)を参照してください。

   [ユーザ定義フィールド](application-setup.md#user_defined_fields)も参照してください。

* **基本検索タイプ**  — 次の2つのオプションから選択できます。 **** コンテナは、指定した値の文字列全体を検索します。 **** StartsWithsは、文字列の先頭から検索し、「次を含む」よりも速く結果を **[!UICONTROL 返します]**。どちらのオプションも、管理者が&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL アプリケーションの一般設定]**&#x200B;で設定したデフォルトよりも優先されます。
* **Show Command Feedback**  — サーバーに対するコマンド要求の表示をオンにする場合に選択します。選択を解除してオフにします。
* **書き出し中にダイアログを表示**  — 書き出し中にポップアップダイアログボックスを表示する場合に選択します。このオプションの選択を解除（オフ）しても、ジョブページに移動して、エクスポートの結果を取得できます。

## 電子メール

* **電子メールオプション**  — アップロードジョブと公開ジョブが完了したときに、Dynamic Media Classicから電子メールで通知する方法を選択します。ジョブ完了通知は、警告またはエラーが発生した場合のみ受信することができます。
* **電子メールの範囲**  — 会社のすべてのジョブ電子メールを受信するか、開始したアップロードジョブと公開ジョブに関する電子メールのみを受信するかを指定します。
* **電子メールタイプ**  — アップロードジョブと公開ジョブが完了したときに通知を受けるかどうかを指定します。

## 言語

* **優先言語**  — インターフェイスで使用する言語を決定します。

## パスワード

* **現在のパスワード**  — 現在のパスワードを入力します。
* **新しいパスワード**  — 新しい有効なパスワードを入力します。パスワードは次の要件を満たす必要があります。
   * 長さは8～25文字です。
   * 少なくとも1文字の小文字を含める。
   * 少なくとも1文字の大文字を含める。
   * 少なくとも1つの数字を含む。
   * 次の特殊文字を少なくとも1つ含める：`# $ & - _ : { }`
* **パスワードの再入力**  — 新しいパスワードを再入力し、正しく入力していることを確認します。
* **パスワードの有効期限**  — セキュリティ対策として、パスワードの有効期限が72日後に切れるかどうかを指定します。「はい」を選択すると、72 日間が経過した後にパスワードを指定するように求められます。
