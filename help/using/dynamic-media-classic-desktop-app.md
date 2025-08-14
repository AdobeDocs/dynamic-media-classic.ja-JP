---
title: Adobe Dynamic Media Classic デスクトップ
description: 使用可能になったAdobe Dynamic Media Classic デスクトップアプリケーションの詳細について説明します。
contentOwner: rbrough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
topic: Administration
level: Intermediate
source-git-commit: afc347201b13c3b91ec5e1bd3ac5304442772f8d
workflow-type: tm+mt
source-wordcount: '1994'
ht-degree: 0%

---

# 提供開始：Adobe Dynamic Media Classic デスクトップアプリケーション {#dynamic-media-classic-desktop-app}

Adobe Dynamic Media Classic ユーザーは、ブラウザーのAdobe Flash テクノロジーに依存しなくなった新しいデスクトップアプリエクスペリエンスにアクセスできるようになりました。

この新しいアプリは、Windows® とmacOSで利用できるようになりました。

>[!IMPORTANT]
>
>Adobeでは、2020 年 10 月 1 日（PT）までに新しいAdobe Dynamic Media Classic デスクトップアプリケーションをインストールすることをお勧めします。 これにより、2020 年 12 月 31 日（PT）にAdobe Flash Player が非推奨（廃止予定）になる前に、スムーズに移行できます。 その日を過ぎると、ブラウザーバージョンのAdobe Dynamic Media Classic ユーザーインターフェイス（製品で「Adobe Dynamic Media Classic」というラベルが付いています）にログオンできなくなります。

[ 新しく利用可能になったAdobe Dynamic Media Classicへのログイン ](/help/using/new-ui-2020.md) については、FAQ を参照してください。

## Adobe Dynamic Media Classic デスクトップアプリケーションの動作環境 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic デスクトップアプリケーションは、次のオペレーティングシステムと互換性があります。

* macOS 10.10 以降。
* Windows® 7 以降。

完全なシステム要件については、[Adobe Dynamic Media Classic デスクトップアプリケーションのシステム要件 ](/help/using/system-requirements.md) を参照してください。

Adobe Dynamic Media Classic デスクトップアプリケーション内のアップグレード通知が、*マイナー* リリースでは生成されません。 マイナーリリースの修正によるメリットが得られる顧客は、アップグレードできます。

## 最新リリース（20.22.2）のmacOSでのみ修正されました {#release-feb2022}

* macOS Monterey：後続のアップロードで、ファイルのアップロードページがフリーズする。<!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## 最新リリース（20.22.1）の修正 {#release-jan2022}

* 画像を編集する際に、「**[!UICONTROL 保存]** ボタンが機能しませんでした。
* セットエディターで、「**[!UICONTROL Assetsを追加]** パネルにアセットをスクロールすると、**[!UICONTROL 閉じる]**、**[!UICONTROL 保存]** および **[!UICONTROL 名前を付けて保存]** ボタンが無効になります。
* ビデオの詳細表示の **[!UICONTROL 再生]** ボタンが機能しませんでした。
* macOS Monterey の実行時に、`d` ユーザー名 `e` フィールドと **[!UICONTROL パスワード]** フィールドに「**[!UICONTROL 」と「]**」を入力できなかった。
* 残りの Analytics API をバージョン 2.0 に移行しました。

## リリース 20.21.3 の修正点 {#release-sept2021}

* デスクトップアプリケーションで無操作状態が続いた後に表示されたアセットのサムネールの破損。
* デスクトップアプリケーションは、通常、設定操作の後に応答を停止します。
* **[!UICONTROL テスト画像サービング]** でリクエストの不明化とロックモードを自動的に有効にします。

  [ セキュアテストサービス ](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service) を参照してください。

* Adobe Analyticsの認証メカニズムを更新しました。 新しい統合に関連しているか、Dynamic Media Classic デスクトップアプリ内から一部の Analytics 変数を更新する必要がある場合。

  更新された手順については、[Adobe Analyticsへのログオン ](/help/using/log-analytics.md) を参照してください。

## リリース 20.21.2 の修正点 {#minor-release}

