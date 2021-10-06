---
title: ビデオビューアでのビデオのプレビュー
description: ビデオビューアでビデオをプレビューする方法を説明します。
uuid: 7ab4e805-6e5d-461b-bd99-5e09b9ced950
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 6a2e6df1-9186-42e2-9b85-01f132936c72
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: b8d1a0b4-67ab-482d-a685-a087fb850143
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 29%

---

# ビデオビューアでのビデオのプレビュー{#previewing-videos-in-a-video-viewer}

ビデオビューアでビデオがどのように再生されるかをプレビューできます。

[ ビューアプリセットの追加と編集 ](application-setup.md#adding_and_editing_viewer_presets) を参照してください。

**ビデオビューアでビデオをプレビューするには:**

1. 左側のアセットライブラリパネルの「表示」ドロップダウンリストで、「**[!UICONTROL ビデオ]**」（単一にエンコードされたビデオ）または「**[!UICONTROL アダプティブビデオセット]**」を選択します。アダプティブビデオエンコーディングプリセットを使用すると、マルチビットレートでエンコードされたビデオのセットが生成されます。
1. 左側のアセットライブラリパネルでアセットフォルダに移動し、プレビューするビデオを選択します。
1. 次のいずれかの操作を行います。

   * アセットウィンドウの上のツールバーの右側で、「**[!UICONTROL リスト表示]**」を選択します。 Asset ウィンドウで、アセットの上にマウスポインターを置いて、**[!UICONTROL Preview]** を選択します。
   * アセットウィンドウの上のツールバーの右側で、「**[!UICONTROL グリッドビュー]**」を選択します。 Asset ウィンドウのアセットのサムネールウィンドウで、「**[!UICONTROL プレビュー]**」を選択します。
   * Assets ウィンドウの上のツールバーの右側で、**[!UICONTROL 詳細ビュー]** を選択します。 同じツールバーで、「**[!UICONTROL プレビュー]**」を選択します。
   * アセットウィンドウで、アセットを選択します。ツールバーで、**[!UICONTROL ファイル]** / **[!UICONTROL プレビュー]** に移動します。

1. （オプション）プレビューウィンドウ下部のドロップダウンリストで、アセットの URL がコピーされるときにアセットの URL に適用する URL エンコーディングを選択します。
1. 「**[!UICONTROL プレビュー]**」リンクを選択して、選択したビューアでアセットをレビューできるようにします。
1. 表示されたビューアを閉じます。
1. 「**[!UICONTROL 閉じる]**」を選択して、アセット画面に戻ります。

>[!NOTE]
>
>Adobe Dynamic Media Classicは、デスクトップで MP4 ビデオをプレビューする便利な方法を提供します。 この方法を使用すると、モバイルコンテンツを携帯端末で物理的にテストしないでコンテンツをデスクトップ上でプレビューできます。ただし、デスクトッププレビューで表示される内容は、モバイルデバイスでの再生を現実的に示すものではありません。 モバイルデバイスでのビデオの外観と再生をプレビューするには、プレビュー画面に移動し、「**[!UICONTROL URL をコピー]**」を選択して、モバイルデバイスの Web ブラウザーにその URL を入力します。 詳しくは、[Web サイトおよびモバイルサイトへのビデオのデプロイ ](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites) を参照してください。

## ビデオビューアプリセットの操作 {#working-with-video-viewer-presets}

ユーザは、ビデオビューアでビデオを再生できます。ビデオビューアの動作、外観、再生コントロールの動作は、ビデオの再生用に選択したビューアプリセットに従います。ビデオプリセットはプレビュー画面で選択できます。プリセットを選択した後、選択したビューアプリセットを使用してビデオを再生するための URL または埋め込みコードを取得できます。

Adobe Dynamic Media Classicには、ビデオを再生するための定義済みのビューアプリセットが多数用意されています。管理者は、カスタムビューアプリセットを作成できます。 ビデオビューア設定のための 10 種類以上の設定が用意されています。サイズ、カラー、ビデオコントロールとオーディオコントロール、プログレスバー、ユーザーインターフェイススキンおよびソーシャル機能を設定できます。

[ ビデオビューアでのビデオのプレビュー ](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer) を参照してください。

[ ビデオプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) のトレーニングビデオも参照してください。

### ビデオビューアプリセットの追加または編集 {#adding-or-editing-a-video-viewer-preset}

ビューアプリセットを使用すると、各種ビューアタイプとその定義済み設定を表示できます。また、カスタマイズした独自のビューアプリセットを追加および編集したり、Adobe Dynamic Media Classicに付属する既存のビューアプリセットを編集したりすることもできます。

ビューアプリセットでは、ビューアプリセットのアクティブ化、フィルタリング、並べ替え、プレビューができます。

詳しくは[ビューアプリセット](application-setup.md#viewer_presets)を参照してください。

[ ビデオプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) のトレーニングビデオも参照してください。

**ビデオビューアプリセットを追加または編集するには:**

1. Adobe Dynamic Media Classicの右上隅付近で、**[!UICONTROL 設定]** / **[!UICONTROL ビューアプリセット]** に移動します。

   ビデオビューアのプリセットのみを表示するには、表のすぐ上にあるツールバーの開いている「ビューア」ドロップダウンリストから「ビデオビューア」を選択します。

1. ビデオを表示するビューアプリセットを追加または編集します。

   * **追加**  — ツールバーで「追 **** 加」を選択します。ビューアプリセットを追加ダイアログボックスで、それぞれのドロップダウンリストからプラットフォームとビューアを選択し、「**** を追加」を選択します。
   [ ビューアプリセットの追加と編集 ](application-setup.md#adding_and_editing_viewer_presets) も参照してください。

   * **既存のビューアプリセットから開始して追加**  — 表で、ビデオビューアプリセットを選択し、ツールバーの「編 **** 集」を選択します。
   ビデオビューアを再設定した後、「**[!UICONTROL 名前を付けて保存]**」を選択して、「プリセット名」テキストフィールドに別の名前を入力してプリセットを保存します。

   * **編集**  — ビデオビューアプリセットを選択し、「編 **[!UICONTROL 集]**」を選択します。



1. ビューアを設定ページの「プリセット名」フィールドに、プリセット名を入力または編集します。
1. 必要に応じてその他のオプションを設定します。

   オプションの説明を確認するには、その情報ヒントアイコンを選択します。

1. 次のいずれかの操作を行います。

   * 既存のプリセットから開始してビューアプリセットを追加した場合は、「**[!UICONTROL 名前を付けて保存]**」を選択します。
   * ビューアプリセットを追加または編集した場合は、「**[!UICONTROL 保存]**」を選択します。

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)
>* [ビデオエンコーディングプリセットの操作](uploading-encoding-videos.md#working_with_video_encoding_presets)

