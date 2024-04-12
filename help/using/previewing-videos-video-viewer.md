---
title: ビデオビューアでビデオをプレビューする
description: ビデオビューアでビデオをプレビューする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: b8d1a0b4-67ab-482d-a685-a087fb850143
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 21%

---

# ビデオビューアでビデオをプレビューする{#previewing-videos-in-a-video-viewer}

ビデオビューアでビデオがどのように再生されるかをプレビューできます。

参照： [ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets).

**ビデオビューアでビデオをプレビューするには：**

1. 左側のアセットライブラリパネルの「表示」ドロップダウンリストで、以下を選択します。 **[!UICONTROL ビデオ]** （シングルエンコードビデオ）または **[!UICONTROL アダプティブビデオセット]**. アダプティブビデオエンコーディングプリセットを使用すると、一連の複数ビットレートのエンコードされたビデオが作成されます。
1. 左側のアセットライブラリパネルでアセットフォルダに移動し、プレビューするビデオを選択します。
1. 次のいずれかの操作を行います。

   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL リスト表示]**. アセットウィンドウで、アセットの上にマウスポインターを置き、次のいずれかを選択します **[!UICONTROL プレビュー]**.
   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL グリッド表示]**. アセットウィンドウのアセットサムネールウィンドウで、次の項目を選択します **[!UICONTROL プレビュー]**.
   * Assets ウィンドウの上のツールバーの右側で、次の項目を選択します **[!UICONTROL 詳細ビュー]**. 同じツールバーで、を選択します。 **[!UICONTROL プレビュー]**.
   * アセットウィンドウで、アセットを選択します。ツールバーの、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL プレビュー]**.

1. （オプション）プレビューウィンドウの下部にあるドロップダウンリストで、アセットの URL をコピーするときに適用する URL エンコーディングを選択します。
1. 「」を選択します **[!UICONTROL プレビュー]** 選択したビューアでアセットを確認できるリンクが表示されます。
1. 表示されたビューアを閉じます。
1. を選択 **[!UICONTROL 閉じる]** をクリックして、アセット画面に戻ります。

>[!NOTE]
>
>Adobe Dynamic Media Classicは、デスクトップで MP4 ビデオをプレビューする便利な方法を提供します。 この方法を使用すると、モバイルコンテンツを携帯端末で物理的にテストしないでコンテンツをデスクトップ上でプレビューできます。ただし、デスクトッププレビューで表示される内容は、モバイルデバイスでの再生の外観を現実的に示すものではないことに注意してください。 モバイルデバイスでのビデオの表示と再生をプレビューするには、プレビュー画面に移動し、次のチェックボックスをオンにします **[!UICONTROL URL をコピー]**&#x200B;を開き、モバイルデバイスの web ブラウザーでその URL を入力します。 詳しくは、を参照してください [Web サイトやモバイルサイトにビデオをデプロイします](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

## ビデオビューアプリセットの操作 {#working-with-video-viewer-presets}

ユーザは、ビデオビューアでビデオを再生できます。ビデオビューアの動作、外観、再生コントロールの動作は、ビデオの再生用に選択したビューアプリセットに従います。ビデオプリセットはプレビュー画面で選択できます。プリセットを選択すると、選択したビューアプリセットを使用してビデオを再生するための URL または埋め込みコードを取得できます。

Adobe Dynamic Media Classicには、ビデオを再生するための事前定義済みのビューアプリセットが多数用意されています。管理者は、カスタムビューアプリセットを作成できます。 ビデオビューアの設定には、12 種類以上の設定があります。 サイズ、カラー、ビデオコントロールとオーディオコントロール、プログレスバー、ユーザーインターフェイススキンおよびソーシャル機能を設定できます。

参照： [ビデオビューアでビデオをプレビューする](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

### ビデオビューアプリセットの追加または編集 {#adding-or-editing-a-video-viewer-preset}

ビューアプリセットを使用すると、各種ビューアタイプとその定義済み設定を表示できます。独自のカスタマイズされたビューアプリセットを追加して編集したり、Adobe Dynamic Media Classicに付属している既存のビューアプリセットを編集したりすることもできます。

ビューアプリセットでは、ビューアプリセットのアクティベート、フィルタリング、並べ替え、プレビューを行うことができます。

詳しくは、[ビューアプリセット](application-setup.md#viewer_presets)を参照してください。

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

**ビデオビューアプリセットを追加または編集するには：:**

1. Adobe Dynamic Media Classicの右上隅にあるに移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.

   ビデオビューアのプリセットのみを表示するには、テーブルのすぐ上にあるツールバーの「ビューアを開く」ドロップダウンリストから「ビデオビューア」を選択します。

1. ビデオを表示するビューアプリセットを追加または編集します。

   * **追加**  – を選択 **[!UICONTROL 追加]** ツールバーの ビューアプリセットを追加ダイアログボックスで、各ドロップダウンリストからプラットフォームとビューアを選択して、を選択します。 **[!UICONTROL 追加]**.

   関連トピック [ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets).

   * **既存のビューアプリセットから開始して追加**  – 表で、ビデオビューアプリセットを選択し、次に選択します **[!UICONTROL 編集]** ツールバーの

   ビデオ・ビューアを再構成した後、次の項目を選択します。 **[!UICONTROL 名前を付けて保存]** プリセット名テキストフィールドで別の名前を使用してプリセットを保存します。

   * **編集** - ビデオビューアプリセットを選択してから、を選択します **[!UICONTROL 編集]**.

1. が含まれる `Configure Viewer` ページの「プリセット名」フィールドで、プリセット名を入力または編集します。
1. 必要に応じてその他のオプションを設定します。

   オプションの説明を表示するには、オプションの情報ヒントアイコンを選択します。

1. 次のいずれかの操作を行います。

   * を選択 **[!UICONTROL 名前を付けて保存]** 既存のプリセットから開始してビューアプリセットを追加した場合。
   * を選択 **[!UICONTROL 保存]** ビューアプリセットを追加または編集した場合。

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)
>* [ビデオエンコーディングプリセットの操作](uploading-encoding-videos.md#working_with_video_encoding_presets)