* 20.21.1 での既知の制限事項：ログイン画面の **[!UICONTROL サーバー]** ドロップダウンリストが空でした。
* **[!UICONTROL アップロードジョブオプション]** で、**[!UICONTROL Photoshop オプション]** のデフォルトのレイヤー名の値は、**[!UICONTROL Photoshopとレイヤー名]** になりました。 PSD ファイル内のレイヤーを別々の画像としてアップロードします。
   * 以前のデフォルトの **[!UICONTROL レイヤー名]** では、PSD ファイル内のレイヤー名またはレイヤー番号に従って画像に名前が付けられていました。 PSD ファイル内のレイヤー名がデフォルトのPhotoshop レイヤー名であった場合、レイヤー番号が使用されていました。
   * 新しいデフォルトの **[!UICONTROL Photoshopとレイヤー名]** では、画像はPSD ファイルの後にレイヤー名またはレイヤー番号を付けた名前になります。 PSD ファイル内のレイヤー名がデフォルトのPhotoshop レイヤー名である場合、レイヤー番号が使用されます。
   * Adobe Dynamic Media Classicのレイヤーイメージには一意の名前が付けられているので、既存のPSDやテンプレート（元のPSD ファイルで共有されるレイヤー名）は更新されません。
* アセットの壊れたサムネール。

## リリース 20.21.1 の修正 {#latest-fixes-desktop-app}

* タイムアウトが原因で次のメッセージが表示される場合は、ログインに問題があります。*このユーザーは、権限のない 1 つ以上のグループに割り当てられている可能性があります。 管理者にお問い合わせください。*
* ビューアプリセットは、誤ったパスワードの試行のたびに重複します。
* ルートフォルダー内のアセットが多いため、デスクトップアプリケーションが応答しなくなる。 （Windows® では修正済み。macOSでは必要に応じて動作します）。

## リリース 20.20.2 の修正点 {#previous-version-fixes-desktop-app}

* macOSと Windows® の両方で、デスクトップアプリケーションのユーザーインターフェイスを使用してアップロードできるファイルの数に制限はありません。
* 会社を切り替えるためにデスクトップアプリからログアウトする必要はありません。
* Windows® で Ctrl+V を押して貼り付け操作を実行できるようになりました。
* 今後、デスクトップアプリケーションの新しいバージョンがリリースされると、デスクトップアプリケーション内でユーザーに通知されるようになりました。

## 最新のAdobe Dynamic Media Classic デスクトップアプリケーションをmacOSまたは Windows® にダウンロードしてインストールする {#installation-dmc-app}

関連トピック：

