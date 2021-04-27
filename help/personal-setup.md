---
title: 個人設定
description: すべてのユーザが、Dynamic Mediaクラシックの個人設定画面で設定を変更できます。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
feature: Dynamic Mediaクラシック
role: Administrator,Business Practitioner
exl-id: a019f973-7647-466f-8af3-5312e9225e89
translation-type: tm+mt
source-git-commit: c4e2b8b42b56420269087d0d4f262490464270c0
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 28%

---

# 個人設定 {#personal-setup}

すべてのユーザが個人設定画面の設定を変更できます。個人設定画面を開くには、設定／個人設定をクリックします。

>[!NOTE]
>
>個人設定画面のリストは、Dynamic Mediaクラシックでのユーザの役割を持ちます。会社管理者、管理者またはユーザー。

個人設定では、参照パネルの初期設定の動作、電子メールの受信方法およびパスワードの設定を管理します。これらの設定を変更したら、必ず「保存」をクリックしてください。

## マイアカウント情報

アカウント名、氏名、ユーザ名（電子メールアドレス）および割り当てられたユーザの役割が示されます。

## デスクトップ

* **イメージキャッシュをクリア** -AdobeDynamic Mediaのキャッシュイメージファイルをすべてコンピュータから削除します。
* **アセットキャッシュのクリア** -AdobeDynamic Mediaがアセットファイルをコンピュータからすべて削除します。

デスクトップアプリケーションを使用して画像とアセットのキャッシュを消去する以外に、ファイルシステムから直接手動でキャッシュをクリアできます。 オペレーティングシステムに応じて、次の場所に移動します。

* macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
* Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## CREATIVE SUITE EXTENSION

**AdobeDynamic MediaCreative Suite拡張機能をインストールするには：**

1. Dynamic Mediaクラシックのツールバーで、**[!UICONTROL セットアップ]**/**[!UICONTROL 個人設定]**&#x200B;をクリックし、「Creative Suite拡張子」で、**[!UICONTROL 今すぐダウンロード]**&#x200B;をクリックして`s7csxs.zxp`ファイルをダウンロードします。
1. 拡張機能に関する詳細については、「**[!UICONTROL インストール]**」および「**[!UICONTROL 必要システム構成]**」のリンクをクリックしてください。

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

* **サムネールのサイズ**  — 参照パネルのグリッド表示に表示されるサムネール画像の初期設定のサイズを指定します。
* **初期設定のアセットライブラリ表示**  — ビルドセットのアセットライブラリ内のアセットをサムネールで表示するか、名前で表示するかを指定します。アセットライブラリで大量のアセットを操作する場合は、アセットを名前順に表示できます。例えば、PDF ファイルを多く含む大規模な eCatalog を作成している場合は、アセットを名前順で表示してリストを短くすることができます。
* **初期設定の参照並べ替え順**  — 参照パネルでのアセットの初期設定の表示順序を指定します。メニューで並べ替え条件を選択して、昇順または降順のどちらで並べ替えるかを指定します。
* **デフォルトの参照場所**  — 参照場所を、デフォルト、最後に参照したフォルダ、またはナビゲートして指定した特定の場所に設定できます。また、ファイルやフォルダを昇順または降順に並べ替えるよう参照場所を設定できます。
* **初期設定の参照表示**  — 初めて参照パネルを開いたときに表示される初期設定の表示を、グリッド表示またはリスト表示のどちらにするかを指定します。
* **スプラッシュスクリーンの表示**  — スタートアップスクリーンなどのスプラッシュスクリーンを表示するかどうかを指定します。
* **ツールヒントを表示**  — ボタン、メニュー、およびナビゲーションリンクにポインタを合わせたときにツールチップを表示するかどうかを指定します。ツールチップは、画面上のユーザインターフェイス項目を説明します。
* **市松模様の背景**  — 画像の背後に市松模様のレイヤーを表示し、アルファチャネルを持つ画像の透明部分を簡単に確認できます。
* **Show File Size**  — 参照時に、アセットのファイルサイズを表示します。
* **検索にユーザ定義フィールドを含める**  — 実行するほとんどのメタデータ検索のシステムパフォーマンスを向上させるには、選択解除（デフォルト）。

   メタデータ検索の多くの場合に、ユーザ定義フィールドを含めることで利点がある場合は、このオプションを選択して有効にすることができます。別の方法として、詳細検索を使用すると、ユーザ定義フィールドを含める場合よりも的を絞った高速な検索ができます。

   詳しくは、[詳細検索の実行](searching-assets.md#conducting_an_advanced_search)を参照してください。

   [ユーザ定義フィールド](application-setup.md#user_defined_fields)も参照してください。

* **基本検索タイプ**  — 次の2つのオプションから選択できます。 **** コンテナは、指定した値の文字列全体を検索します。 **[!UICONTROL StartsWith]** 文字列の先頭から検索し、 **[!UICONTROL Containsよりも早く結果を返し]**&#x200B;ます。どちらのオプションも、管理者が&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL アプリケーションの全般設定]**&#x200B;で設定したデフォルトより優先されます。
* **Show Command Feedback**  — サーバに対するコマンド要求の表示をオンにする場合に選択します。オフにする場合は、選択を解除します。
* **書き出し中にダイアログを表示**  — 書き出し中にポップアップダイアログボックスを表示する場合に選択します。このオプションの選択を解除（オフに）しても、ジョブページに移動して、書き出しの結果を取得できます。

## 電子メール

* **電子メールオプション**  — ジョブのアップロードと公開が完了したときに、Dynamic Mediaクラシックに電子メールで通知する方法を選択します。ジョブ完了通知は、警告またはエラーが発生した場合のみ受信することができます。
* **電子メールの範囲**  — 自分の会社のすべてのジョブの電子メールを受信するか、自分が開始したアップロードおよび公開ジョブに関する電子メールのみを受信するかを指定します。
* **電子メールの種類**  — アップロードジョブと公開ジョブが完了したときに通知を受けるかどうかを指定します。

## 言語

* **優先言語**  — インターフェイスで使用する言語を決定します。

## パスワード

* **現在のパスワード**  — 現在のパスワードを入力します。
* **新しいパスワード**  — 新しい有効なパスワードを入力します。パスワードは、次の要件を満たしている必要があります。
   * 長さは8 ～ 25文字です。
   * 少なくとも1文字の小文字を含むこと。
   * 大文字を少なくとも1文字含むこと。
   * 少なくとも1つの数字を含むこと。
   * 次の特殊文字の少なくとも1つを含める：`# $ & - _ : { }`
* **パスワードの再入力**  — 新しいパスワードを再入力し、正しく入力されていることを確認します。
* **パスワードの有効期限**  — セキュリティ対策として、72日間が経過した後にパスワードの有効期限が切れるかどうかを指定します。「はい」を選択すると、72 日間が経過した後にパスワードを指定するように求められます。
