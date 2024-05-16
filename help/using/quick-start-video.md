---
title: 「クイックスタート：Adobe Dynamic Media Classicのビデオ」
description: すぐに使い始めるのに役立つAdobe Dynamic Media Classicの概要とクイックスタート ビデオです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
topic: Content Management
level: Beginner
source-git-commit: 5140b62c76970cfcee271664f11b1ff605625fe7
workflow-type: tm+mt
source-wordcount: '1443'
ht-degree: 23%

---

# クイックスタート：Adobe Dynamic Media Classicのビデオ{#quick-start-video}

Adobe Dynamic Media Classic ビデオは、高品質のアダプティブビデオを簡単に公開して、デスクトップ、iOS、Android™、BlackBerry®、Windows® モバイルデバイスなど、複数の画面にストリーミングするためのエンドツーエンドのソリューションです。 アダプティブビデオセットは、同じビデオを異なるビットレート（400 kbps、800 kbps および 1000 kbps）やフォーマットでエンコードしたバージョンをグループ化します。デスクトップコンピュータまたは携帯端末は、使用可能な帯域幅を検出します。

例えば、iOS の携帯端末では、3G、4G または Wi-Fi などの帯域幅を検出します。それに基づき、アダプティブビデオセットに含まれる各種ビデオビットレートの中から適切にエンコードされたビデオを自動的に選択します。ビデオはデスクトップ、携帯端末またはタブレットにストリーミングされます。

さらに、デスクトップまたは携帯端末上でネットワークの状態が変化した場合は、ビデオ画質が自動的に動的に切り替わります。また、デスクトップが全画面表示モードに切り替わった場合、アダプティブビデオセットがより高い解像度を使用するように応答するので、ユーザーの視聴エクスペリエンスが向上します。 アダプティブビデオセットを使用すると、最適な再生が可能になります。 Adobe Dynamic Media Classic ビデオを複数の画面やデバイスで再生する場合に最適です。

どのエンコードされたビデオを再生するか決定したり、どのエンコードされたビデオを再生中に選択するか決定するためにビデオプレーヤーが使用するロジックは、次のアルゴリズムに基づいています。

1. ビデオプレーヤーは、プレーヤー自体の「初期ビットレート」に設定されている値に最も近いビットレートに基づいて、初期ビデオフラグメントを読み込みます。
1. 次の条件を使用して、帯域幅の速度の変化に応じてビデオプレーヤーが切り替わります。

   1. プレーヤーは、推定帯域幅以下の最大帯域幅ストリームを選択する。
   1. プレーヤーは、使用可能な帯域幅の 80% ほどを見積もります。 ただし、切り替えを行う場合は、過度に見積もられるのを避け、すぐに切り替えるために、より保守的なのは 70% のみです。

でアルゴリズムのロジックを確認します [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) に関する技術情報。

1 つのビデオおよびアダプティブビデオセットの管理の場合、Adobe Dynamic Media Classicは次の機能をサポートしています。

* 多数のサポートされているビデオ形式からビデオをアップロードする。 複数の画面で再生するために、オーディオ形式をアップロードし、ビデオを MP4 H.264 形式にエンコーディングする。 事前定義済みのAdobe Dynamic Media Classic アダプティブビデオプリセット、または 1 つのビデオのエンコーディングプリセットを使用するか、独自のエンコーディングをカスタマイズしてビデオの画質とサイズを制御することができます。

