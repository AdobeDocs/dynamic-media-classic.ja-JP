---
title: Adobe Dynamic Media Classic デスクトップ
description: 現在利用可能なAdobe Dynamic Media Classic デスクトップアプリケーションについて詳しく説明します。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
autotag-review: '2026-05-13T19:46:24.807Z'
TQID: 'https://experienceleague.adobe.com/w-jPQYG7xGeBmC8fOzcPzi6ZZ-urf0C0-HoDKVbjCWk'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 2135
ht-degree: 1%

---

# 現在利用可能：Adobe Dynamic Media Classic デスクトップアプリ {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic ユーザーは、ブラウザーのAdobe Flash テクノロジに依存しなくなった新しいデスクトップアプリエクスペリエンスにアクセスできるようになりました。

この新しいアプリは、Windows®およびmacOSで使用できるようになりました。

>[!IMPORTANT]
>
>Adobeでは、2020年10月1日までに新しいAdobe Dynamic Media Classic デスクトップアプリケーションをインストールすることをお勧めします。 これにより、2020年12月31日にAdobe Flash Playerが非推奨になる前に、スムーズに移行できるようになります。 その日付以降は、製品内で「Adobe Dynamic Media Classic」というラベルが付いたAdobe Dynamic Media Classic ユーザーインターフェイスのブラウザーバージョンにログオンできません。

[新しいAdobe Dynamic Media Classic ログインに関するFAQを参照してください。](/help/using/new-ui-2020.md)

## Adobe Dynamic Media Classic デスクトップアプリの必要システム構成 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic デスクトップアプリケーションは、次のオペレーティングシステムと互換性があります。

* macOS 10.10以降。
* Windows® 7以降。

完全な必要システム構成については、[Adobe Dynamic Media Classic デスクトップアプリの必要システム構成](/help/using/system-requirements.md)を参照してください。

Adobe Dynamic Media Classic デスクトップアプリケーション内のアップグレード通知は、*マイナー* リリースでは生成されません。 マイナーリリースの修正のメリットを受けるお客様は、アップグレードできます。

## 最新リリース（20.22.2）のmacOSでのみ修正 {#release-feb2022}

* macOS モントレー：その後のアップロードでファイルのアップロードページがフリーズする。<!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## 最新リリース（20.22.1）の修正 {#release-jan2022}

* 画像を編集する際、**[!UICONTROL 保存]** ボタンは機能しませんでした。
* **[!UICONTROL Assetsを追加]** パネルでアセットをスクロールすると、「**[!UICONTROL 閉じる]**」、「**[!UICONTROL 保存]**」、「**[!UICONTROL 別名で保存]**」ボタンが無効になります。
* ビデオの詳細ビューの&#x200B;**[!UICONTROL 再生]** ボタンが機能しませんでした。
* MacOS Montereyの実行中に、**[!UICONTROL ユーザー名]**&#x200B;および&#x200B;**[!UICONTROL パスワード]** フィールドに`d`および`e`を入力できませんでした。
* 残りのAnalytics APIをバージョン 2.0に移動しました。

## リリース 20.21.3の修正 {#release-sept2021}

* デスクトップアプリで非アクティブな状態が続いた後に表示されたアセットのサムネールが破損している。
* デスクトップアプリケーションは、通常、Set操作の後に応答を停止します。
* リクエストの難読化とロックモードは、**[!UICONTROL 画像サービングのテスト]**&#x200B;で自動的に有効になります。

  「[ セキュアテストサービス ](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service)」を参照してください。

* Adobe Analyticsで認証メカニズムを更新しました。 新しい統合の場合や、一部のAnalytics変数をDynamic Media Classic デスクトップアプリ内から更新する必要がある場合に関連します。

  更新された手順については、[Adobe Analyticsにログオン ](/help/using/log-analytics.md)してください。

## リリース 20.21.2の修正 {#minor-release}

* 20.21.1の既知の制限：サインイン画面の&#x200B;**[!UICONTROL サーバー]** ドロップダウンリストが空でした。
* **[!UICONTROL アップロードジョブオプション]**&#x200B;では、**[!UICONTROL Photoshopオプション]**&#x200B;の下のデフォルトのレイヤー名値は、**[!UICONTROL Photoshopとレイヤー名]**&#x200B;になりました。 PSD ファイルのレイヤーは、個別の画像としてアップロードされます。
   * 以前のデフォルトの&#x200B;**[!UICONTROL レイヤー名]**。PSD ファイルのレイヤー名またはレイヤー番号の後に画像の名前が付けられます。 PSD ファイル内のレイヤー名がデフォルトのPhotoshop レイヤー名である場合は、レイヤー番号が使用されました。
   * 新しいデフォルトの&#x200B;**[!UICONTROL Photoshopとレイヤー名]**&#x200B;では、PSD ファイルの後にレイヤー名またはレイヤー番号が続きます。 PSD ファイルのレイヤー名が、初期設定の Photoshop レイヤー名の場合は、レイヤー番号が使用されます。
   * Adobe Dynamic Media Classicのレイヤー画像に一意の名前が付いていることを考えると、既存のPSDやテンプレート（元のPSD ファイル内の共有レイヤー名）は更新されません。
