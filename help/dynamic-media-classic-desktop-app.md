---
title: AdobeDynamic Mediaクラシックデスクトップアプリ — 利用可能
seo-title: AdobeDynamic Mediaクラシックデスクトップアプリ — 利用可能
description: 'null'
seo-description: Dynamic Mediaクラシックデスクトップアプリの詳細を表示します。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/introducing_adobe_dynamic_media_classic
translation-type: tm+mt
source-git-commit: 59116a685629cfd788c32fb5082f35d90e66fb5a
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 0%

---


# 利用可能： AdobeDynamic Mediaクラシックデスクトップアプリ {#dynamic-media-classic-desktop-app}

Dynamic Mediaクラシックのユーザーは、ブラウザーのAdobe Flashテクノロジーに依存しなくなった新しいデスクトップアプリケーションエクスペリエンスにアクセスできるようになりました。

この新しいアプリがWindowsとmacOSで使用できるようになりました。

>[!IMPORTANT]
>
>2020年10月1日までに、新しいAdobeDynamic Mediaクラシックデスクトップアプリケーションをインストールすることをお勧めします。 これにより、スムーズなトランジションが確保され、Adobe Flash Playerが2020年12月31日に廃止されます。 この日、製品のScene7 Publishing Systemというラベルが付いたAdobeDynamic MediaClassicユーザインターフェイスのブラウザバージョンにログオンできなくなります。

新 [規Dynamic MediaクラシックログインエクスペリエンスのFAQを参照してください](/help/new-ui-2020.md)。

## AdobeDynamic Mediaクラシックデスクトップアプリケーションの必要システム構成 {#system-requirements-dmc-app}

AdobeDynamic Mediaクラシックデスクトップアプリは、次のオペレーティングシステムと互換性があります。
* macOS X 10.10以降。
* Windows 7以降。

## AdobeDynamic Mediaクラシックデスクトップアプリケーションのダウンロードとインストール {#installation-dmc-app}

1. システム上の古いDynamic MediaのClassicデスクトップアプリケーションをすべてアンインストールします。

1. AdobeDynamic Mediaクラシックデスクトップアプリ用の最新インストーラーをダウンロードします。

   * macOS(.dmg) - [ダウンロード](http://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.dmg)。
   * Windows(.exe) - [ダウンロード](lhttp://download.macromedia.com/dynamic-media-classic/20.20.1/adobe-dynamic-media-classic-20.20.1.exe)。

1. ダウンロードしたインストーラーに基づいて、次のいずれかの操作を行います。

   * **macOSの場合** - **[!UICONTROL Drag &amp; drop to install]** （ドラッグ&amp;ドロップしてインストール）ダイアログボックスで、 **[!UICONTROL AdobeDynamic MediaClassic]** （クラシック）をドラッグし、「 **[!UICONTROL Applications]**（アプリケーション）」にドロップします。

      ![macOSでのドラッグ&amp;ドロップによるインストール](/help/assets/dragondrop-install.png)

   * 「 **[!UICONTROL Applications]** 」フォルダーで、「AdobeDynamic Mediaクラシック」アイコンをタップします。
   * ダイアログボックスで「 **[!UICONTROL 開く]** 」をタップし、AdobeDynamic Mediaクラシックデスクトップアプリケーションを開きます。

      ![ダウンロードしたアプリを開く](/help/assets/open-dmclassicapp.png)

   * **Windowsの場合** — インストーラーバイナリを実行し、画面に表示される指示に従ってデスクトップアプリケーションをインストールします。

1. アプリを開くと、新しいAdobeDynamic Mediaクラシックログインページが表示されます。

   ![Dynamic Mediaクラシックサインイン](/help/assets/dmclassic-login.png)

1. ブラウザーの資格情報と同じ資格情報を使用してAdobeDynamic Mediaクラシックにサインインします。

   使用する **[!UICONTROL Server]** 、実稼働環境に対する次のマッピングを参照してください。

   | ブラウザーURL | デスクトップアプリサーバー名 |
   |---|---|
   | https://s7sps1.scene7.com/ | NA（北米）プロダクション |
   | https://s7sps3.scene7.com/ | EMEA（ヨーロッパ、中東、アフリカ）プロダクション |
   | https://s7sps5.scene7.com/ | APAC（アジア太平洋）生産 |

1. ログインUIを投稿すると、使い慣れたブラウザーUIが表示されます。 デスクトップアプリUIでは、通常どおり1日アクティビティを提供できます。

## ClassicDynamic Mediaの既知の制限

**_Windowsのみに適用 — デスクトップアプリUIからアップロードできるファイルの数に制限はありますか？_**<br>&#x200B;はい。1度にアップロードできるファイル数は、デスクトップアプリUIから最大150個です。

**_WindowsとmacOSに適用されます。会社を切り替える方法を教えてください。_**<br>&#x200B;会社を切り替えるには、次の手順を実行します。
* Dynamic Mediaクラシックアプリで、会社のドロップダウンリストから新しい会社を選択します。
* ポップアップが表示されたら、「 **[!UICONTROL OK]** 」をタップしてサインアウトし、アプリを閉じます。

   ![新しい会社を使用するには、アプリを再起動します](/help/assets/dmclassic-new-company.png)
* Dynamic MediaClassicを再起動し、通常どおりにサインインして新しい会社を使用します。

## ヒントとテクニック

**_Dynamic Mediaクラシックのランディングページにカートパネルが表示されません。_**<br> Dynamic Mediaクラシックで、 **[!UICONTROL 設定/個人設定をタップします]**。 「ブラウザー」セクションで、「Media Portal機能を **[!UICONTROL 表示」が選択されている(オンになっている]** )ことを確認します。 **[!UICONTROL 保存/閉じるをタップします]**。

**_アセットの公開状態（緑のインジケーター）が正しく反映されません。_**<br>&#x200B;アセットの正しい公開状態を確認するには、ブラウザUIでUIに再ログインする必要がありました。 デスクトップアプリでは、ツールバーの「なしを **[!UICONTROL 選択]** 」ボタンの右側に **[!UICONTROL 「更新]** 」アイコンが追加されました。 「 **[!UICONTROL 更新]** 」アイコンをタップして、特定のページ上のすべてのアセットの最新のステータスを表示します。 ブラウザーUIと同様に、再ログインする必要はありません。

![更新アイコン](/help/assets/refresh-icon.png)*更新アイコン*

**_デスクトップアプリでバッチセットプリセットが機能していない。_**<br>&#x200B;ア **[!UICONTROL ップロード/ジョブオプション/バッチセットプリセットをタップします]**。 関連する **[!UICONTROL バッチセットプリセットが有効になっていることを確認します]** 。 「アップロードを **[!UICONTROL 保存して送信]**」をクリックします。