参照： [アダプティブビデオプリセットをアクティベートまたはアクティベート解除する](/help/using/application-setup.md#activating-or-deactivating-adaptive-video-presets)

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

生成されるアダプティブビデオセットには、MP4 ビデオが含まれます。

>[!NOTE]
>
>プライマリ/ソースビデオおよびその他のソースフォーマットビデオは次のとおりです *ではない* がアダプティブビデオセットに追加されました。

* Univeral_HTML5_Video ビューア、Universal_HTML5_MixedMedia_dark ビューア、Universal_HTML5_MixedMedia_light ビューアでのビデオキャプション、および Univeral_HTML5_Video ビューア、Universal_HTML5_MixedMedia_dark ビューア、Universal_HTML5_MixedMedia_light ビューアでのビデオチャプターナビゲーション。

  参照： [ビデオへのキャプションの追加](adding-captions-video.md).

  参照： [ビデオへのチャプターマーカーの追加](adding-chapter-markers-video.md).

* 完全なメタデータサポートにより、ビデオを整理、参照および検索して、ビデオアセットの効率的な管理を実現します。
* アダプティブビデオセットは、Web や、iPhone、iPad、Android™、BlackBerry®、Windows® Phone などのデスクトップやモバイルデバイスに配信できます。

  アダプティブビデオのストリーミングは、様々なiOS プラットフォームでサポートされています。

  の最新のサポートを参照してください [Adobeビューアリファレンスガイド](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources).

  Adobe Dynamic Media Classicでは、MP4 H.264 ビデオのモバイルビデオ再生がサポートされています。 <!-- LINK IS 404; NO SUITABLE REPLACEMENT WAS FOUND You can find BlackBerry&reg; devices that support this video format at the following website: -->

  <!-- See [Supported video formats on BlackBerry&reg;](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482). -->

  このビデオ形式をサポートする Windows® デバイスについては、次の場所で確認できます。

  [Windows® Phone でサポートされるビデオ形式](https://learn.microsoft.com/en-us/windows/uwp/audio-video-camera/supported-codecs).

* 次のようなAdobe Dynamic Media Classic ビューアプリセットを使用してビデオを再生します。

   * 単一のビデオビューア。
   * ビデオコンテンツと画像コンテンツの両方を組み合わせた混在メディアビューア。

* ブランドニーズに合わせてビデオプレーヤーを設定します。
* 単純な URL か埋め込みコードを使用して、ビデオを web サイト、モバイルサイトまたはモバイルアプリケーションに統合します。

以下のトレーニングビデオを参照してください。
* [MP4 ビデオの概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4 ビデオのプレビュー](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4 ビデオのアップロード](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [ストリーミングの概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**クイックスタート**

次のワークフローの手順説明は、Adobe Dynamic Media Classicでアダプティブビデオセットをすぐに使い始めることを目的としたものです。 各手順に続いて、詳細な情報を見つけることができるトピックの見出しへの相互参照があります。

## 1. ビデオのアップロードとエンコード

次の 2 つのシナリオのうちいずれかを使用して、アダプティブビデオセットをアップロードおよび生成します。

* **事前エンコードされたビデオのアップロード**：ビデオが既にAdobe Dynamic Media Classicの外部でエンコードされている場合は、グローバルナビゲーションバーで「」を選択します **[!UICONTROL Upload]**. MP4 ビデオファイルを参照してAdobe Dynamic Media Classicに直接アップロードします。 次に、に移動します **[!UICONTROL ビルド]** > **[!UICONTROL アダプティブビデオセット]**. ビデオファイルを参照します。目的のビデオファイルをアダプティブビデオセット テーブルにドラッグ&amp;ドロップし、セットを保存します。
* **プライマリソースビデオのアップロード**：ビデオがエンコードされていない場合は、グローバルナビゲーションバーでを選択します **[!UICONTROL Upload]** （MP4 以外の）プライマリビデオソースファイルをアップロードします。 Adobe Dynamic Media Classicは、それらを MP4 ファイルにエンコードします。 が含まれる **[!UICONTROL アップロードジョブオプション]** ダイアログ ボックスの下 **[!UICONTROL ビデオ オプション]**&#x200B;を選択 **[!UICONTROL アダプティブビデオ]**.

  この推奨オプションを使用すると、アダプティブビデオセットを作成できます。 アップロードしたビデオのサイズに合わせて、適切なエンコーディングプリセットが（16:9 と 4:3 のどちらでも）ビデオに自動的に適用されます。 アップロードジョブを送信すると、3 つのエンコーディングビデオ設定が正しい縦横比で含まれるアダプティブビデオセットが自動的に作成されます。

  同様に **[!UICONTROL ジョブオプション]** ダイアログ ボックスの下 **[!UICONTROL ビデオ オプション]**、を展開 **[!UICONTROL 単一エンコーディングプリセット]**. 目的のビデオエンコーディングプリセットを個別に選択します。 以下を選択できます。 **デスクトップ**, **モバイル （iPhone、iPad、Android™）**、および **Tablet （iPad、Android™）** mp4 ファイルを作成します。

* または、プライマリビデオの再処理に使用できます **[!UICONTROL 再処理]** 機能 新しくエンコードされたビデオは、既存のアダプティブビデオセットに追加されます。

参照： [ビデオのアップロードとエンコード](uploading-encoding-videos.md#uploading_and_encoding_videos).

**オプション**

Adobe Dynamic Media Classicには、事前定義済みのビデオエンコーディングプリセットが多数用意されています。 これらの事前定義済みプリセットは、現在使用されている最も一般的なビデオエンコーディング設定を反映しており、ターゲットページでの再生用に最適化されています。

ただし、さらにカスタマイズする必要がある場合は、管理者はビデオプリセットを作成して、エンドユーザー向けのビデオのサイズと再生操作をカスタマイズすることもできます。管理者は、のビデオプリセットページでビデオプリセットを追加および管理できます。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビデオプリセット]** > **[!UICONTROL 単一エンコーディングプリセット]**. ビデオプリセットページには、ビデオプリセットの追加、編集、削除およびアクティブ化を行うオプションがあります。

参照： [ビデオエンコーディングプリセットの操作](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2. ビデオビューアでビデオをプレビューする

デスクトップ、Web サイトまたはモバイルデバイスでのエンドユーザーに対するビデオの再生方法を確認するには、参照パネルでビデオを選択します。 次に、を選択します **[!UICONTROL プレビュー]**.

参照： [ビデオビューアでビデオをプレビューする](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

プレビューページでビデオを再生できます。 また、様々なビデオビューアを選択して、様々なプレーヤーでのビデオの表示方法を確認することもできます。 ベストプラクティスとして、デスクトップ、タブレットおよび携帯端末でのマルチ画面再生には HTML5 ビデオプレーヤーを使用します。

**オプション**

ビューアプリセットのカスタマイズ：Adobe Dynamic Media Classicには、ビデオを配信するための事前定義済みのビューアプリセットが用意されています。 これらのプリセットは、ビューアの外観と、その再生コントロールの動作を決定します。管理者はビデオビューアをカスタマイズするために、ビューアプリセットページでビューアプリセットを追加および管理することができます。このページを開くには、Adobe Dynamic Media Classicの右上隅にあるに移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**. ビューアプリセットページには、ビューアプリセットの追加、編集、削除およびアクティブ化を行うコマンドがあります。

参照： [ビデオビューアプリセットの操作](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

## 3. Web サイトやモバイルサイトにビデオをデプロイする

ビデオを Web サイトに統合するには、次のいずれかの操作を行います。

* ビデオを独自のポップアップウィンドウまたはモーダルウィンドウで表示します。この場合は、 **[!UICONTROL URL をコピー]** 機能

  ビデオの URL を取得するには、グリッド表示またはリスト表示で、参照パネルでビデオを選択します。 を選択 **[!UICONTROL プレビュー]**&#x200B;を選択してから、 **[!UICONTROL URL をコピー]** ～の右側に `Universal_HTML5_Viewer`.

  選択した場合 **[!UICONTROL URL をコピー]** URL がクリップボードにコピーされます。 Web サイト、モバイルサイトまたはアプリケーションの HTML にこのコードを設定します。

  >[!NOTE]
  >
  >URL はビデオまたはアダプティブビデオセットを公開するまでアクティブになりません。

* Web ページに埋め込まれたビデオを表示します。この場合、を使用します **[!UICONTROL 埋め込みコード]** 機能

  ビデオの埋め込みコードを取得するには、グリッド表示またはリスト表示で、参照パネルのビデオを選択します。 に移動 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**. テーブルの「アクション」列で、次の項目を選択します **[!UICONTROL 埋め込みコード]** ～の右側に `Universal_HTML5_Video`. コードの編集はできません。

  を選択 **[!UICONTROL 閉じる]** 次に、埋め込みコードを 1 つ以上の web ページに貼り付けます。

  >[!NOTE]
  >
  >埋め込みコードは、ビデオまたはアダプティブビデオセットを公開した後でのみアクティブ化されます。

参照： [Web サイトやモバイルサイトにビデオをデプロイします](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)
