---
title: AdobeDynamic Media Classicデスクトップアプリケーション — 利用可能
description: Dynamic Media Classicデスクトップアプリケーションの詳細
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Administrator,Business Practitioner
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
source-git-commit: cba2c0ff2478b480d51b3c0f132003e14463a08a
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 1%

---

# 利用可能：AdobeDynamic Media Classicデスクトップアプリケーション {#dynamic-media-classic-desktop-app}

Dynamic Media Classicユーザーは、ブラウザーのAdobeFlashテクノロジーに依存しなくなった新しいデスクトップアプリケーションエクスペリエンスにアクセスできるようになりました。

この新しいアプリは、Windows®とmacOSで利用できるようになりました。

>[!IMPORTANT]
>
>Adobeでは、2020年10月2日までに新しいAdobeのDynamic Media Classicデスクトップアプリケーションをインストールすることをお勧めします。 これにより、AdobeFlash Playerの廃止を2020年12月31日に控える前に、スムーズな移行を確実におこなうことができます。 この日以降、AdobeDynamic Media Classicユーザーインターフェイスのブラウザーバージョン(製品内で「Dynamic Media Classic」というラベル)にログオンすることはできません。

[新しいDynamic Media Classicのログインエクスペリエンスに関するFAQを参照してください。](/help/new-ui-2020.md)

## Dynamic Media ClassicデスクトップAdobeの必要システム構成 {#system-requirements-dmc-app}

AdobeDynamic Media Classicデスクトップアプリケーションは、次のオペレーティングシステムと互換性があります。

* macOS 10.10以降。
* Windows® 7以降。

>[!NOTE]
>
>Dynamic Media Classicデスクトップアプリケーション内のアップグレード通知は、*マイナー*&#x200B;リリースに対しては生成されません。 マイナーリリースの修正のメリットがあるお客様は、アップグレードできます。

## マイナーリリース(20.21.2)の修正点 {#minor-release}

* 「サーバー」ドロップダウン20.21.1の既知の制限が空である。
* **[!UICONTROL アップロードジョブオプション]**&#x200B;で、**[!UICONTROL Photoshopオプション]**&#x200B;の下のレイヤー命名のデフォルト値が&#x200B;**[!UICONTROL Photoshopとレイヤー名]**&#x200B;になりました。 PSD ファイルのレイヤーは、個別の画像としてアップロードされます。
   * 以前の初期設定の&#x200B;**[!UICONTROL レイヤー名]**&#x200B;は、PSDファイル内のレイヤー名またはレイヤー番号に基づいて画像に名前を付けます。 PSDファイル内のレイヤー名がデフォルトのPhotoshopレイヤー名である場合は、レイヤー番号が使用されていました。
   * **[!UICONTROL Photoshopとレイヤー名]**&#x200B;の新しい初期設定では、PSDファイルの後にレイヤー名またはレイヤー番号が続く名前が画像に付けられます。 PSD ファイルのレイヤー名が、初期設定の Photoshop レイヤー名の場合は、レイヤー番号が使用されます。
   * Dynamic Media Classicのレイヤー画像に一意の名前が付けられるので、既存のPSDやテンプレート（元のPSDファイル内の共有レイヤー名）は更新されません。
* アセットの壊れたサムネール。

## 最新バージョンの修正(20.21.1) {#latest-fixes-desktop-app}