* 壊れたアセットのサムネール。

## リリース 20.21.1の修正 {#latest-fixes-desktop-app}

* タイムアウトが原因でログインに問題が発生し、次のメッセージが表示されます：*このユーザーは許可なくグループまたはグループに割り当てられる場合があります。 管理者にお問い合わせください。*
* ビューアプリセットは、誤ったパスワード試行ごとに複製されます。
* ルートフォルダー内のアセットが多いため、デスクトップアプリケーションが応答しなくなります。 （Windowsで修正®、macOSで必要に応じて動作）

## リリース 20.20.2の修正 {#previous-version-fixes-desktop-app}

* MacOSとWindows®の両方のデスクトップアプリのユーザーインターフェイスからアップロードできるファイルの数に制限はありません。
* 会社を切り替えるためにデスクトップアプリからログアウトする必要はありません。
* Windows®で、貼り付け操作のCtrl+Vが機能するようになりました。
* 将来的には、デスクトップアプリの新しいバージョンがリリースされると、デスクトップアプリ自体にユーザーに通知が送信されます。

## MacOSまたはWindowsに最新のAdobe Dynamic Media Classic デスクトップアプリケーションをダウンロードしてインストールする® {#installation-dmc-app}

こちらもご覧ください：

* [最新のAdobe Dynamic Media Classic デスクトップアプリをMacにダウンロードしてサイレントインストールする](#install-silent-mac-dmc-app)
* [Windowsに最新のAdobe Dynamic Media Classic デスクトップアプリをダウンロードしてサイレントインストールする®](#install-silent-windows-dmc-app)

1. 古いバージョンのAdobe Dynamic Media Classic デスクトップアプリをシステムからアンインストールします。

1. Adobe Dynamic Media Classic デスクトップアプリの最新のインストーラーをダウンロードします。

   * 最新バージョンは次の場所で入手できます。

      * [macOS （.DMG）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows （.EXE）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * 以前のバージョンは、次の場所で利用できます。

      * [macOS （.DMG）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® （.EXE）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--
         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) 
-->

<!--
        * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) 
-->

<!--
    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
    * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) 
-->


1. ダウンロードしたインストーラーに基づいて、次のいずれかの操作を行います。

   * **macOS** - **[!UICONTROL ドラッグ&amp;ドロップでインストール]** ダイアログボックスを開き、**[!UICONTROL Adobe Dynamic Media Classic]**&#x200B;をドラッグして&#x200B;**[!UICONTROL アプリケーション]**&#x200B;にドロップします。

     ![macOSでのドラッグ&amp;ドロップのインストール ](/help/using/assets/dragondrop-install1.png)

   * **[!UICONTROL アプリケーション]** フォルダーで、Adobe Dynamic Media Classic アイコンをタップします。
   * ダイアログボックスで「**[!UICONTROL 開く]**」をタップして、Adobe Dynamic Media Classic デスクトップアプリを開きます。

     ![ ダウンロードしたアプリを開く](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - インストーラーバイナリを実行し、画面の指示に従ってデスクトップアプリをインストールします。

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic サインインページが表示されます。

   ![Adobe Dynamic Media Classic ログイン ](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリにログインするには、ブラウザーでAdobe Dynamic Media Classicにログオンするときに使用したのと同じ資格情報を使用します。

   **[!UICONTROL サーバー]**&#x200B;が使用する場合は、実稼動環境の次のマッピングを参照してください。

   | サーバ | ブラウザーURL |
   | --- | --- |
   | NA Production （北米） | https://s7sps1.scene7.com/ |
   | EMEA生産（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC生産（アジア太平洋） | https://s7sps5.scene7.com/ |

1. ログイン後、使い慣れたブラウザーユーザーインターフェイスのエクスペリエンスに注意してください。 デスクトップアプリでは、通常どおりAdobe Dynamic Media Classicの日常業務を続けることができます。

## 最新のAdobe Dynamic Media Classic デスクトップアプリをmacOSにダウンロードして&#x200B;*サイレント* インストールする {#install-silent-mac-dmc-app}

こちらもご覧ください：

* [MacまたはWindowsに最新のAdobe Dynamic Media Classic デスクトップアプリケーションをダウンロードしてインストールする®](#installation-dmc-app)
* [Windowsに最新のAdobe Dynamic Media Classic デスクトップアプリをダウンロードしてサイレントインストールする®](#install-silent-windows-dmc-app)

MacOSに最新バージョンのAdobe Dynamic Media Classic デスクトップアプリをダウンロードして&#x200B;*サイレント* インストールするには：

1. 古いバージョンのAdobe Dynamic Media Classic デスクトップアプリをシステムからアンインストールします。

1. MacOS用Adobe Dynamic Media Classic デスクトップアプリの最新のインストーラーをダウンロードします。

   * [macOS （.DMG）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. 次のコマンドを使用して、ダウンロードしたディスクイメージ（.DMG）をマウントします。

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. 次のコマンドを使用して、.APP ファイルを&#x200B;**[!UICONTROL アプリケーション]**&#x200B;にコピーします。

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic サインインページが表示されます。

   ![Adobe Dynamic Media Classic ログイン ](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリにログインするには、ブラウザーでAdobe Dynamic Media Classicにログオンするときに使用したのと同じ資格情報を使用します。

   **[!UICONTROL サーバー]**&#x200B;が使用する場合は、実稼動環境の次のマッピングを参照してください。

   | サーバ | ブラウザーURL |
   | --- | --- |
   | NA Production （北米） | https://s7sps1.scene7.com/ |
   | EMEA生産（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC生産（アジア太平洋） | https://s7sps5.scene7.com/ |

## Windowsに最新のAdobe Dynamic Media Classic デスクトップアプリをダウンロードして&#x200B;*サイレント* インストール® {#install-silent-windows-dmc-app}

使用するコマンドは、基本的なMSI サイレント インストール用です。 ただし、Adobe Dynamic Media Classic デスクトップアプリインストーラーは、InstallShieldを使用して作成されたInstallScript MSI インストーラーです。 インストーラーをレコードモードで実行すると、ユーザーとのやり取りは応答ファイルに記録されます。 この応答ファイルは、[ サイレントモードでのインストールの実行](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm)で説明されているように、サイレントインストールに使用されます。

こちらもご覧ください：

* [MacまたはWindowsに最新のAdobe Dynamic Media Classic デスクトップアプリケーションをダウンロードしてインストールする®](#installation-dmc-app)

* [最新のAdobe Dynamic Media Classic デスクトップアプリをmacOSにダウンロードしてサイレントインストールする](#install-silent-mac-dmc-app)

Windows®に最新バージョンのAdobe Dynamic Media Classic デスクトップアプリをダウンロードして&#x200B;*サイレント* インストールするには：

1. 古いバージョンのAdobe Dynamic Media Classic デスクトップアプリをシステムからアンインストールします。

1. Adobe Dynamic Media Classic デスクトップアプリの最新のインストーラーをダウンロードします。

   * [Windows® （.EXE）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 次のコマンドを使用して、インストーラーをレコードモードで実行します。

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. GUI インストーラーウィンドウで、インストールの手順に従って、インストール場所などのインタラクション/入力が`Setup.iss` ファイルに記録されるようにします。

1. 作成した`Setup.iss` ファイルと`adobe-dynamic-media-classic-20.22.1.exe`を他のコンピューターにコピーします。

1. サイレントインストールの場合は、次のコマンドを実行します。

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   コマンドラインパラメーターの詳細については、[Setup.exeおよびUpdate.exe コマンドラインパラメーター](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters)を参照してください。

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic サインインページが表示されます。

   ![Adobe Dynamic Media Classic ログイン ](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリにログインするには、ブラウザーでAdobe Dynamic Media Classicにログオンするときに使用したのと同じ資格情報を使用します。

   **[!UICONTROL サーバー]**&#x200B;が使用する場合は、実稼動環境の次のマッピングを参照してください。

   | サーバ | ブラウザーURL |
   | --- | --- |
   | NA Production （北米） | https://s7sps1.scene7.com/ |
   | EMEA生産（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC生産（アジア太平洋） | https://s7sps5.scene7.com/ |

## Adobe Dynamic Media Classic デスクトップアプリの使用に関するビデオチュートリアル {#dmc-app-video-walk-through}

Adobe Dynamic Media Classic デスクトップアプリ ](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media)の使用に関する[ ビデオのチュートリアルを視聴します（所要時間：2分36秒）。

## デスクトップアプリを使用して、コンピューター上の画像キャッシュとアセットキャッシュを消去する {#clear-cache}

1. Adobe Dynamic Media Classic デスクトップアプリの右上隅付近で、**[!UICONTROL 設定]**/**[!UICONTROL 個人設定]**&#x200B;をタップします。
1. **[!UICONTROL 個人設定]** ページの&#x200B;**[!UICONTROL デスクトップ]**&#x200B;見出しの下で、次のいずれかの操作を行います。
   * コンピューターからAdobe Dynamic Media キャッシュ済みのすべての画像ファイルを削除するには、**[!UICONTROL 画像キャッシュをクリア]**&#x200B;をタップしてから、**[!UICONTROL OK]**&#x200B;をタップします。
   * Adobe Dynamic Mediaにキャッシュされたすべてのアセットファイルをコンピューターから削除するには、**[!UICONTROL アセットキャッシュをクリア]**&#x200B;をタップしてから、**[!UICONTROL OK]**&#x200B;をタップします。
1. ページの右下隅にある「**[!UICONTROL 閉じる]**」をタップします。

### 画像キャッシュとアセットキャッシュを手動でクリアする

デスクトップアプリを使用して画像とアセットキャッシュをクリアするだけでなく、ファイルシステムから直接キャッシュを手動でクリアできます。

1. オペレーティングシステムに応じて、次の場所に移動します。

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic 20.21.1の既知の制限事項

* Adobe Dynamic Media Classic デスクトップアプリケーション 20.21.1にアップデートした後、**[!UICONTROL Server]** ドロップダウンリストが空になります。シナリオ：Adobe Dynamic Media Classic 20.20.1または20.20.2をインストールしてログインし、アプリケーションを閉じます。 次に、Adobe Dynamic Media Classic 20.21.1に更新します。 ログインしようとすると、**[!UICONTROL アカウントへのログイン]** ダイアログボックスの&#x200B;**[!UICONTROL サーバー]** ドロップダウンリストが空になります。 この問題を回避するには、[手動でキャッシュをクリアする必要があります](#clear-cache) （上記の手順を参照）。

## Adobe Dynamic Media Classic 20.20.1の既知の制限事項（20.20.2で修正）

**_Windows®にのみ適用 – デスクトップアプリ UIを使用してアップロードできるファイルの数に制限がありますか？_**<br>はい。デスクトップアプリ UIを使用して、一度に最大150個のファイルをアップロードできます。

**_Windows®およびmacOSに適用されます。企業間で切り替えるにはどうすればよいですか？_**<br>企業間で切り替えるには、次の操作を行います。

* Adobe Dynamic Media Classic アプリで、会社ドロップダウンリストから新しい会社を選択します。
* ポップアップウィンドウが表示されたら、**[!UICONTROL OK]**&#x200B;をタップしてログアウトし、アプリを閉じます。

  ![新しい会社を使用するには、アプリを再起動してください](/help/using/assets/dmclassic-new-company1.png)

* Adobe Dynamic Media Classicを再起動し、通常どおりログインして新しい会社で作業します。

## ヒントとテクニック

**_Adobe Dynamic Media ClassicのランディングページにMedia Cart パネルが表示されません。_**<br>Adobe Dynamic Media Classicで、**[!UICONTROL 設定/個人設定&#x200B;]**をタップします。 「ブラウザー」セクションで、「**[!UICONTROL MediaPortal機能を表示&#x200B;]**」が選択されていることを確認します（オン）。**[!UICONTROL 保存/閉じる&#x200B;]**をタップします。

**_アセットの公開状態（緑色のインジケーター）が正しく反映されない。_**<br>ブラウザーのユーザーインターフェイスでは、以前はUIに再ログインして、アセットの正しい公開状態を確認する必要がありました。 デスクトップアプリで、Adobeのツールバーに**[!UICONTROL 更新&#x200B;]**アイコンが導入されました。「**[!UICONTROL なし選択&#x200B;]**」ボタンの右側にあります。**[!UICONTROL リフレッシャー&#x200B;]**アイコンをタップすると、特定のページのすべてのアセットの最新のステータスが表示されます。 ブラウザーUIと同様に、再ログオンは必要ありません。

![更新アイコン](/help/using/assets/refresh-icon1.png)
*更新アイコン*

**_デスクトップアプリでバッチセットプリセットが機能しません。_**<br>アップロード/ジョブオプション/バッチセットプリセット]**をタップします。**[!UICONTROL 関連する**[!UICONTROL バッチセットプリセット&#x200B;]**が有効になっていることを確認します。 「**[!UICONTROL 保存してアップロードを送信&#x200B;]**」をクリックします。