* [Macに最新のAdobe Dynamic Media Classic デスクトップアプリケーションをダウンロードし、サイレントにインストールする](#install-silent-mac-dmc-app)
* [Windows に最新のAdobe Dynamic Media Classic デスクトップアプリをダウンロードし、サイレントにインストールする](#install-silent-windows-dmc-app)

1. 古いバージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをアンインストールします。

1. Adobe Dynamic Media Classic デスクトップアプリケーションの最新のインストーラーをダウンロードします。

   * 最新バージョンは以下で入手できます。

      * [macOS （.DMG）: ダウンロード ](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows （.EXE）: ダウンロード ](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * 以前のバージョンは次の場所で入手できます。

      * [macOS （.DMG）: ダウンロード ](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® （.EXE）: ダウンロード ](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. ダウンロードしたインストーラーに応じて、次のいずれかの操作を行います。

   * **macOS** – 「**[!UICONTROL ドラッグ&amp;ドロップしてインストール]**」ダイアログボックスで、「**[!UICONTROL Adobe Dynamic Media Classic]**」をドラッグして **[!UICONTROL アプリケーション]** にドロップします。

     ![macOSへのインストールをドラッグ&amp;ドロップ ](/help/using/assets/dragondrop-install1.png)

   * **[!UICONTROL Applications]** フォルダーで、「Adobe Dynamic Media Classic」アイコンをタップします。
   * ダイアログボックスで、「**[!UICONTROL 開く]** をタップして、Adobe Dynamic Media Classic デスクトップアプリケーションを開きます。

     ![ ダウンロードしたアプリを開く ](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - インストーラーバイナリを実行し、画面の指示に従ってデスクトップアプリケーションをインストールします。

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic ログインページが表示されます。

   ![Adobe Dynamic Media Classicへのログイン ](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicへのログオンに使用したのと同じ資格情報を使用します。

   **[!UICONTROL Server]** で使用するには、実稼動環境に対する次のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | NA 生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 地域（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC 実稼動（アジア太平洋） | https://s7sps5.scene7.com/ |

1. ログイン後、使い慣れたブラウザーユーザーインターフェイスのエクスペリエンスに注意してください。 デスクトップアプリでは、通常どおりに日常のAdobe Dynamic Media Classic アクティビティを続けることができます。

## macOSに最新のAdobe Dynamic Media Classic デスクトップアプリをダウンロードし ** サイレント）にインストールする {#install-silent-mac-dmc-app}

関連トピック：

* [最新のAdobe Dynamic Media Classic デスクトップアプリケーションをMacまたは Windows にダウンロードしてインストールする](#installation-dmc-app)
* [Windows に最新のAdobe Dynamic Media Classic デスクトップアプリをダウンロードし、サイレントにインストールする](#install-silent-windows-dmc-app)

macOSに最新バージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをダウンロードし *サイレントに* インストールするには：

1. 古いバージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをアンインストールします。

1. macOS用Adobe Dynamic Media Classic デスクトップアプリケーションの最新のインストーラーをダウンロードします。

   * [macOS （.DMG）: ダウンロード ](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. 次のコマンドを使用して、ダウンロードしたディスクイメージ（.DMG）をマウントポイントの場所にマウントします。

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. 次のコマンドを使用して、.APP ファイルを **[!UICONTROL Applications]** にコピーします。

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic ログインページが表示されます。

   ![Adobe Dynamic Media Classicへのログイン ](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicへのログオンに使用したのと同じ資格情報を使用します。

   **[!UICONTROL Server]** で使用するには、実稼動環境に対する次のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | NA 生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 地域（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC 実稼動（アジア太平洋） | https://s7sps5.scene7.com/ |

## Windows に最新のAdobe Dynamic Media Classic デスクトップアプリをダウンロードし ** サイレントに）インストールする® {#install-silent-windows-dmc-app}

使用するコマンドは、基本的な MSI サイレントインストール用です。 ただし、Adobe Dynamic Media Classic デスクトップアプリケーションインストーラーは、InstallShield を使用して作成された InstallScript MSI インストーラーです。 インストーラーを記録モードで実行すると、ユーザーの操作がすべて応答ファイルに記録されます。 次に、この応答ファイルは、「サイレントモードでのインストールの実行 [ で説明されているように、サイレントインストールに使用され ](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm) す。

関連トピック：

* [最新のAdobe Dynamic Media Classic デスクトップアプリケーションをMacまたは Windows にダウンロードしてインストールする](#installation-dmc-app)

* [macOSに最新のAdobe Dynamic Media Classic デスクトップアプリケーションをダウンロードし、サイレントにインストールする](#install-silent-mac-dmc-app)

Windows® 上で最新バージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをダウンロードし *サイレントにインストールするには、以下の手順に従います*。

1. 古いバージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをアンインストールします。

1. Adobe Dynamic Media Classic デスクトップアプリケーションの最新のインストーラーをダウンロードします。

   * [Windows® （.EXE）: ダウンロード ](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 次のコマンドを使用して、記録モードでインストーラーを実行します。

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. GUI インストーラーウィンドウで、インストール手順に従って、インストール場所などの操作/入力をファイルに記録 `Setup.iss` ます。

1. 作成した `Setup.iss` ファイルと `adobe-dynamic-media-classic-20.22.1.exe` を別のコンピューターにコピーします。

1. サイレントインストールの場合は、次のコマンドを実行します。

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   コマンド ライン パラメーターの詳細については、[Setup.exe および Update.exe コマンド ライン パラメーター ](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters) を参照してください。

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic ログインページが表示されます。

   ![Adobe Dynamic Media Classicへのログイン ](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicへのログオンに使用したのと同じ資格情報を使用します。

   **[!UICONTROL Server]** で使用するには、実稼動環境に対する次のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | NA 生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 地域（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC 実稼動（アジア太平洋） | https://s7sps5.scene7.com/ |

## Adobe Dynamic Media Classic デスクトップアプリケーションの使用に関するビデオウォークスルー {#dmc-app-video-walk-through}

Adobe Dynamic Media Classic デスクトップアプリケーションの使用方法に関する [ ビデオウォークスルー ](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) （長さ：2 分 36 秒）を視聴します。

## デスクトップアプリケーションを使用した、コンピューター上の画像キャッシュとアセットキャッシュのクリア {#clear-cache}

1. Adobe Dynamic Media Classic デスクトップアプリケーションの右上隅付近で、**[!UICONTROL 設定]**/**[!UICONTROL 個人設定]** をタップします。
1. **[!UICONTROL 個人用セットアップ]** ページの **[!UICONTROL デスクトップ]** 見出しの下で、次のいずれかの操作を行います。
   * Adobe Dynamic Media でキャッシュされたすべての画像ファイルをコンピューターから削除するには、**[!UICONTROL 画像キャッシュをクリア]** をタップし、**[!UICONTROL OK]** をタップします。
   * Adobe Dynamic Media でキャッシュされたすべてのアセットファイルをコンピューターから削除するには、「**[!UICONTROL アセットキャッシュをクリア]**」をタップし、「**[!UICONTROL OK]**」をタップします。
1. ページの右下隅にある「**[!UICONTROL 閉じる]** をタップします。

### 画像キャッシュとアセットキャッシュの手動消去

デスクトップアプリケーションを使用して画像とアセットのキャッシュをクリアする以外に、ファイルシステムから直接キャッシュを手動でクリアすることもできます。

1. オペレーティングシステムに応じて、次に移動します。

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic 20.21.1 の既知の制限

* Adobe Dynamic Media Classic デスクトップアプリケーション 20.21.1 にアップデートすると、「**[!UICONTROL サーバー]**」ドロップダウンリストが空になります。シナリオ：Adobe Dynamic Media Classic 20.20.1 または 20.20.2 をインストールしてログインし、アプリケーションを閉じます。 次に、Adobe Dynamic Media Classic 20.21.1 に更新します。ログインしようとすると、「**[!UICONTROL アカウントへのサインイン]**」ダイアログボックスの **[!UICONTROL サーバー]** ドロップダウンリストが空になります。 この問題を回避するには、[ 手動でキャッシュをクリア ](#clear-cache) する必要があります（上記の手順を参照）。

## Adobe Dynamic Media Classic 20.20.1 の既知の制限（20.20.2 で修正）

**_Windows のみ® - デスクトップアプリケーション UI を使用してアップロードできるファイルの数に制限はありますか？_**<br>はい。デスクトップアプリケーション UI を使用して一度にアップロードできるファイルは最大 150 個です。

**_Windows® とmacOSに適用 – 企業間を切り替える方法&#x200B;_**<br>会社を切り替えるには、次の手順を実行します。

* Adobe Dynamic Media Classic アプリケーションで、会社ドロップダウンリストから新しい会社を選択します。
* ポップアップウィンドウが表示されたら、「**[!UICONTROL OK]**」をタップしてログアウトし、アプリを閉じます。

  ![ 新しい会社を使用するには、アプリを再起動します ](/help/using/assets/dmclassic-new-company1.png)

* Adobe Dynamic Media Classicを再起動し、通常どおりログインして新しい会社で作業します。

## ヒントとテクニック

**_Adobe Dynamic Media Classicのランディングページにメディアの買い物かごパネルが表示されません。_**<br>Adobe Dynamic Media Classicで、**[!UICONTROL 設定/個人設定&#x200B;]**をタップします。 「ブラウザー」セクションで、「**[!UICONTROL MediaPortal 機能を表示&#x200B;]**」が選択（オン）されていることを確認します。**[!UICONTROL 保存/閉じる&#x200B;]**をタップします。

**_アセットの公開状態（緑色のインジケーター）が正しく反映されていない。_**<br>ブラウザーユーザーインターフェイスで、アセットの正しい公開状態を確認するには、UI への再ログインが必要でした。 デスクトップアプリケーションで、Adobeのツールバーの「**[!UICONTROL 何も選択しない&#x200B;]**ボタンの右側にある**[!UICONTROL 更新&#x200B;]**アイコンが導入されました。**[!UICONTROL 更新&#x200B;]**アイコンをタップして、特定のページ上のすべてのアセットの最新のステータスを表示します。 ブラウザー UI の場合のように、再ログオンは必要ありません。

![ 更新アイコン ](/help/using/assets/refresh-icon1.png)
*更新アイコン*

**_デスクトップアプリケーションでバッチセットプリセットが機能しません。_**<br>アップロード**[!UICONTROL ジョブオプション/バッチセットプリセット&#x200B;]**をタップします。 関連する**[!UICONTROL バッチセットプリセット&#x200B;]**が有効になっていることを確認します。**[!UICONTROL アップロードを保存して送信&#x200B;]**をクリックします。