* タイムアウトによりサインインに問題が発生し、次のメッセージが表示されます。*このユーザーは、権限を持たずにグループに割り当てられる場合があります。 管理者に問い合わせてください。*
* 不正なパスワードが試行されるたびに、ビューアプリセットが複製されます。
* ルートフォルダー内の多くのアセットが原因で、デスクトップアプリケーションが応答しなくなる。 (Windows®で修正。（macOSで必要に応じて動作）。

## 以前のバージョンの修正点(20.20.2) {#previous-version-fixes-desktop-app}

* macOSとWindows®の両方でデスクトップアプリケーションのユーザーインターフェイスを使用してアップロードできるファイルの数に制限はありません。
* 会社を切り替えるためにデスクトップアプリケーションからサインアウトする必要はありません。
* Windows®で、貼り付け操作のCtrl+Vが機能するようになりました。
* 今後、新しいバージョンのデスクトップアプリケーションがリリースされると、デスクトップアプリケーション内でユーザーに通知が送信されます。

## macOSまたはWindows®での最新AdobeのDynamic Media Classicデスクトップアプリケーションのダウンロードとインストール {#installation-dmc-app}

関連項目:

* [最新AdobeのDynamic Media ClassicデスクトップアプリケーションをMacにダウンロードしてサイレントインストールする](#install-silent-mac-dmc-app)
* [Windows®での最新AdobeのDynamic Media Classicデスクトップアプリケーションのダウンロードとサイレントインストール](#install-silent-windows-dmc-app)

1. 古いバージョンのDynamic Media Classicデスクトップアプリケーションをシステムからアンインストールします。

1. Dynamic Media ClassicデスクトップアプリケーションのAdobe用の最新インストーラーをダウンロードします。

   * 最新バージョン(20.21.2)は、次の場所で入手できます。

      * [macOS(.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows® (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * 以前のバージョン(20.21.1)は、次の場所で入手できます。

      * [macOS(.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows® (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. ダウンロードしたインストーラーに基づいて、次のいずれかの操作を行います。

   * **macOSの場合**  - Drag &amp; drop to  **[!UICONTROL installダイアログボックスで、]** Dynamic Media Classicを **[!UICONTROL Adobe]** し、 **[!UICONTROL Applications]**&#x200B;にドロップします。

      ![macOSでのドラッグ&amp;ドロップインストール](/help/assets/dragondrop-install1.png)

   * **[!UICONTROL アプリケーション]**&#x200B;フォルダーで、AdobeDynamic Media Classicアイコンをタップします。
   * ダイアログボックスで、「**[!UICONTROL 開く]**」をタップして、Dynamic Media ClassicデスクトップAdobeを開きます。

      ![ダウンロードしたアプリを開く](/help/assets/open-dmclassicapp1.png)

   * **Windowsの場合**  — インストーラーバイナリを実行し、画面に表示される指示に従ってデスクトップアプリケーションをインストールします。

1. アプリケーションを開くと、新しいAdobeDynamic Media Classicログインページが表示されます。

   ![Dynamic Media Classicログイン](/help/assets/dmclassic-login1.png)

1. Dynamic Media ClassicデスクトップAdobeにログインするには、ブラウザーでDynamic Media Classicにログオンする際に使用したのと同じ資格情報を使用します。

   **[!UICONTROL サーバー]**&#x200B;を使用するには、実稼動環境で次のマッピングを参照してください。

   | ブラウザーURL | デスクトップアプリケーションサーバー名 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北米）生産 |
   | https://s7sps3.scene7.com/ | EMEA（ヨーロッパ、中東、アフリカ）の生産 |
   | https://s7sps5.scene7.com/ | APAC（アジア太平洋）生産 |

1. ログイン後、使い慣れたブラウザーユーザーインターフェイスが表示されます。 デスクトップアプリケーションでは、通常どおり1日を通じてDynamic Media Classicのアクティビティを続行できます。

## macOSで最新AdobeのDynamic Media Classicデスクトップアプリケーションをダウンロードし、*サイレント*&#x200B;インストールします。 {#install-silent-mac-dmc-app}

関連項目:

* [最新AdobeのDynamic Media ClassicデスクトップアプリケーションをMacまたはWindows®にダウンロードしてインストールする](#installation-dmc-app)
* [Windows®での最新AdobeのDynamic Media Classicデスクトップアプリケーションのダウンロードとサイレントインストール](#install-silent-windows-dmc-app)

macOSで最新バージョンのDynamic Media Classicデスクトップアプリケーションをダウンロードして&#x200B;*サイレント* Adobeするには、次の手順を実行します。

1. 古いバージョンのDynamic Media Classicデスクトップアプリケーションをシステムからアンインストールします。

1. macOS用Dynamic Media ClassicデスクトップアプリケーションAdobeの最新のインストーラーをダウンロードします。

   * [macOS(.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. 次のコマンドを使用して、ダウンロードしたディスク・イメージ(.DMG)をマウントポイントの場所にマウントします。

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. 次のコマンドを使用して、.APPファイルを&#x200B;**[!UICONTROL Applications]**&#x200B;にコピーします。

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG - hdiutil detach <mount_point_path>
   ```

1. アプリケーションを開くと、新しいAdobeDynamic Media Classicログインページが表示されます。

   ![Dynamic Media Classicログイン](/help/assets/dmclassic-login1.png)

1. Dynamic Media ClassicデスクトップAdobeにログインするには、ブラウザーでDynamic Media Classicにログオンする際に使用したのと同じ資格情報を使用します。

   **[!UICONTROL サーバー]**&#x200B;を使用するには、実稼動環境で次のマッピングを参照してください。

   | ブラウザーURL | デスクトップアプリケーションサーバー名 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北米）生産 |
   | https://s7sps3.scene7.com/ | EMEA（ヨーロッパ、中東、アフリカ）の生産 |
   | https://s7sps5.scene7.com/ | APAC（アジア太平洋）生産 |

## Windows®で最新AdobeのDynamic Media Classicデスクトップアプリケーションをダウンロードし、*サイレント*&#x200B;インストールします。 {#install-silent-windows-dmc-app}

使用するコマンドは、基本的なMSIサイレントインストール用です。 ただし、Dynamic Media Classicデスクトップアプリケーションのインストーラーは、InstallShieldを使用して作成されたInstallScript MSIインストーラーです。 インストーラーをレコードモードで実行すると、ユーザーの操作が応答ファイルに記録されます。 次に、[サイレントモードでのインストールの実行で説明されているように、この応答ファイルをサイレントインストールに使用します。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

関連項目:

* [最新AdobeのDynamic Media ClassicデスクトップアプリケーションをMacまたはWindows®にダウンロードしてインストールする](#installation-dmc-app)
* [macOSでの最新AdobeのDynamic Media Classicデスクトップアプリケーションのダウンロードとサイレントインストール](#install-silent-mac-dmc-app)

Windows®で最新バージョンのDynamic Media Classicデスクトップアプリケーションをダウンロードして&#x200B;*サイレント* Adobeするには、次の手順を実行します。

1. 古いバージョンのDynamic Media Classicデスクトップアプリケーションをシステムからアンインストールします。

1. Dynamic Media ClassicデスクトップアプリケーションのAdobe用の最新インストーラーをダウンロードします。

   * [Windows® (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. 次のコマンドを使用して、インストーラーをレコードモードで実行します。

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. GUIインストーラーウィンドウで、インストール場所などの操作/入力を`Setup.iss`ファイルに記録するように、手順に従ってをインストールします。

1. 作成した`Setup.iss`ファイルと`adobe-dynamic-media-classic-20.21.2.exe`を他のコンピューターにコピーします。

1. サイレント・インストールの場合は、次のコマンドを実行します。

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   コマンドラインパラメータの詳細は、[Setup.exeとUpdate.exeのコマンドラインパラメータで確認できます。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. アプリケーションを開くと、新しいAdobeDynamic Media Classicログインページが表示されます。

   ![Dynamic Media Classicログイン](/help/assets/dmclassic-login1.png)

1. Dynamic Media ClassicデスクトップAdobeにログインするには、ブラウザーでDynamic Media Classicにログオンする際に使用したのと同じ資格情報を使用します。

   **[!UICONTROL サーバー]**&#x200B;を使用するには、実稼動環境で次のマッピングを参照してください。

   | ブラウザーURL | デスクトップアプリケーションサーバー名 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北米）生産 |
   | https://s7sps3.scene7.com/ | EMEA（ヨーロッパ、中東、アフリカ）の生産 |
   | https://s7sps5.scene7.com/ | APAC（アジア太平洋）生産 |


## Dynamic Media Classic Desktop Appの使用に関するビデオウォークスルー {#dmc-app-video-walk-through}

Dynamic Media Classic Desktop App](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media)の使用に関する[ビデオのウォークスルーを視聴します(長さ：2分36秒)。

## デスクトップアプリケーションを使用したコンピューター上の画像キャッシュとアセットキャッシュのクリア {#clear-cache}

1. Dynamic Media Classicデスクトップアプリケーションで、右上隅付近にある&#x200B;**[!UICONTROL 設定]** / **[!UICONTROL 個人設定]**&#x200B;をタップします。
1. **[!UICONTROL 個人設定]**&#x200B;ページの「**[!UICONTROL デスクトップ]**」見出しの下で、次のいずれかの操作を行います。
   * Dynamic MediaでキャッシュされたすべてのAdobe画像ファイルをコンピューターから削除するには、「**[!UICONTROL 画像キャッシュをクリア]**」をタップし、「**[!UICONTROL OK]**」をタップします。
   * Dynamic MediaでキャッシュされたすべてのAdobeアセットファイルをコンピューターから削除するには、「**[!UICONTROL アセットキャッシュをクリア]**」をタップし、「**[!UICONTROL OK]**」をタップします。
1. ページの右下隅にある「**[!UICONTROL 閉じる]**」をタップします。

### 画像キャッシュとアセットキャッシュの手動でのクリア

デスクトップアプリケーションを使用して画像とアセットのキャッシュをクリアする以外に、ファイルシステムから直接キャッシュを手動でクリアできます。

1. ご使用のオペレーティングシステムに応じて、次の場所に移動します。

   * macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Dynamic Media Classic 20.21.1の既知の制限

* Dynamic Media Classicデスクトップアプリケーション20.21.1 — シナリオに更新した後、**[!UICONTROL Server]**&#x200B;ドロップダウンリストが空になる：Dynamic Media Classic 20.20.1または20.20.2をインストールしてログインし、アプリケーションを閉じます。 次に、Dynamic Media Classic 20.21.1に更新します。サインインしようとすると、**[!UICONTROL Sign in to your account]**&#x200B;ダイアログボックスの&#x200B;**[!UICONTROL Server]**&#x200B;ドロップダウンリストは空になります。 この問題を回避するには、[手動でキャッシュ](#clear-cache)をクリアする必要があります（上記の手順を参照）。

## Dynamic Media Classic 20.20.1の既知の制限(20.20.2で修正)

**_Windows®のみに適用 — デスクトップアプリケーションのUIを使用してアップロードできるファイルの数に制限はありますか。_**<br>はい。デスクトップアプリケーションのUIを使用して、一度に最大150個のファイルをアップロードできます。

**_Windows®とmacOSに適用 — 会社を切り替える方法&#x200B;_**<br>会社を切り替えるには、次の操作を行います。

* Dynamic Media Classicアプリで、会社ドロップダウンリストから新しい会社を選択します。
* ポップアップウィンドウが表示されたら、「**[!UICONTROL OK]**」をタップしてサインアウトし、アプリを閉じます。

   ![新しい会社を使用するには、アプリを再起動します。](/help/assets/dmclassic-new-company1.png)

* Dynamic Media Classicを再起動し、通常どおりにログインして、新しい会社で作業します。

## ヒントとテクニック

**_Dynamic Media ClassicのランディングページにMedia Cartパネルが表示されません。_**<br>Dynamic Media Classicで、設**[!UICONTROL 定/個人設定&#x200B;]**をタップします。「ブラウザー」セクションで、「**[!UICONTROL MediaPortal機能を表示&#x200B;]**」が選択（オン）されていることを確認します。**[!UICONTROL 保存/閉じる&#x200B;]**をタップします。

**_アセットの公開状態（緑のインジケーター）が正しく反映されません。_**<br>アセットの正しい公開状態を確認するには、ブラウザーのユーザーインターフェイスでUIに再ログインする必要がありました。デスクトップアプリケーションでは、Adobeのツールバーに**[!UICONTROL 更新&#x200B;]**アイコンが表示され、「**[!UICONTROL なし&#x200B;]**を選択」ボタンの右側に表示されます。**[!UICONTROL 更新&#x200B;]**アイコンをタップして、特定のページ上のすべてのアセットの最新のステータスを表示します。 ブラウザーUIと同様に、再ログインは不要です。

![更新アイ](/help/assets/refresh-icon1.png)
*コン更新アイコン*

**_デスクトップアプリケーションでバッチセットプリセットが機能しない。_**<br>アップロ**[!UICONTROL ード/ジョブオプション/バッチセットプリセット&#x200B;]**の順にタップします。関連する**[!UICONTROL バッチセットプリセット&#x200B;]**が有効になっていることを確認します。 「**[!UICONTROL アップロードを保存して送信&#x200B;]**」をクリックします。
