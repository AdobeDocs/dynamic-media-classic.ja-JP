---
title: 「クイックスタート：Adobe Dynamic Media Classicのビデオ»
description: すばやく使い始めるのに役立つ、概要とAdobe Dynamic Media Classicのクイックスタートビデオです。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1808'
ht-degree: 25%

---

# クイックスタート：Adobe Dynamic Media Classicのビデオ{#quick-start-video}

Adobe Dynamic Media Classicビデオは、デスクトップ、iOS、Android™、BlackBerry®、Windows®モバイルデバイスなど、複数の画面にストリーミング用の高品質なアダプティブビデオを簡単に公開できるエンドツーエンドのソリューションです。 アダプティブビデオセットは、同じビデオを異なるビットレート（400 kbps、800 kbps および 1000 kbps）やフォーマットでエンコードしたバージョンをグループ化します。デスクトップコンピュータまたは携帯端末は、使用可能な帯域幅を検出します。

例えば、iOS の携帯端末では、3G、4G または Wi-Fi などの帯域幅を検出します。それに基づき、アダプティブビデオセットに含まれる各種ビデオビットレートの中から適切にエンコードされたビデオを自動的に選択します。ビデオはデスクトップ、携帯端末またはタブレットにストリーミングされます。

さらに、デスクトップまたは携帯端末上でネットワークの状態が変化した場合は、ビデオ画質が自動的に動的に切り替わります。また、顧客がデスクトップでフルスクリーンモードに移行した場合、アダプティブビデオセットはより高い解像度を使用して応答し、顧客の表示エクスペリエンスが向上します。 アダプティブビデオセットを使用すると、複数の画面やデバイスでAdobe Dynamic Media Classicビデオを再生する場合に、できる限り最高の再生をおこなうことができます。

どのエンコードされたビデオを再生するか決定したり、どのエンコードされたビデオを再生中に選択するか決定するためにビデオプレーヤーが使用するロジックは、次のアルゴリズムに基づいています。

1. ビデオプレーヤーは、プレーヤー自体の「初期ビットレート」に設定されている値に最も近いビットレートに基づいて、初期ビデオフラグメントを読み込みます。
1. 次の条件を使用して、帯域幅の速度に対する変更に基づいてビデオプレーヤーが切り替わります。

   1. プレーヤーは、推定帯域幅以下の最大帯域幅ストリームを選択します。
   1. プレーヤーは、使用可能な帯域幅の 80%のみを考慮します。 ただし、上に切り替える場合は、帯域幅を大きく見積もりすぎず、すぐに元の帯域幅に戻す必要があるのを防ぐため、より控えめな 70%の見積もりです。

アルゴリズムのロジックについては、 [https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) 」を参照してください。

単一のビデオおよびアダプティブビデオセットの管理で、Adobe Dynamic Media Classicは次の機能をサポートしています。

* 多数のサポートされているビデオ形式およびオーディオ形式からビデオをアップロードし、複数の画面で再生するためにビデオを MP4 H.264 形式にエンコーディングします。 事前定義済みのAdobe Dynamic Media Classicアダプティブビデオプリセット、単一のビデオエンコーディングプリセットを使用するか、独自のエンコーディングをカスタマイズして、ビデオの品質とサイズを制御することができます。

詳しくは、 [アダプティブビデオプリセットのアクティベートとアクティベート解除](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets)

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

アダプティブビデオセットが生成されると、MP4 ビデオが含まれます。

>[!NOTE]
>
>プライマリ/ソースビデオおよびその他のソース形式のビデオは、 *not* をアダプティブビデオセットに追加しました。

* Universal_Video、Universal_Caption5_Video、Universal_Media5_MixedMedia_dark、Universal_Chapter_Video、Universal_Chapter5_MixedMedia_dark、Universal_HTML5_MixedMedia_MediaVidea でのビューアおよびビデオHTMLナビゲーションライトビューア

   詳しくは、 [ビデオにキャプションを追加](adding-captions-video.md).

   詳しくは、 [ビデオへのチャプターマーカーの追加](adding-chapter-markers-video.md).

