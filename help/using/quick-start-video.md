---
title: クイックスタート：Adobe Dynamic Media Classicのビデオ
description: Adobe Dynamic Media Classicの概要とクイックスタートのビデオを使用して、すぐに使い始めることができます。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
autotag-review: '2026-05-13T20:11:06.721Z'
TQID: 'https://experienceleague.adobe.com/lB0O224FfzW1smqCgkraE9czEF4XSD98qarRus6GEFw'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 1748
ht-degree: 19%

---

# クイックスタート：Adobe Dynamic Media Classicのビデオ{#quick-start-video}

Adobe Dynamic Media Classic Videoは、デスクトップ、iOS、Android™、BlackBerry®、Windows® モバイルデバイスなど、複数のスクリーンでストリーミングするための高品質なアダプティブビデオを簡単に公開できるエンドツーエンドのソリューションです。 アダプティブビデオセットは、同じビデオを異なるビットレート（400 kbps、800 kbps および 1000 kbps）やフォーマットでエンコードしたバージョンをグループ化します。 デスクトップコンピュータまたは携帯端末は、使用可能な帯域幅を検出します。

例えば、iOSのモバイルデバイスでは、3G、4G、Wi-Fiなどの帯域幅を検出します。 それに基づき、アダプティブビデオセットに含まれる各種ビデオビットレートの中から適切にエンコードされたビデオを自動的に選択します。 ビデオはデスクトップ、携帯端末またはタブレットにストリーミングされます。

さらに、デスクトップまたは携帯端末上でネットワークの状態が変化した場合は、ビデオ画質が自動的に動的に切り替わります。 また、お客様がデスクトップでフルスクリーンモードに入った場合、アダプティブビデオセットは、より良い解像度を使用して応答し、お客様の視聴体験を向上させます。 アダプティブビデオセットを使用すると、最適な再生が可能になります。 複数の画面やデバイスでAdobe Dynamic Media Classic Videoを再生する場合に最適です。

どのエンコードされたビデオを再生するか決定したり、どのエンコードされたビデオを再生中に選択するか決定するためにビデオプレーヤーが使用するロジックは、次のアルゴリズムに基づいています。

1. ビデオプレーヤーは、プレーヤー自体で「初期ビットレート」に設定されている値に最も近いビットレートに基づいて、初期ビデオフラグメントを読み込みます。
1. ビデオプレーヤーは、次の条件を使用して、帯域幅の速度の変更に基づいて切り替わります。

   1. プレーヤーは、推定された帯域幅より低いまたは等しい最も高い帯域幅ストリームを選択します。
   1. プレーヤーは、利用可能な帯域幅の80%のみを考慮します。 しかし、切り替えている場合、過大評価を避けて即座に切り替えるのは、わずか70%でより保守的です。

技術的な情報については、[https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp)のアルゴリズムのロジックを参照してください。

シングルビデオおよびアダプティブビデオセットを管理する場合、Adobe Dynamic Media Classicでは次の機能がサポートされています。

* 多数のサポートされているビデオ形式からビデオをアップロードします。 また、オーディオ形式をアップロードし、ビデオをMP4 H.264形式にエンコードして、複数の画面で再生できます。 定義済みのAdobe Dynamic Media Classic アダプティブビデオプリセット、シングルビデオエンコーディングプリセットを使用するか、独自のエンコーディングをカスタマイズして、ビデオの画質とサイズを制御できます。

[ アダプティブビデオプリセットの有効化または無効化](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)を参照してください

[ ビデオプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)のトレーニングビデオも参照してください。

アダプティブビデオセットが生成されると、MP4 ビデオが含まれます。

>[!NOTE]
>
>プライマリ/ソースビデオおよびその他のソースフォーマットのビデオは、アダプティブビデオセットに&#x200B;*not*&#x200B;追加されています。

* ユニバーサル_HTML5_Video、ユニバーサル_HTML5_MixedMedia_dark、ユニバーサル_HTML5_MixedMedia_light ビューアのビデオキャプションと、ユニバーサル_HTML5_Video、ユニバーサル_HTML5_MixedMedia_dark、ユニバーサル_HTML5_MixedMedia_light ビューアのビデオチャプターナビゲーション。

  [ ビデオにキャプションを追加](adding-captions-video.md)を参照してください。

  ビデオに[章マーカーを追加](adding-chapter-markers-video.md)を参照してください。

