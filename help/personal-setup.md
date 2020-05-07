---
title: 個人設定
seo-title: 個人設定
description: 'null'
seo-description: すべてのユーザーが、ダイナミックメディアクラシックの個人設定画面で設定を変更できます。
uuid: 29cb825a-f158-4a1e-9d5f-7636ee411b6e
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 6314e7b7-5bde-4fe2-8674-e4fc525d4d1c
translation-type: tm+mt
source-git-commit: df0c2897b9fceddde648be53b23e25b13388d6b9
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 80%

---


# 個人設定 {#personal-setup}

すべてのユーザが個人設定画面の設定を変更できます。個人設定画面を開くには、設定／個人設定をクリックします。

>[!NOTE]
>
>個人設定画面には、Scene7 Publishing System で各自が持っているユーザの役割（会社の管理者、管理者、ユーザ）が表示されます。

個人設定では、参照パネルの初期設定の動作、電子メールの受信方法およびパスワードの設定を管理します。これらの設定を変更したら、必ず「保存」をクリックしてください。

## マイアカウント情報

アカウント名、氏名、ユーザ名（電子メールアドレス）および割り当てられたユーザの役割が示されます。

### デスクトップバージョン

「今すぐインストール」をクリックして、Scene7 Publishing System デスクトップバージョンをローカルハードドライブにインストールします。または、「今すぐ再インストール」をクリックして、デスクトップバージョンをインストールし直します。

## ローカルのハードドライブにプラグインをインストールするには

1. Scene7 Publishing System の個人設定ページの Web-to-Print 向け Illustrator プラグインで、「**今すぐダウンロード**」をクリックして **Illustrator Plug-in for Web-to-Print.zip** ファイルをダウンロードします。
1. この ZIP ファイルを一時フォルダーに解凍します。

   解凍されたファイルのルートに readme ファイルがあります。このファイルには、プラグインに関する追加情報が記載されています。

1. インストールされているオペレーティングシステムに対応した次のいずれかの操作を行います。

### Windows