* 完全なメタデータサポートにより、ビデオを整理、参照および検索して、ビデオアセットの効率的な管理を実現します。
* Web およびデスクトップおよびモバイルデバイス (iPhone、iPad、Android™、BlackBerry®、Windows®電話を含む ) にアダプティブビデオセットを配信します。

   アダプティブビデオのストリーミングは、様々なiOSプラットフォームでサポートされています。

   最新のサポートについては、 [Adobeビューアリファレンスガイド](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html).

   Adobe Dynamic Media Classicは、MP4 H.264 ビデオのモバイルビデオ再生をサポートしています。 このビデオ形式をサポートする BlackBerry®デバイスは、次の Web サイトで確認できます。

   詳しくは、 [BlackBerry®でサポートされるビデオ形式](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482).

   このビデオ形式をサポートする Windows®デバイスは、次の場所にあります。

   詳しくは、 [Windows® Phone でサポートされるビデオ形式](https://docs.microsoft.com/en-us/).

* 以下を含むAdobe Dynamic Media Classicビューアプリセットを使用してビデオを再生します。

   * 単一のビデオビューア。
   * ビデオコンテンツと画像コンテンツの両方を組み合わせた混在メディアビューア。

* ブランドニーズに合わせてビデオプレーヤーを設定します。
* 簡素な URL または埋め込みコードを使用して、ビデオを Web サイト、モバイルサイトまたはモバイルアプリケーションに統合します。

次のトレーニングビデオを参照してください。
* [MP4 ビデオの概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/563_MP4%20Video%20Overview_converted%20renamed_eVideos-AVS)

* [MP4 ビデオプレビュー](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/564_MP4%20Video%20Preview_converted%20renamed_eVideos-AVS)

* [MP4 ビデオのアップロード](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/565_MP4%20Video%20Upload_converted%20renamed_eVideos-AVS)

* [ストリーミングの概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/567_Streaming%20Overview_master_eVideos_converted%20renamed_eVideos-AVS)

**クイックスタート**

次のワークフローの手順説明は、Adobe Dynamic Media Classicのアダプティブビデオセットをすぐに使い始めるためのものです。 各手順の後に、トピックの見出しへの相互参照があり、詳細を確認できます。

## 1.ビデオのアップロードとエンコード

次の 2 つのシナリオのうちいずれかを使用して、アダプティブビデオセットをアップロードおよび生成します。

* **エンコード済みビデオのアップロード**  — ビデオが既にAdobe Dynamic Media Classicの外部でエンコードされている場合は、グローバルナビゲーションバーで、 **[!UICONTROL アップロード]** : MP4 ビデオファイルを参照し、Adobe Dynamic Media Classicに直接アップロードします。 次に、に移動します。 **[!UICONTROL ビルド]** > **[!UICONTROL アダプティブビデオセット]**. ビデオファイルを参照します。目的のビデオファイルを「アダプティブビデオセット」テーブルにドラッグ&amp;ドロップし、セットを保存します。
* **プライマリソースビデオのアップロード**  — ビデオがエンコードされていない場合は、グローバルナビゲーションバーで、 **[!UICONTROL アップロード]** プライマリビデオソースファイル（MP4 以外）をアップロードする場合。 Adobe Dynamic Media Classicによって MP4 ファイルにエンコードされます。 内 **[!UICONTROL アップロードジョブオプション]** ダイアログボックスの下 **[!UICONTROL eVideo オプション]**&#x200B;を選択します。 **[!UICONTROL アダプティブビデオ]**.

   これは推奨されているオプションで、アップロードしたビデオのサイズに合わせて、ビデオに適切なエンコーディングプリセット（16:9 または 4:3）を自動的に適用するアダプティブビデオセットを作成できます。アップロードジョブを送信すると、アダプティブビデオセットが自動的に作成されます。この中には、正しい縦横比の 3 つのエンコードビデオ設定が含まれています。

   または、同じ **[!UICONTROL ジョブオプション]** ダイアログボックスの下 **[!UICONTROL eVideo オプション]**、展開 **[!UICONTROL 単一のエンコーディングプリセット]**.使用する個々のビデオエンコーディングプリセットを選択します。 **デスクトップ**, **モバイル (iPhone、iPad、Android™)**、および **タブレット (iPad、Android™)** MP4 ファイルを作成できます。

* または、 **[!UICONTROL 再処理]** 機能。 新しくエンコードされたビデオは、既存のアダプティブビデオセットに追加されます。

詳しくは、 [ビデオのアップロードとエンコード](uploading-encoding-videos.md#uploading_and_encoding_videos).

**オプション**

Adobe Dynamic Media Classicには、多数の定義済みのビデオエンコーディングプリセットが用意されています。 これらの事前定義済みプリセットは、現在使用されている最も一般的なビデオエンコーディング設定を反映し、ターゲットページでの再生用に最適化されています。

ただし、さらにカスタマイズする必要がある場合は、管理者はビデオプリセットを作成して、エンドユーザー向けのビデオのサイズと再生操作をカスタマイズすることもできます。管理者は、以下にあるビデオプリセットページでビデオプリセットの追加と管理をおこなうことができます。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビデオプリセット]** > **[!UICONTROL 単一のエンコーディングプリセット]**. ビデオプリセットページには、ビデオプリセットの追加、編集、削除およびアクティブ化を行うオプションがあります。

詳しくは、 [ビデオエンコーディングプリセットの操作](uploading-encoding-videos.md#working_with_video_encoding_presets).

## 2.ビデオビューアでビデオをプレビューする

デスクトップ、Web サイト、モバイルデバイスでエンドユーザーに対してビデオが再生される様子を確認するには、参照パネルでビデオを選択し、「 **[!UICONTROL プレビュー]**.

詳しくは、 [ビデオビューアでビデオをプレビューする](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer).

ビデオはプレビューページで再生できます。 また、様々なビデオビューアを選択して、ビデオが様々なプレーヤーでどのように表示されるかを調べることもできます。 ベストプラクティスとして、デスクトップ、タブレットおよび携帯端末でのマルチ画面再生には HTML5 ビデオプレーヤーを使用します。

**オプション**

ビューアプリセットのカスタマイズ — Adobe Dynamic Media Classicには、ビデオを配信するための事前定義済みのビューアプリセットが用意されています。 これらのプリセットは、ビューアの外観と、その再生コントロールの動作を決定します。管理者はビデオビューアをカスタマイズするために、ビューアプリセットページでビューアプリセットを追加および管理することができます。このページを開くには、Adobe Dynamic Media Classicの右上隅にあるに移動します。 **[!UICONTROL 設定]** > **[!UICONTROL ビューアプリセット]**. ビューアプリセットページには、ビューアプリセットの追加、編集、削除およびアクティブ化を行うコマンドがあります。

詳しくは、 [ビデオビューアプリセットの操作](previewing-videos-video-viewer.md#working_with_video_viewer_presets).

関連トピック [ビデオプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

## 3. Web サイトやモバイルサイトにビデオをデプロイする

ビデオを Web サイトに統合するには、次のいずれかの操作を行います。

* ビデオを独自のポップアップウィンドウまたはモーダルウィンドウで表示します ( この場合、 **[!UICONTROL URL をコピー]** 機能。

   ビデオの URL を取得するには、グリッドビューまたはリストビューの参照パネルでビデオを選択します。選択 **[!UICONTROL プレビュー]**&#x200B;を選択し、 **[!UICONTROL URL をコピー]** 右に `Universal_HTML5_Viewer`.

   次を選択した場合： **[!UICONTROL URL をコピー]**&#x200B;の場合、URL はクリップボードにコピーされます。 Web サイト、モバイルサイトまたはアプリケーションの HTML にこのコードを設定します。

   >[!NOTE]
   >
   >URL はビデオまたはアダプティブビデオセットを公開するまでアクティブになりません。

* Web ページに埋め込まれたビデオを表示します ( この場合、 **[!UICONTROL 埋め込みコード]** 機能。

   ビデオの埋め込みコードを取得するには、グリッドビューまたはリストビューの参照パネルでビデオを選択します。に移動します。 **[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**. テーブルの「アクション」列で、「 **[!UICONTROL 埋め込みコード]** 右に `Universal_HTML5_Video`. コードの編集はできません。

   選択 **[!UICONTROL 閉じる]** 埋め込みコードを web ページに貼り付けます。

   >[!NOTE]
   >
   >埋め込みコードはビデオまたはアダプティブビデオセットを公開するまでアクティブになりません。

詳しくは、 [Web サイトやモバイルサイトにビデオをデプロイする](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites).

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)

