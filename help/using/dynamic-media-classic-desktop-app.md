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

Adobe Dynamic Media Classic ユーザーは、ブラウザーのAdobeFlashテクノロジーに依存しなくなった新しいデスクトップアプリエクスペリエンスにアクセスできるようになりました。

この新しいアプリは、Windows® とmacOSで利用できるようになりました。

>[!IMPORTANT]
>
>Adobeでは、2020 年 10 月 1 日（PT）までに新しいAdobe Dynamic Media Classic デスクトップアプリケーションをインストールすることをお勧めします。 これにより、2020 年 12 月 31 日（PT）にAdobeFlash Playerが廃止される前に、スムーズに移行できます。 その日を過ぎると、ブラウザーバージョンのAdobe Dynamic Media Classic ユーザーインターフェイス（製品で「Adobe Dynamic Media Classic」というラベルが付いています）にログオンできなくなります。

の FAQ を参照してください [新しいAdobe Dynamic Media Classic ログインが利用できるようになりました。](/help/using/new-ui-2020.md)

## Adobe Dynamic Media Classic デスクトップアプリケーションの動作環境 {#system-requirements-dmc-app}

Adobe Dynamic Media Classic デスクトップアプリケーションは、次のオペレーティングシステムと互換性があります。

* macOS 10.10 以降。
* Windows® 7 以降。

完全なシステム要件については、を参照してください。 [Adobe Dynamic Media Classic デスクトップアプリケーションの動作環境](/help/using/system-requirements.md).

Adobe Dynamic Media Classic デスクトップアプリケーション内のアップグレード通知が用に生成されません *軽微* リリース。 マイナーリリースの修正によるメリットが得られる顧客は、アップグレードできます。

## 最新リリース（20.22.2）のmacOSでのみ修正されました {#release-feb2022}

* macOS Monterey：後続のアップロードで、ファイルのアップロードページがフリーズする。 <!-- https://jira.corp.adobe.com/browse/ASSETS-7948 -->

## 最新リリース（20.22.1）の修正 {#release-jan2022}

* 画像の編集時、 **[!UICONTROL 保存]** ボタンが機能しなかった。
* セットエディターで、 **[!UICONTROL 閉じる]**, **[!UICONTROL 保存]**、および **[!UICONTROL 名前を付けて保存]** でアセットをスクロールすると、ボタンが無効になる **[!UICONTROL アセットを追加]** パネル。
* この **[!UICONTROL 再生]** ビデオの詳細ビューのボタンが機能しませんでした。
* Could not enter `d` および `e` 。対象： **[!UICONTROL ユーザー名]** および **[!UICONTROL パスワード]** macOS Monterey を実行する際のフィールド。
* 残りの Analytics API をバージョン 2.0 に移行しました。

## リリース 20.21.3 の修正点 {#release-sept2021}