| 実行ソフトウェア | 操作 |
|--- |--- |
| Adobe Creative Cloud 2014 の Adobe Illustrator 18 | <ul><li>解凍されたフォルダーのルートにある CC-2014 をクリックします。</li><li>使用している Adobe Illustrator の bit バージョンに応じて、win32 または win64 をクリックします。</li><li>libraries／flame をクリックし、`aflame.dll` を Adobe Illustrator の実行可能フォルダーにコピーします。For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Support Files\Contents\Windows`. </li></ul><br/>**注意&#x200B;**: 次の例は、64ビットの場所のパスです。 32ビットの場所は、プログラムファイル(x86)の下にある場合があります。<br/><ul><li>libraries フォルダーに戻り、flamingo をクリックし、`aflamingo.dll` を前の手順と同じ Adobe Illustrator 実行可能フォルダーにコピーします。 </li><li>手順 2 で選択した win32 または win64 フォルダーに戻り、`AdobeS7FXGFileFormat.aip` を Adobe Illustrator のプラグインフォルダーにコピーします。For example, `C:\Program Files\Adobe\Adobe Illustrator CC 2014\Plug-ins\Illustrator Formats`. </li></ul> <br/>**注意&#x200B;**: 次の例は、64ビットの場所のパスです。 32ビットの場所は、プログラムファイル(x86)の下にある場合があります。 |
| Adobe Creative Cloud の Adobe Illustrator 17 | <ul><li>解凍されたフォルダーのルートにある CC をクリックします。 </li><li>使用している Adobe Illustrator の bit バージョンに応じて、win32 または win64 をクリックします。</li><li> Copy `AdobeS7FXGFileFormat.aip` to Adobe Illustrator&#39;s plug-ins folder. For example, `C:\Program Files\Adobe\Adobe Illustrator CC (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**注意&#x200B;**: 次の例は、64ビットの場所のパスです。 32ビットの場所は、プログラムファイル(x86)の下にある場合があります。 |
| Adobe Creative Suite 6 の Adobe Illustrator 16 | <ul><li>解凍されたフォルダーのルートにある 6.0 をクリックします。 </li><li>使用している Adobe Illustrator の bit バージョンに応じて、win32 または win64 をクリックします。 </li><li>AdobeS7FXGFileFormat.aip を Adobe Illustrator のプラグインフォルダーにコピーします。For example, `C:\Program Files\Adobe\Adobe Illustrator CS6 (64 Bit)\Plug-ins\Illustrator Formats`.</li></ul><br/>**注意&#x200B;**: 次の例は、64ビットの場所のパスです。 32ビットの場所は、プログラムファイル(x86)の下にある場合があります。 |

### Mac

| 実行ソフトウェア | 操作 |
|--- |--- |
| Adobe Creative Cloud 2014 の Adobe Illustrator 18 | <ul><li>解凍されたフォルダーのルートにある CC-2014／mac64 をクリックします。</li><li>libraries／flame をクリックし、`aflame.framework` フォルダーを Adobe Illustrator パッケージ内容フォルダーにコピーします。For example, `/Applications/Adobe Illustrator CC 2014/ Illustrator.app/Contents/Frameworks/`. （Adobe Illustratorのパッケージ内容フォルダーを開くには、Adobe illustrator CC 2014アイコンを右クリックし、コンテキストメニューから「パッケージの内容を表示」をクリックします）。</li><li>libraries フォルダーに戻り、`flamingo` をクリックし、`aflamingo.framework` フォルダーを前の手順と同じ Adobe Illustrator パッケージ内容フォルダーにコピーします。</li><li>手順 1 で選択した mac64 フォルダーに戻り、`AdobeS7FXGFileFormat.aip` フォルダーを Adobe Illustrator のプラグインフォルダーにコピーします。For example, `/Applications/Adobe Illustrator CC 2014/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Creative Cloud の Adobe Illustrator 17 | <ul><li>解凍されたフォルダーのルートにあるCC/mac64をクリックします。</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CC/Plug-ins/Illustrator Formats/`.</li></ul><br/> |
| Adobe Creative Suite 6 の Adobe Illustrator 16 | <ul><li>解凍されたフォルダーのルートにある6.0/mac64をクリックします。</li><li>Copy the `AdobeS7FXGFileFormat.aip` folder to Adobe Illustrator’s plug-in folder. For example, `/Applications/Adobe Illustrator CS6/Plug-ins/Illustrator Formats/`.</li></ul> |

この設定により、プラグインが Adobe Illustrator で使用できるようになります。

### ブラウザ

* **サムネールサイズ**
   * 参照パネルのグリッドビューでのサムネール画像の初期設定のサイズを指定します。
* **初期設定のアセットライブラリビュー**
   * ビルドセットのアセットライブラリ内のアセットをサムネールで表示するか、名前で表示するかを指定します。アセットライブラリで大量のアセットを操作する場合は、アセットを名前順に表示できます。例えば、PDF ファイルを多く含む大規模な eCatalog を作成している場合は、アセットを名前順で表示してリストを短くすることができます。
* **初期設定表示での並べ替え順序**
   * 参照パネルでのアセットの初期設定の表示順序を指定します。メニューで並べ替え条件を選択して、昇順または降順のどちらで並べ替えるかを指定します。
* **初期設定の参照場所**
   * 参照場所として、初期設定、ブラウズされた最後のフォルダ、ナビゲートして指定した特定の場所のいずれかを設定できます。また、ファイルやフォルダを昇順または降順に並べ替えるよう参照場所を設定できます。
* **初期設定の参照ビュー**
   * 参照パネルを初めて開いたときの初期設定表示を、グリッドビューまたはリストビューのどちらにするかを指定します。
* **スプラッシュスクリーンの表示**
   * スタートアップスクリーンなどの起動画面を表示するかどうかを指定します。
* **ツールチップを表示**
   * ボタン、メニューおよびナビゲーションリンクにポインタを合わせたときにツールチップが表示されるようにするかどうかを指定します。ツールチップは、画面上の項目の説明を表示します。
* **市松模様の背景**
   * 画像の後ろに市松模様のレイヤーを表示して、アルファチャンネルを含む画像の透明部分を簡単に判別できるようにします。
* **ファイルサイズを表示**
   * ブラウズ時にアセットのファイルサイズを表示します。
* **SPS の終了時に確認する**
   * Scene7 Publishing System を終了する前に確認ウィンドウを表示します。
* **検索にユーザ定義フィールドを含める**
   * 実行する多くのメタデータ検索でシステムのパフォーマンスを向上させるために、選択されていません（デフォルト）。

メタデータ検索の多くの場合に、ユーザ定義フィールドを含めることで利点がある場合は、このオプションを選択して有効にすることができます。別の方法として、詳細検索を使用すると、ユーザ定義フィールドを含める場合よりも的を絞った高速な検索ができます。

詳しくは、[詳細検索の実行](searching-assets.md#conducting_an_advanced_search)を参照してください。

[ユーザ定義フィールド](application-setup.md#user_defined_fields)も参照してください。

* **基本検索タイプ**
   * 初期設定の検索タイプとして、「次を含む」または「次で始まる」を選択します。
* **Media Portal 機能を表示**
   * このオプションを選択すると、カートなどの Media Portal 機能にアクセスできます。
* **コマンドフィードバックを表示**
   * サーバへのコマンド要求を表示します。
* **書き出し中にダイアログを表示**
   * 書き出しの実行時にダイアログボックスを表示します。このオプションの選択を解除しても、ジョブページに移動して書き出しの結果を取得することができます。

## 電子メール

* **電子メールオプション**
   * ジョブのアップロードと公開が完了したときに、Dynamic Media Classicから電子メールで通知する方法を選択します。 ジョブ完了通知は、警告またはエラーが発生した場合のみ受信することができます。
* **電子メールの範囲**
   * 会社のすべてのジョブの電子メールを受信するか、自分が実行したアップロードおよび公開ジョブの電子メールのみを受信するかを指定します。
* **電子メールタイプ**
   * アップロードジョブと公開ジョブが完了したときに、通知を受信するかどうかを指定します。
* **言語**
* **設定言語**
   * インターフェイスの言語を指定します。
* **パスワード**
* **新しいパスワード**
   * 新しい有効なパスワードを入力します。 パスワードは、次の要件を満たしている必要があります。
      * 長さは8 ～ 25文字
      * 最低1文字の小文字を含む
      * 大文字を少なくとも1文字含む
      * 少なくとも1つの数字を含む
      * 次の特殊文字の少なくとも1つを含める： #$&amp;-_:{}
* **パスワードの再入力**
   * 新しいパスワードをもう一度入力して、正しく入力したことを確認します。
* **パスワードの有効期限**
   * セキュリティ対策として、72 日間が経過した後にパスワードを期限切れにするかどうかを指定します。「はい」を選択すると、72 日間が経過した後に新しいパスワードを指定するように求められます。