* 完全なメタデータサポートにより、ビデオを整理、参照および検索して、ビデオアセットの効率的な管理を実現します。
* アダプティブビデオセットをWebや、iPhone、iPad、Android™、BlackBerry®、Windows® phoneなどのデスクトップやモバイルデバイスに配信します。

  アダプティブビデオストリーミングは、様々なiOS プラットフォームでサポートされています。

  最新のサポートについては、[Adobe ビューアリファレンスガイド ](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources)を参照してください。

  Adobe Dynamic Media Classicは、MP4 H.264 ビデオのモバイルビデオ再生をサポートしています。<!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  このビデオ形式をサポートするWindows® デバイスは、次の場所にあります。

  [Windows® Phone](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs)でサポートされているビデオ形式。

* 次のようなAdobe Dynamic Media Classic ビューアプリセットを使用して、ビデオを再生します。

   * 単一の動画ビューアー：
   * ビデオコンテンツと画像コンテンツの両方を組み合わせた混在メディアビューア。

* ブランドニーズに合わせてビデオプレーヤーを設定します。
* シンプルなURLまたは埋め込みコードを使用して、web サイト、モバイルサイト、モバイルアプリケーションに動画を統合できます。

次のトレーニングビデオを参照してください。
* [MP4 ビデオの概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4 ビデオのプレビュー](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4 ビデオのアップロード ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [ ストリーミングの概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**クイックスタート**

次の手順を踏んだワークフローの説明は、Adobe Dynamic Media Classicのアダプティブビデオセットの使用を迅速に開始できるように設計されています。 各ステップの後、トピック見出しへの相互参照があり、詳細を確認できます。

## &#x200B;1. ビデオのアップロードとエンコード

次の 2 つのシナリオのうちいずれかを使用して、アダプティブビデオセットをアップロードおよび生成します。

* **プリエンコードされたビデオをアップロード**：ビデオが既にAdobe Dynamic Media Classicから外部でエンコードされている場合は、グローバルナビゲーションバーで「**[!UICONTROL アップロード]**」を選択します。 MP4 ビデオファイルを参照してAdobe Dynamic Media Classicに直接アップロードします。 次に、**[!UICONTROL ビルド]** > **[!UICONTROL アダプティブビデオセット]**&#x200B;に移動します。 ビデオファイルを参照します。 目的のビデオファイルをアダプティブビデオセットテーブルにドラッグ&amp;ドロップし、セットを保存します。
* **プライマリソースビデオをアップロード**：ビデオがエンコードされていない場合は、グローバルナビゲーションバーで「**[!UICONTROL アップロード]**」を選択して、プライマリビデオソースファイル（MP4以外）をアップロードします。 Adobe Dynamic Media Classicは、それらをMP4 ファイルにエンコードします。 **[!UICONTROL アップロードジョブオプション]** ダイアログボックスの&#x200B;**[!UICONTROL ビデオオプション]**&#x200B;で、**[!UICONTROL アダプティブビデオ]**&#x200B;を選択します。

  このオプションを使用すると、アダプティブビデオセットを作成できます。 正しいエンコーディングプリセットは、アップロードしたビデオのサイズに合わせて、16:9または4:3のビデオに自動的に適用されます。 アップロードジョブを送信すると、アダプティブビデオセットが自動的に作成され、3つのエンコードビデオ設定が正しい縦横比で含まれます。

  または、同じ&#x200B;**[!UICONTROL ジョブオプション]** ダイアログボックスの&#x200B;**[!UICONTROL ビデオオプション]**&#x200B;で、**[!UICONTROL シングルエンコーディングプリセット]**&#x200B;を展開します。 必要な個々のビデオエンコーディングプリセットを選択します。 **デスクトップ**、**モバイル（iPhone、iPad、Android™）**&#x200B;および&#x200B;**タブレット（iPad、Android™）**&#x200B;を選択して、MP4 ファイルを作成できます。

* または、**[!UICONTROL 再処理]**&#x200B;機能を使用してプライマリビデオを再処理することもできます。 新しくエンコードされたビデオは、既存のアダプティブビデオセットに追加されます。

[ ビデオのアップロードとエンコード ](uploading-encoding-videos.md#uploading_and_encoding_videos)を参照してください。

**オプション**

Adobe Dynamic Media Classicには、多数の定義済みビデオエンコーディングプリセットが用意されています。 これらの事前定義済みプリセットは、現在使用されている最も一般的なビデオエンコーディング設定を反映しており、ターゲットページでの再生に最適化されています。

ただし、さらにカスタマイズする必要がある場合は、管理者はビデオプリセットを作成して、エンドユーザー向けのビデオのサイズと再生操作をカスタマイズすることもできます。 管理者は、**[!UICONTROL セットアップ]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビデオプリセット]** > **[!UICONTROL 単一エンコーディングプリセット]**&#x200B;で利用可能なビデオプリセットページからビデオプリセットを追加および管理できます。 ビデオプリセットページには、ビデオプリセットの追加、編集、削除およびアクティブ化を行うオプションがあります。

[ ビデオエンコーディングプリセットの操作](uploading-encoding-videos.md#working_with_video_encoding_presets)を参照してください。

## &#x200B;2. ビデオビューアでのビデオのプレビュー

デスクトップ、web サイト、モバイルデバイス上のエンドユーザーに対して、ビデオの再生方法を確認するには、参照パネルでビデオを選択します。 次に、**[!UICONTROL プレビュー]**&#x200B;を選択します。

ビデオ ビューアで[ ビデオをプレビュー](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)を参照してください。

プレビューページでビデオを再生できます。 また、様々なビデオビューアを選択して、様々なプレーヤーでビデオがどのように表示されるかを確認することもできます。 ベストプラクティスとして、デスクトップ、タブレットおよび携帯端末でのマルチ画面再生には HTML5 ビデオプレーヤーを使用します。

**オプション**

ビューアプリセットのカスタマイズ：Adobe Dynamic Media Classicでは、ビデオを配信するための事前定義済みのビューアプリセットが提供されます。 これらのプリセットは、ビューアの外観と、その再生コントロールの動作を決定します。 管理者はビデオビューアをカスタマイズするために、ビューアプリセットページでビューアプリセットを追加および管理することができます。 このページを開くには、Adobe Dynamic Media Classicの右上隅にある&#x200B;**[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**&#x200B;に移動します。 ビューアプリセットページには、ビューアプリセットの追加、編集、削除およびアクティブ化を行うコマンドがあります。

[ ビデオビューアプリセットの操作](previewing-videos-video-viewer.md#working_with_video_viewer_presets)を参照してください。

[ ビデオプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS)のトレーニングビデオも参照してください。

## &#x200B;3. Web サイトとモバイルサイトへのビデオのデプロイ

ビデオを Web サイトに統合するには、次のいずれかの操作を行います。

* ビデオを独自のポップアップウィンドウまたはモーダルウィンドウで表示します。この場合、**[!UICONTROL URLをコピー]**&#x200B;機能を使用します。

  ビデオのURLを取得するには、グリッド表示またはリスト表示で、参照パネルでビデオを選択します。 「**[!UICONTROL プレビュー]**」を選択し、`Universal_HTML5_Viewer`の右側にある「**[!UICONTROL URLをコピー]**」を選択します。

  「**[!UICONTROL URLをコピー]**」を選択すると、URLがクリップボードにコピーされます。 Web サイト、モバイルサイトまたはアプリケーションの HTML にこのコードを設定します。

  >[!NOTE]
  >
  >URL はビデオまたはアダプティブビデオセットを公開するまでアクティブになりません。

* Web ページに埋め込まれたビデオを表示します。この場合は、埋め込まれたコード機能を使用します。

  ビデオの埋め込みコードを取得するには、グリッド表示またはリスト表示で、参照パネルでビデオを選択します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアーリスト]**&#x200B;に移動します。 テーブルの「アクション」列で、`Universal_HTML5_Video`の右側にある「**[!UICONTROL コードを埋め込む]**」を選択します。 コードの編集はできません。

  **[!UICONTROL 閉じる]**&#x200B;を選択し、埋め込まれたコードを1つ以上のWeb ページに貼り付けます。

  >[!NOTE]
  >
  >埋め込まれたコードは、ビデオまたはアダプティブビデオセットを公開した後にのみアクティブ化されます。

[Web サイトとモバイルサイトへのビデオのデプロイ ](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)を参照してください。

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)