* デスクトップアプリケーションで無操作状態が続いた後に表示されたアセットのサムネールの破損。
* デスクトップアプリケーションは、通常、設定操作の後に応答を停止します。
* でリクエストの不明化とロックモードを自動的に有効にする **[!UICONTROL テスト画像サービング]**.

  参照： [セキュアテストサービス](/help/using/testing-assets-making-them-public.md#testing-the-secure-testing-service).

* Adobe Analyticsの認証メカニズムを更新しました。 新しい統合に関連しているか、Dynamic Media Classic デスクトップアプリ内から一部の Analytics 変数を更新する必要がある場合。

  参照： [Adobe Analyticsへのログオン](/help/using/log-analytics.md) （更新された手順）。

## リリース 20.21.2 の修正点 {#minor-release}

* 20.21.1 の既知の制限は、 **[!UICONTROL サーバー]** ログイン画面のドロップダウンリストが空でした。
* 対象： **[!UICONTROL アップロードジョブオプション]**：の下にあるデフォルトのレイヤー名の値 **[!UICONTROL Photoshopのオプション]**、現在 **[!UICONTROL Photoshopとレイヤー名]**. PSDファイル内のレイヤーを別々の画像としてアップロードします。
   * 以前のデフォルト **[!UICONTROL レイヤー名]**&#x200B;は、PSDファイル内のレイヤー名またはレイヤー番号に従って画像に名前を付けます。 PSDファイル内のレイヤー名がデフォルトのPhotoshop レイヤー名であった場合、レイヤー番号が使用されていました。
   * 新しいデフォルト **[!UICONTROL Photoshopとレイヤー名]**&#x200B;は、PSDファイルの後にレイヤー名またはレイヤー番号を付けた名前になります。 PSDファイル内のレイヤー名がデフォルトのPhotoshop レイヤー名である場合、レイヤー番号が使用されます。
   * Adobe Dynamic Media Classicのレイヤーイメージには一意の名前が付けられているため、既存のPSDやテンプレート（元のPSDファイルで共有されているレイヤー名）は更新されません。
* アセットの壊れたサムネール。

## リリース 20.21.1 の修正 {#latest-fixes-desktop-app}

* タイムアウトが原因でログインに問題が発生し、次のメッセージが表示される： *このユーザーは、権限なしで 1 つまたは複数のグループに割り当てることができます。 管理者にお問い合わせください。*
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

      * [macOS（.DMG）：ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)
      * [Windows （.EXE）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

   * 以前のバージョンは次の場所で入手できます。

      * [macOS（.DMG）：ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.dmg)
      * [Windows® （.EXE）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.exe)

<!--         * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.3/adobe-dynamic-media-classic-20.21.3.dmg) -->

<!--    * [macOS (.DMG): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
        * [Windows&reg; (.EXE): Download](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe) -->

<!--    * [macOS (.DMG): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE): Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. ダウンロードしたインストーラーに応じて、次のいずれかの操作を行います。

   * **macOS** に含まれます。 **[!UICONTROL ドラッグ&amp;ドロップでインストール]** ダイアログ ボックス、ドラッグする **[!UICONTROL Adobe Dynamic Media Classic]** それをドロップ **[!UICONTROL アプリケーション]**.

     ![macOSへのインストールをドラッグ&amp;ドロップ](/help/using/assets/dragondrop-install1.png)

   * が含まれる **[!UICONTROL アプリケーション]** フォルダーで、「Adobe Dynamic Media Classic」アイコンをタップします。
   * ダイアログボックスで、をタップします **[!UICONTROL 開く]** Adobe Dynamic Media Classic デスクトップアプリケーションを開きます。

     ![ダウンロードしたアプリを開く](/help/using/assets/open-dmclassicapp1.png)

   * **Windows** - インストーラーバイナリを実行し、画面の指示に従ってデスクトップアプリケーションをインストールします。

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic ログインページが表示されます。

   ![Adobe Dynamic Media Classicへのログイン](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicへのログオンに使用したのと同じ資格情報を使用します。

   の場合 **[!UICONTROL サーバー]** 使用するには、実稼動環境の以下のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | NA 生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 地域（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC 実稼動（アジア太平洋） | https://s7sps5.scene7.com/ |

1. ログイン後、使い慣れたブラウザーユーザーインターフェイスのエクスペリエンスに注意してください。 デスクトップアプリでは、通常どおりに日常のAdobe Dynamic Media Classic アクティビティを続けることができます。

## とをダウンロード *黙って* macOSへの最新のAdobe Dynamic Media Classic デスクトップアプリケーションのインストール {#install-silent-mac-dmc-app}

関連トピック：

* [最新のAdobe Dynamic Media Classic デスクトップアプリケーションをMacまたは Windows にダウンロードしてインストールする](#installation-dmc-app)
* [Windows に最新のAdobe Dynamic Media Classic デスクトップアプリをダウンロードし、サイレントにインストールする](#install-silent-windows-dmc-app)

とをダウンロードするには *黙って* macOSに最新バージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをインストールします。

1. 古いバージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをアンインストールします。

1. macOS用Adobe Dynamic Media Classic デスクトップアプリケーションの最新のインストーラーをダウンロードします。

   * [macOS（.DMG）：ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.2/adobe-dynamic-media-classic-20.22.2.dmg)

1. 次のコマンドを使用して、ダウンロードしたディスクイメージ（.DMG）をマウントポイントの場所にマウントします。

   `hdiutil attach adobe-dynamic-media-classic-20.22.2.dmg -mountpoint <mount_point_path>`

1. .APP ファイルをにコピーします **[!UICONTROL アプリケーション]** 次のコマンドを使用：

   ```
   rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
   Unmount DMG: hdiutil detach <mount_point_path>
   ```

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic ログインページが表示されます。

   ![Adobe Dynamic Media Classicへのログイン](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicへのログオンに使用したのと同じ資格情報を使用します。

   の場合 **[!UICONTROL サーバー]** 使用するには、実稼動環境の以下のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | NA 生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 地域（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC 実稼動（アジア太平洋） | https://s7sps5.scene7.com/ |

## とをダウンロード *黙って* windows® への最新のAdobe Dynamic Media Classic デスクトップアプリケーションのインストール {#install-silent-windows-dmc-app}

使用するコマンドは、基本的な MSI サイレントインストール用です。 ただし、Adobe Dynamic Media Classic デスクトップアプリケーションインストーラーは、InstallShield を使用して作成された InstallScript MSI インストーラーです。 インストーラーを記録モードで実行すると、ユーザーの操作がすべて応答ファイルに記録されます。 その後、この応答ファイルは、で説明されているように、サイレントインストールに使用されます。 [サイレントモードでのインストールの実行](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/SilentInstall.htm).

関連トピック：

* [最新のAdobe Dynamic Media Classic デスクトップアプリケーションをMacまたは Windows にダウンロードしてインストールする](#installation-dmc-app)

* [macOSに最新のAdobe Dynamic Media Classic デスクトップアプリケーションをダウンロードし、サイレントにインストールする](#install-silent-mac-dmc-app)

とをダウンロードするには *黙って* windows® に最新バージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをインストールします。

1. 古いバージョンのAdobe Dynamic Media Classic デスクトップアプリケーションをアンインストールします。

1. Adobe Dynamic Media Classic デスクトップアプリケーションの最新のインストーラーをダウンロードします。

   * [Windows® （.EXE）: ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.22.1/adobe-dynamic-media-classic-20.22.1.exe)

1. 次のコマンドを使用して、記録モードでインストーラーを実行します。

   `adobe-dynamic-media-classic-20.22.1.exe /r /f1"C:\Setup.iss"`

1. GUI インストーラーウィンドウで、インストール手順に従って、インストール場所などの操作/入力をに記録します `Setup.iss` ファイル。

1. 作成したのコピー `Setup.iss` ファイルと `adobe-dynamic-media-classic-20.22.1.exe` 別のコンピューターに送信します。

1. サイレントインストールの場合は、次のコマンドを実行します。

   `adobe-dynamic-media-classic-20.22.1.exe /s /f1"C:\Setup.iss"`

   コマンドラインパラメーターの詳細については、を参照してください。 [Setup.exe および Update.exe コマンド ライン パラメーター](https://docs.revenera.com/installshield25helplib/installshield25helplib.htm#helplibrary/IHelpSetup_EXECmdLine.htm?Highlight=Setup.exe%20and%20Update.exe%20Command-Line%20Parameters).

1. アプリケーションを開くと、新しいAdobe Dynamic Media Classic ログインページが表示されます。

   ![Adobe Dynamic Media Classicへのログイン](/help/using/assets/dmclassic-login1.png)

1. Adobe Dynamic Media Classic デスクトップアプリケーションにログインするには、ブラウザーでAdobe Dynamic Media Classicへのログオンに使用したのと同じ資格情報を使用します。

   の場合 **[!UICONTROL サーバー]** 使用するには、実稼動環境の以下のマッピングを参照してください。

   | サーバ | ブラウザー URL |
   | --- | --- |
   | NA 生産（北米） | https://s7sps1.scene7.com/ |
   | EMEA 地域（ヨーロッパ、中東、アフリカ） | https://s7sps3.scene7.com/ |
   | APAC 実稼動（アジア太平洋） | https://s7sps5.scene7.com/ |

## Adobe Dynamic Media Classic デスクトップアプリケーションの使用に関するビデオウォークスルー {#dmc-app-video-walk-through}

を視聴 [Adobe Dynamic Media Classic デスクトップアプリケーションの使用に関するビデオウォークスルー](https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application#dynamic-media) （長さ：2 分 36 秒）。

## デスクトップアプリケーションを使用した、コンピューター上の画像キャッシュとアセットキャッシュのクリア {#clear-cache}

1. Adobe Dynamic Media Classic デスクトップアプリケーションの右上隅付近にあるをタップします **[!UICONTROL 設定]** > **[!UICONTROL 個人設定]**.
1. 日 **[!UICONTROL 個人設定]** ページの下 **[!UICONTROL デスクトップ]** 見出し。次のいずれかの操作を行います。
   * Dynamic MediaにキャッシュされたすべてのAdobe画像ファイルをコンピューターから削除するには、をタップします **[!UICONTROL 画像キャッシュのクリア]**&#x200B;をタップし、 **[!UICONTROL OK]**.
   * Dynamic MediaでキャッシュされたすべてのAdobeアセットファイルをコンピューターから削除するには、をタップします **[!UICONTROL アセットキャッシュのクリア]**&#x200B;をタップし、 **[!UICONTROL OK]**.
1. ページの右下隅にあるをタップします。 **[!UICONTROL 閉じる]**.

### 画像キャッシュとアセットキャッシュの手動消去

デスクトップアプリケーションを使用して画像とアセットのキャッシュをクリアする以外に、ファイルシステムから直接キャッシュを手動でクリアすることもできます。

1. オペレーティングシステムに応じて、次に移動します。

   * macOS: `~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Adobe Dynamic Media Classic 20.21.1 の既知の制限

* この **[!UICONTROL サーバー]** Adobe Dynamic Media Classic デスクトップアプリケーション 20.21.1 にアップデートすると、ドロップダウンリストが空になります。シナリオ：Adobe Dynamic Media Classic 20.20.1 または 20.20.2 をインストールしてログインし、アプリケーションを閉じます。 次に、Adobe Dynamic Media Classic 20.21.1 に更新します。ログインしようとすると、 **[!UICONTROL サーバー]** のドロップダウンリスト **[!UICONTROL アカウントにサインイン]** ダイアログボックスが空です。 この問題を回避するには、次の操作をおこなう必要があります [手動でキャッシュをクリアする](#clear-cache) （上記の手順を参照してください）。

## Adobe Dynamic Media Classic 20.20.1 の既知の制限（20.20.2 で修正）

**_Windows® のみに適用 – デスクトップアプリケーション UI を使用してアップロードできるファイルの数に制限はありますか？_**<br>はい。デスクトップアプリケーション UI を使用して一度にアップロードできるファイルは最大 150 個です。

**_Windows® とmacOSに適用 – 企業間を切り替える方法&#x200B;_**<br>会社を切り替えるには、次の手順を実行します。

* Adobe Dynamic Media Classic アプリケーションで、会社ドロップダウンリストから新しい会社を選択します。
* ポップアップウィンドウが表示されたら、をタップします **[!UICONTROL OK]** からサインアウトしてアプリを閉じます。

  ![新しい会社を使用するには、アプリを再起動します](/help/using/assets/dmclassic-new-company1.png)

* Adobe Dynamic Media Classicを再起動し、通常どおりログインして新しい会社で作業します。

## ヒントとテクニック

**_Adobe Dynamic Media Classicのランディングページにメディアの買い物かごパネルが表示されません。_**<br>Adobe Dynamic Media Classicで、をタップします**[!UICONTROL 設定/個人設定&#x200B;]**. 「ブラウザー」セクションで、次のことを確認します**[!UICONTROL MediaPortal 機能の表示&#x200B;]**が選択（チェック済み）されています。 タップ**[!UICONTROL 保存/閉じる&#x200B;]**.

**_アセットの公開状態（緑色のインジケーター）が正しく反映されていません。_**<br>ブラウザーのユーザーインターフェイスで、アセットの正しい公開状態を確認するには、UI への再ログインが必要でした。 デスクトップアプリケーションでは、Adobeは以下を導入しました**[!UICONTROL 更新&#x200B;]**アイコンをクリックします（ツールバーの右側）**[!UICONTROL 何も選択しない&#x200B;]**ボタン。 をタップします**[!UICONTROL 更新&#x200B;]**アイコンをクリックして、特定のページ上のすべてのアセットの最新のステータスを表示します。 ブラウザー UI の場合のように、再ログオンは必要ありません。

![更新アイコン](/help/using/assets/refresh-icon1.png)
*更新アイコン*

**_デスクトップアプリケーションでバッチセットプリセットが機能しません。_**<br>タップ**[!UICONTROL アップロード/ジョブオプション/バッチセットプリセット&#x200B;]**. 関連するを確認します**[!UICONTROL バッチセットプリセット&#x200B;]**が有効になっています。 クリック**[!UICONTROL アップロードの保存と送信&#x200B;]**.
