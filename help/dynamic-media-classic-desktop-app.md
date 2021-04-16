---
title: AdobeDynamic Mediaクラシックデスクトップアプリ — 現在提供中
description: Dynamic Mediaクラシックデスクトップアプリケーションの詳細を表示します。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
feature: Dynamic Mediaクラシック
role: Administrator,Business Practitioner
exl-id: 604b4630-4704-4254-84b5-91b33bb19d58
translation-type: tm+mt
source-git-commit: 8427c3ea6ca3083fd0868286e634a5569c62f7ab
workflow-type: tm+mt
source-wordcount: '1845'
ht-degree: 1%

---

# 利用可能：AdobeDynamic Mediaクラシックデスクトップアプリ{#dynamic-media-classic-desktop-app}

Dynamic Mediaクラシックのユーザーは、新しいデスクトップアプリケーションエクスペリエンスにアクセスできるようになりました。このエクスペリエンスでは、AdobeのFlashテクノロジーに依存しなくなりました。

この新しいアプリケーションは、Windows®とmacOSで使用できるようになりました。

>[!IMPORTANT]
>
>Adobeでは、2020年10月1日までに新しいAdobeのDynamic Mediaクラシックデスクトップアプリケーションをインストールすることをお勧めします。 これにより、スムーズなトランジションが得られ、AdobeFlash Playerは2020年12月31日に廃止されます。 その日以降は、AdobeのDynamic Mediaクラシックユーザインターフェイスのブラウザバージョンにログオンできません。製品のラベルは「Dynamic Mediaクラシック」です。

[新しいDynamic MediaクラシックログインエクスペリエンスのFAQを参照してください。](/help/new-ui-2020.md)

## AdobeDynamic Mediaクラシックデスクトップアプリケーション{#system-requirements-dmc-app}の必要システム構成

AdobeDynamic Mediaクラシックデスクトップアプリは、次のオペレーティングシステムと互換性があります。

* macOS 10.10以降。
* Windows® 7以降。

>[!NOTE]
>
>*マイナー*&#x200B;リリースに対しては、Dynamic Mediaクラシックデスクトップアプリケーション内のアップグレード通知は生成されません。 マイナーリリースの修正を受けるお客様は、アップグレードできます。

## マイナーリリース(20.21.2)の修正点{#minor-release}

* 20.21.1の「サーバ」ドロップダウンが空であるという既知の制限。
* **[!UICONTROL アップロードオプション]**&#x200B;で、**[!UICONTROL Photoshopオプション]**&#x200B;の下のレイヤーの初期設定値が&#x200B;**[!UICONTROL Photoshopとレイヤー名]**&#x200B;になりました。 PSD ファイルのレイヤーは、個別の画像としてアップロードされます。
   * 以前の初期設定の&#x200B;**[!UICONTROL レイヤー名]**&#x200B;は、PSDファイルのレイヤー名またはレイヤー番号に従って、画像に名前が付けられていました。 PSDファイル内のレイヤー名が初期設定のPhotoshopレイヤー名の場合は、レイヤー番号が使用されました。
   * 新しい初期設定の&#x200B;**[!UICONTROL Photoshopとレイヤー名]**&#x200B;では、PSDファイルの後にレイヤー名またはレイヤー番号が続く名前が画像に付けられます。 PSD ファイルのレイヤー名が、初期設定の Photoshop レイヤー名の場合は、レイヤー番号が使用されます。
   * Dynamic Mediaクラシックのレイヤー画像には一意の名前が付けられるので、既存のPSDまたはテンプレート（元のPSDファイル内の共有レイヤー名）は更新されません。
* アセットのサムネールの破損。

## 最新バージョン(20.21.1)の修正点{#latest-fixes-desktop-app}

