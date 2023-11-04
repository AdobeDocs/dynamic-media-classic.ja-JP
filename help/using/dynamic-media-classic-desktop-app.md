---
title: Adobe Dynamic Media Classicデスクトップアプリケーション — 利用可能になりました
description: Adobe Dynamic Media Classicデスクトップアプリケーションの詳細。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '2035'
ht-degree: 1%

---

# 利用可能： Adobe Dynamic Media Classicデスクトップアプリケーション {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classicのユーザーは、ブラウザーのAdobeFlashテクノロジーに依存しなくなった、新しいデスクトップアプリケーションエクスペリエンスにアクセスできるようになりました。

この新しいアプリは、Windows®とmacOSで使用できます。

>[!IMPORTANT]
>
>Adobeでは、2020 年 10 月 2 日までに新しいAdobe Dynamic Media Classicデスクトップアプリケーションをインストールすることをお勧めします。 これにより、AdobeFlash Playerが 2020 年 12 月 31 日に廃止される前に、スムーズな移行が実現します。 この日以降、製品で「 Adobe Dynamic Media Classic 」というラベルが付いたAdobe Dynamic Media Classicユーザーインターフェイスのブラウザーバージョンにログオンすることはできません。

詳しくは、 FAQ( [新しいAdobe Dynamic Media Classicログインが利用できるようになりました。](/help/using/new-ui-2020.md)

## Adobe Dynamic Media Classicデスクトップアプリケーションの必要システム構成 {#system-requirements-dmc-app}

Adobe Dynamic Media Classicデスクトップアプリケーションは次のオペレーティングシステムと互換性があります。

* macOS 10.10 以降。
* Windows® 7 以降。

必要システム構成の詳細については、 [Adobe Dynamic Media Classicデスクトップアプリケーションの必要システム構成](/help/using/system-requirements.md).

Adobe Dynamic Media Classicデスクトップアプリケーション内のアップグレード通知は、 *軽微* リリース。 マイナーリリースの修正のメリットがあるお客様は、アップグレードできます。

## 最新リリース (20.22.2) のmacOSのみで修正済み {#release-feb2022}

* macOS Monterey — 以降のアップロードで、ファイルのアップロードページがフリーズする。 <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## 最新リリースの修正点 (20.22.1) {#release-jan2022}

* 画像編集 **[!UICONTROL 保存]** ボタンが機能しなかった問題を修正しました。
* セットエディターで、 **[!UICONTROL 閉じる]**, **[!UICONTROL 保存]**、および **[!UICONTROL 名前を付けて保存]** 内でアセットをスクロールした後、ボタンが無効になる **[!UICONTROL アセットを追加]** パネル。
* **[!UICONTROL 再生]** ビデオの詳細表示のボタンが機能しませんでした。
* 入力できませんでした `d` および `e` in **[!UICONTROL ユーザー名]** および **[!UICONTROL パスワード]** フィールド (macOS Monterey の実行時 )
* 残りの Analytics API をバージョン 2.0 に移動しました。

## リリース20.21.3の修正点 {#release-sept2021}

* デスクトップアプリケーションで操作が実行されなかった時間が経過した後に表示されるアセットの壊れたサムネール。
* 通常、設定操作の後、デスクトップアプリケーションが応答を停止します。
* の下での要求の難読化とロックモードの自動有効化 **[!UICONTROL 画像サービングをテスト]**.

  詳しくは、 [セキュアテストサービスのテスト](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* 認証メカニズムがAdobe Analyticsに更新されました。 新しい統合に関連している場合、または一部の Analytics 変数をDynamic Media Classicデスクトップアプリケーション内で更新する必要がある場合。

  詳しくは、 [Adobe Analyticsにログイン](/help/using/log-analytics.md) を参照してください。

## リリース20.21.2の修正点 {#minor-release}

* 20.21.1の既知の制限： **[!UICONTROL サーバー]** ログイン画面のドロップダウンリストが空でした。
* In **[!UICONTROL アップロードジョブオプション]**，レイヤー名のデフォルト値は以下にあります。 **[!UICONTROL Photoshop Options]**、現在は **[!UICONTROL Photoshopと画層名]**. PSD ファイルのレイヤーは、個別の画像としてアップロードされます。
   * 以前のデフォルトは、 **[!UICONTROL レイヤー名]**&#x200B;は、画像ファイル内のレイヤー名またはレイヤー番号にちなんでPSDに名前を付けます。 レイヤ番号は、PSDファイル内のレイヤ名が既定のPhotoshopレイヤ名である場合に使用されました。
   * の新しいデフォルト **[!UICONTROL Photoshopと画層名]**&#x200B;では、画像ファイルの後にPSDの名前を付け、その後にレイヤー名またはレイヤー番号を付けます。 PSD ファイルのレイヤー名が、初期設定の Photoshop レイヤー名の場合は、レイヤー番号が使用されます。
   * Adobe Dynamic Media Classicのレイヤー画像に一意の名前が付けられるので、既存のPSDやテンプレート ( 元のPSDファイル内の共有レイヤー名 ) の更新はおこなわれません。
* アセットの壊れたサムネール。

## リリース20.21.1の修正点 {#latest-fixes-desktop-app}

* タイムアウトによりサインインに関する問題が発生し、次のメッセージが表示されます。 *このユーザーは、権限を持たずにグループに割り当てられる場合があります。 管理者に問い合わせてください。*
* 不正なパスワードが試行されるたびに、ビューアプリセットが複製されます。
* ルートフォルダー内の多数のアセットが原因で、デスクトップアプリケーションが応答しなくなる。 (Windows®で修正。macOSで必要に応じて動作 )。

## リリース20.20.2の修正点 {#previous-version-fixes-desktop-app}

* macOSと Windows®の両方で、デスクトップアプリケーションのユーザーインターフェイスを使用してアップロードできるファイルの数に制限はありません。
* 会社を切り替えるためにデスクトップアプリケーションからサインアウトする必要はありません。
* Windows®で貼り付け操作の Ctrl + V が機能するようになりました。
* 今後、新しいバージョンのデスクトップアプリケーションがリリースされると、デスクトップアプリケーション内でユーザーに通知が送信されるようになります。

## macOSまたは Windows®での最新のAdobe Dynamic Media Classicデスクトップアプリケーションのダウンロードとインストール {#installation-dmc-app}

関連項目:

* [Macでの最新のAdobe Dynamic Media Classicデスクトップアプリケーションのダウンロードとサイレントインストール](#install-silent-mac-dmc-app)
* [Windows での最新のAdobe Dynamic Media Classicデスクトップアプリケーションのダウンロードとサイレントインストール](#install-silent-windows-dmc-app)

1. システムで古いAdobe Dynamic Media Classicデスクトップアプリケーションバージョンをアンインストールします。

1. Adobe Dynamic Media Classicデスクトップアプリケーション用の最新のインストーラーをダウンロードします。

   * 最新バージョンは、以下で入手できます。

      * [macOS (.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * 以前のバージョンは、次の場所で利用できます。

      * [macOS (.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE) - Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. ダウンロードしたインストーラーに基づいて、次のいずれかの操作を行います。

   * **macOS** - **[!UICONTROL ドラッグ&amp;ドロップしてインストール]** ダイアログボックス、ドラッグ **[!UICONTROL Adobe Dynamic Media Classic]** をクリックし、次にドロップします。 **[!UICONTROL アプリ]**.

     ![macOSでのドラッグ&amp;ドロップによるインストール](/help/using/assets/dragondrop-install1.png)

   * Adobe Analytics の **[!UICONTROL アプリ]** フォルダーで、「Adobe Dynamic Media Classic」アイコンをタップします。
   * ダイアログボックスで、をタップします。 **[!UICONTROL 開く]** をクリックして、Adobe Dynamic Media Classicデスクトップアプリケーションを開きます。

     ![ダウンロードしたアプリを開く](/help/using/assets/open-dmclassicapp1.png)

   * **Windows**  — インストーラーバイナリを実行し、画面に表示される指示に従ってデスクトップアプリケーションをインストールします。

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classicログインページが表示されます。

   ![Adobe Dynamic Media Classicサインイン](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classicデスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicにログオンするために使用したのと同じ資格情報を使用します。

   の **[!UICONTROL サーバー]** を使用するには、実稼動環境で次のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | 北米生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 実稼動（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC Production （アジア太平洋） | https://s7sps5.scene7.com/ |

1. ログイン後に、使い慣れたブラウザーユーザーインターフェイスが表示されます。 デスクトップアプリケーションでは、通常どおり、毎日のAdobe Dynamic Media Classicアクティビティを続行できます。

## ダウンロードと *無音* macOSでの最新のAdobe Dynamic Media Classicデスクトップアプリケーションのインストール {#install-silent-mac-dmc-app}

関連項目:

* [Macまたは Windows での最新のAdobe Dynamic Media Classicデスクトップアプリケーションのダウンロードとインストール](#installation-dmc-app)
* [Windows での最新のAdobe Dynamic Media Classicデスクトップアプリケーションのダウンロードとサイレントインストール](#install-silent-windows-dmc-app)

をダウンロードして *無音* macOSに最新バージョンのAdobe Dynamic Media Classicデスクトップアプリケーションをインストールします。

1. システムで古いAdobe Dynamic Media Classicデスクトップアプリケーションバージョンをアンインストールします。

1. macOS用Adobe Dynamic Media Classicデスクトップアプリケーションの最新のインストーラーをダウンロードします。

   * [macOS (.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. 次のコマンドを使用して、ダウンロードしたディスクイメージ (.DMG) をマウントポイントの場所にマウントします。

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. .APP ファイルのコピー先 **[!UICONTROL アプリ]** 次のコマンドを使用します。

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classicログインページが表示されます。

   ![Adobe Dynamic Media Classicサインイン](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classicデスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicにログオンするために使用したのと同じ資格情報を使用します。

   の **[!UICONTROL サーバー]** を使用するには、実稼動環境で次のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | 北米生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 実稼動（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC Production （アジア太平洋） | https://s7sps5.scene7.com/ |

## ダウンロードと *無音* Windows®での最新のAdobe Dynamic Media Classicデスクトップアプリケーションのインストール {#install-silent-windows-dmc-app}

使用するコマンドは、基本的な MSI サイレントインストール用です。 ただし、Adobe Dynamic Media Classicデスクトップアプリケーションインストーラーは、InstallShield を使用して作成された InstallScript MSI インストーラーです。 インストーラーをレコードモードで実行すると、ユーザーの操作が応答ファイルに記録されます。 この応答ファイルは、次に [サイレントモードでのインストールの実行](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

関連項目:

* [Macまたは Windows での最新のAdobe Dynamic Media Classicデスクトップアプリケーションのダウンロードとインストール](#installation-dmc-app)

* [macOSでの最新のAdobe Dynamic Media Classicデスクトップアプリケーションのダウンロードとサイレントインストール](#install-silent-mac-dmc-app)

をダウンロードして *無音* Windows®での最新バージョンのAdobe Dynamic Media Classicデスクトップアプリケーションのインストール：

1. システムで古いAdobe Dynamic Media Classicデスクトップアプリケーションバージョンをアンインストールします。

1. Adobe Dynamic Media Classicデスクトップアプリケーション用の最新のインストーラーをダウンロードします。

   * [Windows® (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 次のコマンドを使用して、インストーラーをレコードモードで実行します。

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. GUI インストーラウィンドウで、インストール場所などの操作/入力を記録するために、次の手順に従います。 `Setup.iss` ファイル。

1. 作成した `Setup.iss` ファイルと `adobe-dynamic-media-classic-20.22.1.exe` を他のコンピューターに送信します。

1. サイレントインストールに対して次のコマンドを実行します。

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   コマンドラインパラメータの詳細は、次の場所で確認できます。 [Setup.exe および Update.exe コマンドラインパラメーター](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classicログインページが表示されます。

   ![Adobe Dynamic Media Classicサインイン](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classicデスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicにログオンするために使用したのと同じ資格情報を使用します。

   の **[!UICONTROL サーバー]** を使用するには、実稼動環境で次のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | 北米生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 実稼動（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC Production （アジア太平洋） | https://s7sps5.scene7.com/ |

## Adobe Dynamic Media Classic Desktop App の使用に関するビデオウォークスルー {#dmc-app-video-walk-through}

所要時間： [Adobe Dynamic Media Classic Desktop App の使用に関するビデオウォークスルー](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) （長さ：2 分 36 秒）。

## デスクトップアプリケーションを使用した、コンピューター上の画像キャッシュとアセットキャッシュのクリア {#clear-cache}

1. Adobe Dynamic Media Classicデスクトップアプリケーションで、右上隅付近にあるをタップします。 **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.
1. 次の日： **[!UICONTROL 個人設定]** ページの **[!UICONTROL デスクトップ]** 見出しで、次のいずれかの操作を行います。
   * Dynamic MediaでキャッシュされたAdobeのすべての画像ファイルをコンピューターから削除するには、をタップします。 **[!UICONTROL 画像キャッシュをクリア]**&#x200B;をタップし、 **[!UICONTROL OK]**.
   * Dynamic MediaでキャッシュされたAdobeファイルをすべてコンピューターから削除するには、 **[!UICONTROL アセットキャッシュをクリア]**&#x200B;をタップし、 **[!UICONTROL OK]**.
1. ページの右下隅にあるをタップします。 **[!UICONTROL 閉じる]**.

### 画像キャッシュとアセットキャッシュの手動クリア

デスクトップアプリケーションを使用して画像とアセットのキャッシュをクリアする以外に、ファイルシステムから直接キャッシュを手動でクリアすることもできます。

1. ご使用のオペレーティングシステムに応じて、次の場所に移動します。

   * MACOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic 20.21.1の既知の制限

* The **[!UICONTROL サーバー]** Adobe Dynamic Media Classicデスクトップアプリケーション20.21.1に更新した後、ドロップダウンリストが空になる — シナリオ：Adobe Dynamic Media Classic 20.20.1または20.20.2をインストールしてログインし、アプリケーションを閉じます。 次に、Adobe Dynamic Media Classic 20.21.1に更新します。ログインを試みると、 **[!UICONTROL サーバー]** ドロップダウンリスト **[!UICONTROL アカウントにサインイン]** ダイアログボックスが空です。 この問題を回避するには、次の手順を実行する必要があります。 [キャッシュを手動でクリアする](#clear-cache) （上記の手順を参照）。

## Adobe Dynamic Media Classic 20.20.1の既知の制限 (20.20.2で修正 )

**_Windows®のみに適用 — デスクトップアプリケーションの UI からアップロードできるファイルの数に制限はありますか。_**<br>はい。デスクトップアプリケーション UI を使用して、一度に最大 150 個のファイルをアップロードできます。

**_Windows®とmacOSに適用 — 会社を切り替える方法を教えてください。_**<br>会社を切り替えるには、次の手順を実行します。

* Adobe Dynamic Media Classicアプリで、会社ドロップダウンリストから新しい会社を選択します。
* ポップアップウィンドウが表示されたら、をタップします。 **[!UICONTROL OK]** をクリックして、アプリを閉じます。

  ![新しい会社を使用するには、アプリを再起動します](/help/using/assets/dmclassic-new-company1.png)

* Adobe Dynamic Media Classicを再起動し、通常どおりにサインインして、新しい会社で作業します。

## ヒントとテクニック

**_Adobe Dynamic Media Classicのランディングページに Media Cart パネルが表示されません。_**<br>Adobe Dynamic Media Classicで、**[!UICONTROL 設定/個人設定&#x200B;]**. 「ブラウザー」セクションで、**[!UICONTROL MediaPortal 機能を表示&#x200B;]**が選択されている（オンになっている）。 タップ**[!UICONTROL 保存/閉じる&#x200B;]**.

**_アセットの公開状態（緑色のインジケーター）が正しく反映されていません。_**<br>アセットの正しい公開状態を確認するには、ブラウザーのユーザーインターフェイスで UI に再ログインする必要がありました。 デスクトップアプリケーションで、Adobeでは**[!UICONTROL 更新&#x200B;]**アイコン（右側）**[!UICONTROL なしを選択&#x200B;]**」ボタンをクリックします。 次をタップします。**[!UICONTROL 更新&#x200B;]**アイコンをクリックして、特定のページ上にあるすべてのアセットの最新ステータスを確認します。 ブラウザー UI と同様に、再ログインは不要です。

![更新アイコン](/help/using/assets/refresh-icon1.png)
*更新アイコン*

**_デスクトップアプリケーションでバッチセットプリセットが機能しない。_**<br>タップ**[!UICONTROL アップロード/ジョブオプション/バッチセットプリセット&#x200B;]**. 関連する**[!UICONTROL バッチセットプリセット&#x200B;]**が有効になっている。 クリック**[!UICONTROL アップロードを保存して送信&#x200B;]**.
