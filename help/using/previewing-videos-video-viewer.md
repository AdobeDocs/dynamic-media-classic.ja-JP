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
source-git-commit: c4613c78347c4bda3d84747a72146617158c03b6
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 21%

---

# ビデオビューアでビデオをプレビューする{#previewing-videos-in-a-video-viewer}

ビデオビューアでビデオがどのように再生されるかをプレビューできます。

[ ビューアプリセットの追加と編集 ](application-setup.md#adding_and_editing_viewer_presets) を参照してください。

**ビデオビューアでビデオをプレビューするには：**

1. 左側のアセットライブラリパネルの「表示」ドロップダウンリストで、「**[!UICONTROL ビデオ]**」（単一のエンコードビデオ）または「**[!UICONTROL アダプティブビデオセット]**」を選択します。 アダプティブビデオエンコーディングプリセットを使用すると、一連の複数ビットレートのエンコードされたビデオが作成されます。
1. 左側のアセットライブラリパネルでアセットフォルダに移動し、プレビューするビデオを選択します。
1. 次のいずれかの操作を行います。

   * Assetsウィンドウの上のツールバーの右側にある「**[!UICONTROL リスト表示]**」を選択します。 アセットウィンドウで、アセットの上にマウスポインターを置き、「**[!UICONTROL プレビュー]**」を選択します。
   * Assetsウィンドウの上のツールバーの右側にある「**[!UICONTROL グリッド表示]**」を選択します。 アセットウィンドウのアセットサムネールウィンドウで、「**[!UICONTROL プレビュー]**」を選択します。
   * Assetsウィンドウの上のツールバーの右側にある「**[!UICONTROL 詳細ビュー]**」を選択します。 同じツールバーで「**[!UICONTROL プレビュー]**」を選択します。
   * アセットウィンドウで、アセットを選択します。ツールバーで、**[!UICONTROL ファイル]**/**[!UICONTROL プレビュー]** に移動します。

1. （オプション）プレビューウィンドウの下部にあるドロップダウンリストで、アセットの URL をコピーするときに適用する URL エンコーディングを選択します。
1. **[!UICONTROL プレビュー]** リンクを選択すると、選択したビューアでアセットを確認できます。
1. 表示されたビューアを閉じます。
1. 「**[!UICONTROL 閉じる]**」を選択して、Assets画面に戻ります。

>[!NOTE]
>
>Adobe Dynamic Media Classicは、デスクトップで MP4 ビデオをプレビューする便利な方法を提供します。 この方法を使用すると、モバイルコンテンツを携帯端末で物理的にテストしないでコンテンツをデスクトップ上でプレビューできます。ただし、デスクトッププレビューで表示される内容は、モバイルデバイスでの再生の外観を現実的に示すものではないことに注意してください。 モバイルデバイスでのビデオの表示と再生をプレビューするには、プレビュー画面に移動します。 **[!UICONTROL URL をコピー]** をクリックして、モバイルデバイスの web ブラウザーにその URL を入力します。 詳しくは、[Web サイトやモバイルサイトへのビデオのデプロイ ](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites) を参照してください。

## ビデオビューアプリセットの操作 {#working-with-video-viewer-presets}

ユーザは、ビデオビューアでビデオを再生できます。ビデオビューアの動作、外観、再生コントロールの動作は、ビデオの再生用に選択したビューアプリセットに従います。ビデオプリセットはプレビュー画面で選択できます。プリセットを選択すると、選択したビューアプリセットを使用してビデオを再生するための URL または埋め込みコードを取得できます。

Adobe Dynamic Media Classicには、ビデオを再生するための事前定義済みのビューアプリセットが多数用意されています。管理者は、カスタムビューアプリセットを作成できます。 ビデオビューアの設定には、12 種類以上の設定があります。 サイズ、カラー、ビデオコントロールとオーディオコントロール、プログレスバー、ユーザーインターフェイススキンおよびソーシャル機能を設定できます。

[ ビデオビューアでビデオをプレビューする ](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer) を参照してください。

[ ビデオプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) のトレーニングビデオも参照してください。

### ビデオビューアプリセットを追加または編集する {#adding-or-editing-a-video-viewer-preset}

ビューアプリセットを使用すると、各種ビューアタイプとその定義済み設定を表示できます。カスタマイズした独自のビューアプリセットを追加して編集したり、Adobe Dynamic Media Classicに付属している既存のビューアプリセットを編集したりすることもできます。

ビューアプリセットでは、ビューアプリセットのアクティベート、フィルタリング、並べ替え、プレビューを行うことができます。

詳しくは、[ビューアプリセット](application-setup.md#viewer_presets)を参照してください。

[ ビデオプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) のトレーニングビデオも参照してください。

**ビデオビューアプリセットを追加または編集するには：**

1. Adobe Dynamic Media Classicの右上隅付近にある **[!UICONTROL 設定]**/**[!UICONTROL ビューアプリセット]** に移動します。

   ビデオビューアのプリセットのみを表示するように選択できます。 テーブルのすぐ上のツールバーで、「ビューアを開く」ドロップダウンリストから「ビデオビューア」を選択します。

1. ビデオを表示するビューアプリセットを追加または編集します。

   * **追加**：ツールバーの **[!UICONTROL 追加]** を選択します。 ビューアプリセットを追加ダイアログボックスで、それぞれのドロップダウンリストからプラットフォームとビューアを選択して、「**[!UICONTROL 追加]**」を選択します。

   [ ビューアプリセットの追加と編集 ](application-setup.md#adding_and_editing_viewer_presets) も参照してください。

   * **既存のビューアプリセットから開始して追加**：テーブルで、ビデオビューアプリセットを選択したあと、ツールバーで **[!UICONTROL 編集]** を選択します。

   ビデオビューアを再設定した後、「**[!UICONTROL 名前を付けて保存]**」を選択して、「プリセット名」テキストフィールドで別の名前を使用してプリセットを保存します。

   * **編集**：ビデオビューアプリセットを選択してから、**[!UICONTROL 編集]** を選択します。

1. `Configure Viewer` ページの「プリセット名」フィールドで、プリセット名を入力または編集します。
1. 必要に応じてその他のオプションを設定します。

   オプションの説明を表示するには、オプションの情報ヒントアイコンを選択します。

1. 次のいずれかの操作を行います。

   * 既存のプリセットから開始してビューアプリセットを追加した場合は、「**[!UICONTROL 名前を付けて保存]**」を選択します。
   * ビューアプリセットを追加または編集した場合は、「**[!UICONTROL 保存]**」を選択します。

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)
>* [ ビデオエンコーディングプリセットの操作 ](uploading-encoding-videos.md#working_with_video_encoding_presets)