* タイムアウトにより次のメッセージが表示されるログインの問題が発生しました：*このユーザーは、権限なしでグループに割り当てられる場合があります。 管理者に問い合わせてください。*
* ビューアプリセットは、間違ったパスワードが試行されるたびに複製されます。
* ルートフォルダー内の多くのアセットが原因で、デスクトップアプリケーションが応答しなくなる。 (Windows®で修正されました。（macOSで必要に応じて動作）。

## 以前のバージョン(20.20.2)の修正点{#previous-version-fixes-desktop-app}

* macOSとWindows®の両方で、デスクトップアプリのユーザーインターフェイスからアップロードできるファイル数に制限はありません。
* 会社を切り替えるために、デスクトップアプリケーションからサインアウトする必要はありません。
* Windows®で、貼り付け操作用のCtrl + Vが機能するようになりました。
* 今後、新しいバージョンのデスクトップアプリがリリースされると、ユーザーにはデスクトップアプリ内で通知されます。

## macOSまたはWindows® {#installation-dmc-app}に最新AdobeのDynamic Mediaクラシックデスクトップアプリをダウンロードしてインストールします

関連項目:

* [Macに最新AdobeのDynamic Mediaクラシックデスクトップアプリケーションをダウンロードしてサイレントインストールする](#install-silent-mac-dmc-app)
* [Windows®で最新AdobeのDynamic Mediaクラシックデスクトップアプリケーションをダウンロードしてサイレントインストールする](#install-silent-windows-dmc-app)

1. 古いバージョンのDynamic Mediaクラシックデスクトップアプリケーションをシステムからアンインストールします。

1. AdobeDynamic Mediaクラシックデスクトップアプリ用の最新インストーラーをダウンロードします。

   * 最新バージョン(20.21.2)は、次の場所で入手できます。

      * [macOS(.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)
      * [Windows® (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)
   * 以前のバージョン(20.21.1)は、次の場所で入手できます。

      * [macOS(.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.dmg)
      * [Windows® (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.1/adobe-dynamic-media-classic-20.21.1.exe)


<!--         * [macOS (.DMG) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.dmg)
        * [Windows (.EXE) - Download.](https://download.macromedia.com/dynamic-media-classic/20.20.2/adobe-dynamic-media-classic-20.20.2.exe) -->


1. ダウンロードしたインストーラーに基づいて、次のいずれかの操作を行います。

   * **macOSの場合** -  **[!UICONTROL Drag &amp; drop to]** installdialogダイアログボックスで、 **[!UICONTROL Adobe「Dynamic Mediaクラシック」をドラッグし、「ア]** プリケーション ****」にドロップします。

      ![macOSでのドラッグ&amp;ドロップによるインストール](/help/assets/dragondrop-install1.png)

   * **[!UICONTROL Applications]**&#x200B;フォルダー内で、Adobe「Dynamic Mediaクラシック」アイコンをタップします。
   * ダイアログボックスで、「**[!UICONTROL 開く]**」をタップして、AdobeのDynamic Mediaクラシックデスクトップアプリを開きます。

      ![ダウンロードしたアプリを開く](/help/assets/open-dmclassicapp1.png)

   * **Windowsの場合**  — インストーラーのバイナリを実行し、画面に表示される指示に従ってデスクトップアプリケーションをインストールします。

1. アプリを開くと、新しいAdobeの「Dynamic Mediaクラシックログイン」ページが表示されます。

   ![Dynamic Mediaクラシックサインイン](/help/assets/dmclassic-login1.png)

1. AdobeDynamic Mediaクラシックデスクトップアプリにサインインするには、ブラウザーでDynamic Mediaクラシックにログオンするのに使用したのと同じ資格情報を使用します。

   **[!UICONTROL Server]**&#x200B;を使用するには、本番環境の次のマッピングを参照してください。

   | ブラウザーURL | デスクトップアプリサーバー名 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北米）プロダクション |
   | https://s7sps3.scene7.com/ | EMEA（ヨーロッパ、中東、アフリカ）プロダクション |
   | https://s7sps5.scene7.com/ | APAC（アジア太平洋）生産 |

1. ログイン後は、使い慣れたブラウザーユーザーインターフェイスが表示されます。 デスクトップアプリケーションでは、通常どおり1日のDynamic Mediaクラシックアクティビティを継続できます。

## macOS {#install-silent-mac-dmc-app}に最新AdobeのDynamic Mediaクラシックデスクトップアプリをダウンロードして&#x200B;*サイレント*&#x200B;インストールします

関連項目:

* [MacまたはWindows®に最新AdobeのDynamic Mediaクラシックデスクトップアプリケーションをダウンロードしてインストールする](#installation-dmc-app)
* [Windows®で最新AdobeのDynamic Mediaクラシックデスクトップアプリケーションをダウンロードしてサイレントインストールする](#install-silent-windows-dmc-app)

macOSに最新バージョンのAdobeDynamic Mediaクラシックデスクトップアプリをダウンロードして&#x200B;*サイレント*&#x200B;インストールするには：

1. 古いバージョンのDynamic Mediaクラシックデスクトップアプリケーションをシステムからアンインストールします。

1. macOS用AdobeDynamic Mediaクラシックデスクトップアプリケーション用の最新インストーラーをダウンロードします。

   * [macOS(.DMG) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.dmg)

1. 次のコマンドを使用して、ダウンロードしたディスク・イメージ(.DMG)をマウントポイントの場所にマウントします。

   `hdiutil attach adobe-dynamic-media-classic-20.21.2.dmg -mountpoint <mount_point_path>`

1. 次のコマンドを使用して、.APPファイルを&#x200B;**[!UICONTROL Applications]**&#x200B;にコピーします。

   `rsync -a <mount_point_path>/Adobe\ Dynamic\ Media\ Classic.app /Applications/
Unmount DMG - hdiutil detach <mount_point_path>`

1. アプリを開くと、新しいAdobeの「Dynamic Mediaクラシックログイン」ページが表示されます。

   ![Dynamic Mediaクラシックサインイン](/help/assets/dmclassic-login1.png)

1. AdobeDynamic Mediaクラシックデスクトップアプリにサインインするには、ブラウザーでDynamic Mediaクラシックにログオンするのに使用したのと同じ資格情報を使用します。

   **[!UICONTROL Server]**&#x200B;を使用するには、本番環境の次のマッピングを参照してください。

   | ブラウザーURL | デスクトップアプリサーバー名 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北米）プロダクション |
   | https://s7sps3.scene7.com/ | EMEA（ヨーロッパ、中東、アフリカ）プロダクション |
   | https://s7sps5.scene7.com/ | APAC（アジア太平洋）生産 |

## Windows® {#install-silent-windows-dmc-app}に最新AdobeのDynamic Mediaクラシックデスクトップアプリをダウンロードして&#x200B;*サイレント*&#x200B;インストールします

使用するコマンドは、基本的なMSIサイレントインストール用です。 ただし、Dynamic Mediaクラシックデスクトップアプリケーションのインストーラーは、InstallShieldを使用して作成されたInstallScript MSIインストーラーです。 インストーラーを記録モードで実行すると、ユーザーの操作が応答ファイルに記録されます。 次に、[サイレントモードでのインストールの実行で説明されているように、この応答ファイルをサイレントインストールに使用します。](https://docs.revenera.com/installshield19helplib/helplibrary/SilentInstall.htm)

関連項目:

* [MacまたはWindows®に最新AdobeのDynamic Mediaクラシックデスクトップアプリケーションをダウンロードしてインストールする](#installation-dmc-app)
* [macOSで最新AdobeのDynamic Mediaクラシックデスクトップアプリケーションをダウンロードし、サイレントインストールする](#install-silent-mac-dmc-app)

Windows®で最新バージョンのAdobeDynamic Mediaクラシックデスクトップアプリをダウンロードして&#x200B;*サイレント*&#x200B;インストールするには：

1. 古いバージョンのDynamic Mediaクラシックデスクトップアプリケーションをシステムからアンインストールします。

1. AdobeDynamic Mediaクラシックデスクトップアプリ用の最新インストーラーをダウンロードします。

   * [Windows® (.EXE) — ダウンロード](https://download.macromedia.com/dynamic-media-classic/20.21.2/adobe-dynamic-media-classic-20.21.2.exe)

1. 次のコマンドを使用して、インストーラーを記録モードで実行します。

   `adobe-dynamic-media-classic-20.21.2.exe /r /f1"C:\Setup.iss"`

1. GUIインストーラーウィンドウで、インストールする手順に従って、インストール場所などの操作や入力を`Setup.iss`ファイルに記録します。

1. 作成した`Setup.iss`ファイルと`adobe-dynamic-media-classic-20.21.2.exe`を他のコンピューターにコピーします。

1. サイレントインストールを行うには、次のコマンドを実行します。

   `adobe-dynamic-media-classic-20.21.2.exe /s /f1"C:\Setup.iss"`

   コマンドラインパラメータの詳細については、[Setup.exeおよびUpdate.exeのコマンドラインパラメータを参照してください。](https://docs.revenera.com/installshield19helplib/helplibrary/IHelpSetup_EXECmdLine.htm)

1. アプリを開くと、新しいAdobeの「Dynamic Mediaクラシックログイン」ページが表示されます。

   ![Dynamic Mediaクラシックサインイン](/help/assets/dmclassic-login1.png)

1. AdobeDynamic Mediaクラシックデスクトップアプリにサインインするには、ブラウザーでDynamic Mediaクラシックにログオンするのに使用したのと同じ資格情報を使用します。

   **[!UICONTROL Server]**&#x200B;を使用するには、本番環境の次のマッピングを参照してください。

   | ブラウザーURL | デスクトップアプリサーバー名 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北米）プロダクション |
   | https://s7sps3.scene7.com/ | EMEA（ヨーロッパ、中東、アフリカ）プロダクション |
   | https://s7sps5.scene7.com/ | APAC（アジア太平洋）生産 |


## Dynamic Mediaクラシックデスクトップアプリの使用に関するビデオウォークスルー{#dmc-app-video-walk-through}

[ビデオのウォークスルービデオを見る(Dynamic Mediaクラシックデスクトップアプリの使用)](https://experienceleague.adobe.com/docs/experience-manager-learn/assets/dynamic-media/dynamic-media-classic-desktop-application.html#dynamic-media) (長さ：2分36秒)。

## デスクトップアプリケーション{#clear-cache}を使用して、コンピューター上の画像キャッシュとアセットキャッシュをクリアします

1. Dynamic Mediaクラシックデスクトップアプリケーションの右上隅近くで、**[!UICONTROL セットアップ]**/**[!UICONTROL 個人設定]**&#x200B;をタップします。
1. **[!UICONTROL 個人設定]**&#x200B;ページの&#x200B;**[!UICONTROL デスクトップ]**&#x200B;見出しの下で、次のいずれかの操作を行います。
   * Dynamic MediaにキャッシュされたすべてのAdobeの画像ファイルをコンピューターから削除するには、「**[!UICONTROL 画像キャッシュをクリア]**」をタップし、「**[!UICONTROL OK]**」をタップします。
   * Dynamic MediaがキャッシュしたアセットファイルをAdobeーからすべて削除するには、「**[!UICONTROL アセットキャッシュをクリア]**」をタップし、「**[!UICONTROL OK]**」をタップします。
1. ページ右下隅の「**[!UICONTROL 閉じる]**」をタップします。

### 画像キャッシュとアセットキャッシュの手動によるクリア

デスクトップアプリケーションを使用して画像とアセットのキャッシュを消去する以外に、ファイルシステムから直接手動でキャッシュをクリアできます。

1. オペレーティングシステムに応じて、次の場所に移動します。

   * macOS:`~/Library/Application\ Support/com.adobe.DMCDesktop/Local\ Store/`
   * Windows®: `C:\Users\YourUserName\AppData\Roaming\com.adobe.DMCDesktop\Local Store`

## Dynamic MediaClassic 20.21.1の既知の制限

* **[!UICONTROL Server]**&#x200B;ドロップダウンリストが空になるのは、Dynamic Mediaクラシックデスクトップアプリケーション20.21.1 — シナリオ：Dynamic MediaClassic 20.20.1または20.20.2をインストールしてサインインし、アプリケーションを閉じます。 次に、Dynamic MediaClassic 20.21.1に更新します。サインインしようとすると、**[!UICONTROL アカウント]**&#x200B;にサインインダイアログボックスの&#x200B;**[!UICONTROL サーバー]**&#x200B;ドロップダウンリストが空になります。 この問題を回避するには、[手動でキャッシュ](#clear-cache)をクリアする必要があります（上記の手順を参照）。

## Dynamic MediaClassic 20.20.1の既知の制限（20.20.2で修正）

**_Windows®にのみ適用されます。デスクトップアプリUIからアップロードできるファイルの数に制限はありますか。_**<br>はい。1度にアップロードできるファイル数は、デスクトップアプリUIから最大150個です。

**_Windows®とmacOSに適用 —会社を切り替える方法を教えてください。_**<br>会社を切り替えるには、次の手順を実行します。

* Dynamic Mediaクラシックアプリで、「会社」ドロップダウンリストから新しい会社を選択します。
* ポップアップウィンドウが表示されたら、「**[!UICONTROL OK]**」をタップしてサインアウトし、アプリを閉じます。

   ![新しい会社を使用するには、アプリを再起動します](/help/assets/dmclassic-new-company1.png)

* Dynamic Mediaクラシックを再起動し、通常どおりにサインインして新しい会社を使用します。

## ヒントとテクニック

**_Dynamic Mediaクラシックのランディングページでカートパネルが表示されません。_**<br>Dynamic Mediaクラシックで、**[!UICONTROL 設定/個人設定をタップします&#x200B;]**。「ブラウザー」セクションで、「**[!UICONTROL MediaPortal機能を表示&#x200B;]**」が選択されている（オンになっている）ことを確認します。**[!UICONTROL 保存/]**を閉じるをタップします。

**_アセットの公開状態（緑のインジケーター）が正しく反映されません。_**<br>ブラウザーのユーザーインターフェイスで、アセットの正しい公開状態を確認するには、UIに再ログインする必要がありました。デスクトップアプリケーションでは、Adobeがツールバーの**[!UICONTROL 「なしを選択」]**ボタンの右に**[!UICONTROL 更新&#x200B;]**アイコンを追加しました。**[!UICONTROL 更新&#x200B;]**アイコンをタップして、特定のページ上のすべてのアセットの最新のステータスを表示します。 ブラウザーUIと同様に再ログインする必要はありません。

![更新](/help/assets/refresh-icon1.png)
*アイコン更新アイコン*

**_デスクトップアプリでバッチセットプリセットが機能していない。_**<br>ア**[!UICONTROL ップロード/ジョブオプション/バッチセットプリセットをタップします&#x200B;]**。関連する**[!UICONTROL バッチセットプリセット&#x200B;]**が有効になっていることを確認します。 「**[!UICONTROL アップロードを保存して送信&#x200B;]**」をクリックします。
