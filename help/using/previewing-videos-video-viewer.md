---
title: ビデオビューアでビデオをプレビューする
description: ビデオビューアでビデオをプレビューする方法を説明します。
uuid: 7ab4e805-6e5d-461b-bd99-5e09b9ced950
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 6a2e6df1-9186-42e2-9b85-01f132936c72
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: b8d1a0b4-67ab-482d-a685-a087fb850143
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 28%

---

# ビデオビューアでビデオをプレビューする{#previewing-videos-in-a-video-viewer}

ビデオビューアでビデオがどのように再生されるかをプレビューできます。

詳しくは、 [ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets).

**ビデオビューアでビデオをプレビューするには:**

1. 左側のアセットライブラリパネルの「表示」ドロップダウンリストで、 **[!UICONTROL ビデオ]** （1 つのエンコードされたビデオ）または **[!UICONTROL アダプティブビデオセット]**.アダプティブビデオエンコーディングプリセットを使用すると、マルチビットレートでエンコードされたビデオのセットが生成されます。
1. 左側のアセットライブラリパネルでアセットフォルダに移動し、プレビューするビデオを選択します。
1. 次のいずれかの操作を行います。

   * アセットウィンドウの上のツールバーの右側で、を選択します。 **[!UICONTROL リスト表示]**. Asset ウィンドウで、アセットにマウスポインターを置いて、「 **[!UICONTROL プレビュー]**.
   * アセットウィンドウの上のツールバーの右側で、を選択します。 **[!UICONTROL グリッド表示]**. アセットウィンドウのアセットのサムネールウィンドウで、 **[!UICONTROL プレビュー]**.
   * アセットウィンドウの上のツールバーの右側で、を選択します。 **[!UICONTROL 詳細ビュー]**. 同じツールバーで、 **[!UICONTROL プレビュー]**.
   * アセットウィンドウで、アセットを選択します。ツールバーで、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL プレビュー]**.

1. （オプション）プレビューウィンドウ下部のドロップダウンリストで、アセットの URL がコピーされるときにアセットの URL に適用する URL エンコーディングを選択します。
1. を選択します。 **[!UICONTROL プレビュー]** リンクをクリックして、選択したビューアでアセットを確認できます。
1. 表示されたビューアを閉じます。
1. 選択 **[!UICONTROL 閉じる]** をクリックして、アセット画面に戻ります。

>[!NOTE]
>
>Adobe Dynamic Media Classicは、MP4 ビデオをデスクトップでプレビューする便利な方法を提供しています。 この方法を使用すると、モバイルコンテンツを携帯端末で物理的にテストしないでコンテンツをデスクトップ上でプレビューできます。ただし、デスクトッププレビューで表示される内容は、モバイルデバイスでの再生を現実的に示すものではありません。 モバイルデバイスでのビデオの表示と再生をプレビューするには、プレビュー画面に移動し、 **[!UICONTROL URL をコピー]**&#x200B;をクリックし、モバイルデバイスの Web ブラウザーにその URL を入力します。 詳しくは、 [Web サイトやモバイルサイトにビデオをデプロイする](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

## ビデオビューアプリセットの操作 {#working-with-video-viewer-presets}

ユーザは、ビデオビューアでビデオを再生できます。ビデオビューアの動作、外観、再生コントロールの動作は、ビデオの再生用に選択したビューアプリセットに従います。ビデオプリセットはプレビュー画面で選択できます。プリセットを選択した後、選択したビューアプリセットを使用してビデオを再生するための URL または埋め込みコードを取得できます。

Adobe Dynamic Media Classicには、ビデオ再生用の定義済みのビューアプリセットが多数用意されています。管理者は、カスタムビューアプリセットを作成できます。 ビデオビューアの設定には、12 以上の異なる設定があります。 サイズ、カラー、ビデオコントロールとオーディオコントロール、プログレスバー、ユーザーインターフェイススキンおよびソーシャル機能を設定できます。

詳しくは、 [ビデオビューアでビデオをプレビューする](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

### ビデオビューアプリセットの追加または編集 {#adding-or-editing-a-video-viewer-preset}

ビューアプリセットを使用すると、各種ビューアタイプとその定義済み設定を表示できます。また、カスタマイズした独自のビューアプリセットを追加および編集したり、Adobe Dynamic Media Classicに付属する既存のビューアプリセットを編集したりすることもできます。

ビューアプリセットでは、ビューアプリセットのアクティブ化、フィルタリング、並べ替え、プレビューができます。

詳しくは[ビューアプリセット](application-setup.md#viewer_presets)を参照してください。

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

**ビデオビューアプリセットを追加または編集するには:**

1. Adobe Dynamic Media Classicの右上隅近くにある、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**.

   ビデオビューアのプリセットのみを表示するには、表のすぐ上にあるツールバーにある「ビューア」ドロップダウンリストで「ビデオビューア」を選択します。

1. ビデオを表示するビューアプリセットを追加または編集します。

   * **追加**  — 選択 **[!UICONTROL 追加]** 」と入力します。 ビューアプリセットを追加ダイアログボックスで、それぞれのドロップダウンリストからプラットフォームとビューアを選択し、 **[!UICONTROL 追加]**.
   関連トピック [ビューアプリセットの追加と編集](application-setup.md#adding_and_editing_viewer_presets).

   * **既存のビューアプリセットから開始して追加**  — 表で、ビデオビューアプリセットを選択し、「 **[!UICONTROL 編集]** 」と入力します。
   ビデオビューアを再設定したら、 **[!UICONTROL 名前を付けて保存]** 「プリセット名」テキストフィールドで別の名前を使用してプリセットを保存する場合。

   * **編集**  — ビデオビューアプリセットを選択し、「 」を選択します **[!UICONTROL 編集]**.



1. ビューアを設定ページの「プリセット名」フィールドに、プリセット名を入力または編集します。
1. 必要に応じてその他のオプションを設定します。

   オプションの説明を表示するには、その情報ヒントアイコンを選択します。

1. 次のいずれかの操作を行います。

   * 選択 **[!UICONTROL 名前を付けて保存]** 既存のプリセットから開始してビューアプリセットを追加した場合。
   * 選択 **[!UICONTROL 保存]** （ビューアプリセットを追加または編集した場合）

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)
>* [ビデオエンコーディングプリセットの操作](uploading-encoding-videos.md#working_with_video_encoding_presets)

