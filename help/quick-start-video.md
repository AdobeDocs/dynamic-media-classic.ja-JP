---
title: 「クイックスタート：Adobe Dynamic Media Classicのビデオ»
description: すばやく使い始めるのに役立つ、Adobe Dynamic Media Classicの概要およびクイックスタートビデオです。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: 352b1c383195fa03294ad3501207d63f3cfe3e42
workflow-type: tm+mt
source-wordcount: '1806'
ht-degree: 28%

---

# クイックスタート：Adobe Dynamic Media Classicのビデオ{#quick-start-video}

Adobe Dynamic Media Classicビデオは、デスクトップ、iOS、Android™、BlackBerry®、Windows®モバイルデバイスなど、複数の画面にストリーミング用の高品質なアダプティブビデオを簡単に公開できるエンドツーエンドのソリューションです。 アダプティブビデオセットは、同じビデオを異なるビットレート（400 kbps、800 kbps および 1000 kbps）やフォーマットでエンコードしたバージョンをグループ化します。デスクトップコンピュータまたは携帯端末は、使用可能な帯域幅を検出します。

例えば、iOS の携帯端末では、3G、4G または Wi-Fi などの帯域幅を検出します。それに基づき、アダプティブビデオセットに含まれる各種ビデオビットレートの中から適切にエンコードされたビデオを自動的に選択します。ビデオはデスクトップ、携帯端末またはタブレットにストリーミングされます。

さらに、デスクトップまたは携帯端末上でネットワークの状態が変化した場合は、ビデオ画質が自動的に動的に切り替わります。また、顧客がデスクトップでフルスクリーンモードに切り替えると、アダプティブビデオセットはより高い解像度を使用して応答し、顧客の表示エクスペリエンスが向上します。 アダプティブビデオセットを使用すると、複数の画面やデバイスでAdobe Dynamic Media Classicビデオを再生するお客様に最高の再生を提供できます。

どのエンコードされたビデオを再生するか決定したり、どのエンコードされたビデオを再生中に選択するか決定するためにビデオプレーヤーが使用するロジックは、次のアルゴリズムに基づいています。

1. ビデオプレーヤーは、プレーヤー自体の「初期ビットレート」に設定された値に最も近いビットレートに基づいて、初期ビデオフラグメントを読み込みます。
1. 次の条件を使用して、帯域幅速度の変更に基づいてビデオプレーヤーが切り替わります。

   1. プレーヤーは、推定帯域幅以下で最も高い帯域幅ストリームを選択します。
   1. プレーヤーは、使用可能な帯域幅の 80%しか考慮しません。 ただし、上に切り替える場合は、帯域幅を大きく見積もりすぎず、すぐに元の帯域幅に戻す必要があるので、より控えめな 70%程度です。

技術的な情報については、[https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp) にあるアルゴリズムのロジックを参照してください。

単一のビデオとアダプティブビデオセットの管理に関して、Adobe Dynamic Media Classicでは次の機能をサポートしています。

* 多数あるサポート対象のビデオ形式およびオーディオ形式のビデオを、複数の画面で再生できる MP4 H.264 形式でアップロードします。事前定義済みのAdobe Dynamic Media Classicアダプティブビデオプリセット、単一のビデオエンコーディングプリセットを使用するか、独自のエンコーディングをカスタマイズしてビデオの品質とサイズを制御することができます。

[ アダプティブビデオプリセットのアクティベートとアクティベート解除 ](/help/application-setup.md#activating-or-deactivating-adaptive-video-presets) を参照してください。

[ ビデオプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) のトレーニングビデオも参照してください。

アダプティブビデオセットが生成されると、MP4 ビデオが含まれます。

>[!NOTE]
>
>マスター/ソースビデオおよびその他のソース形式のビデオは、アダプティブビデオセットに *追加されません*。

* Universal_Video5_Video、Universal_Commedia5_MixedMedia_dark、Universal_Media_light ビューアおよび Universal_Video5_Video、Universal_MixedMedia_dark、Universal_HTML5_MixedMedia_Media_Vidia のビデオHTMLとビデオHTMLライトビューア

   [ ビデオにキャプションを追加する ](adding-captions-video.md) を参照してください。

   [ ビデオへのチャプターマーカーの追加 ](adding-chapter-markers-video.md) を参照してください。

* 完全なメタデータサポートにより、ビデオを整理、参照および検索して、ビデオアセットの効率的な管理を実現します。
* Web およびデスクトップおよびモバイルデバイス (iPhone、iPad、Android™、BlackBerry®、Windows® Phone など ) へのアダプティブビデオセットの配信

   アダプティブビデオのストリーミングは、様々なiOSプラットフォームでサポートされています。

   『[Adobeビューアリファレンスガイド ](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html)』の最新のサポートを参照してください。

   Adobe Dynamic Media Classicは、MP4 H.264 ビデオのモバイルビデオ再生をサポートしています。 このビデオ形式をサポートする BlackBerry®デバイスは、次の Web サイトにあります。

   [BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482) でサポートされているビデオ形式を参照してください。

   このビデオ形式をサポートする Windows®デバイスは、次の場所にあります。

   [Windows® Phone でサポートされているビデオ形式 ](https://docs.microsoft.com/en-us/) を参照してください。

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

次のワークフローの手順説明は、Adobe Dynamic Media Classicのアダプティブビデオセットをすばやく使い始めるためのものです。 各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

## 1.ビデオのアップロードとエンコード

次の 2 つのシナリオのうちいずれかを使用して、アダプティブビデオセットをアップロードおよび生成します。

* **事前エンコードされたビデオのアップロード**  — ビデオが既にAdobe Dynamic Media Classicの外部でエンコードされている場合、グローバルナビゲーションバーの「アップロード」を選択し **** て、MP4 ビデオファイルを参照してAdobe Dynamic Media Classicに直接アップロードします。次に、**[!UICONTROL ビルド]** / **[!UICONTROL アダプティブビデオセット]** に移動します。 ビデオファイルを参照します。目的のビデオファイルを「アダプティブビデオセット」テーブルにドラッグアンドドロップし、セットを保存します。
* **マスターソースビデオのアップロード**  — ビデオがエンコードされていない場合、グローバルナビゲーションバーの「アップロード」を選択して、マスタービデオソースファイル（MP4 以外）をアップロードしま **** す。Adobe Dynamic Media Classicによって MP4 ファイルにエンコードされます。 **[!UICONTROL アップロードオプション]** ダイアログボックスの **[!UICONTROL 「EVideo オプション]**」で、「**[!UICONTROL アダプティブビデオ]**」を選択します。

   これは推奨されているオプションで、アップロードしたビデオのサイズに合わせて、ビデオに適切なエンコーディングプリセット（16:9 または 4:3）を自動的に適用するアダプティブビデオセットを作成できます。アップロードジョブを送信すると、アダプティブビデオセットが自動的に作成されます。この中には、正しい縦横比の 3 つのエンコードビデオ設定が含まれています。

   または、同じ **[!UICONTROL ジョブオプション]** ダイアログボックスの **[!UICONTROL 「EVideo オプション]**」で、「**[!UICONTROL 単一エンコーディングプリセット]**」を展開します。MP4 ファイルを作成するために、 **デスクトップ**、 **モバイル (iPhone、iPad、Android™)**、 **タブレット (iPad、Android™)** から、必要な個々のビデオエンコーディングプリセットを選択します。

* または、**[!UICONTROL 再処理]** 機能を使用して、マスタービデオを再処理できます。 新しくエンコードされたビデオは、既存のアダプティブビデオセットに追加されます。

[ ビデオのアップロードとエンコード ](uploading-encoding-videos.md#uploading_and_encoding_videos) を参照してください。

**オプション**

Adobe Dynamic Media Classicでは、定義済みのビデオエンコーディングプリセットが多数用意されています。 これらの事前定義済みプリセットは、現在使用されている最も一般的なビデオエンコーディング設定を反映し、ターゲットページでの再生用に最適化されています。

ただし、さらにカスタマイズする必要がある場合は、管理者はビデオプリセットを作成して、エンドユーザー向けのビデオのサイズと再生操作をカスタマイズすることもできます。管理者は、 **[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL ビデオプリセット]** / **[!UICONTROL 単一エンコーディングプリセット]** で利用できるビデオプリセットページでビデオプリセットを追加および管理できます。 ビデオプリセットページには、ビデオプリセットの追加、編集、削除およびアクティブ化を行うオプションがあります。

[ ビデオエンコーディングプリセットの操作 ](uploading-encoding-videos.md#working_with_video_encoding_presets) を参照してください。

## 2.ビデオビューアでビデオをプレビューする

デスクトップ、Web サイトまたはモバイルデバイスでエンドユーザーに対してビデオが再生される様子を確認するには、参照パネルでビデオを選択し、「**[!UICONTROL プレビュー]**」を選択します。

[ ビデオビューアでのビデオのプレビュー ](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer) を参照してください。

ビデオはプレビューページで再生できます。 また、様々なビデオビューアを選択して、様々なプレーヤーでのビデオの表示方法を確認できます。 ベストプラクティスとして、デスクトップ、タブレットおよび携帯端末でのマルチ画面再生には HTML5 ビデオプレーヤーを使用します。

**オプション**

ビューアプリセットのカスタマイズ — Adobe Dynamic Media Classicには、ビデオを配信するための事前定義済みのビューアプリセットが用意されています。 これらのプリセットは、ビューアの外観と、その再生コントロールの動作を決定します。管理者はビデオビューアをカスタマイズするために、ビューアプリセットページでビューアプリセットを追加および管理することができます。このページを開くには、Adobe Dynamic Media Classicの右上隅にある **[!UICONTROL 設定]** / **[!UICONTROL ビューアプリセット]** に移動します。 ビューアプリセットページには、ビューアプリセットの追加、編集、削除およびアクティブ化を行うコマンドがあります。

[ ビデオビューアプリセットの操作 ](previewing-videos-video-viewer.md#working_with_video_viewer_presets) を参照してください。

[ ビデオプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/549_video-presets_converted%20renamed_Done-AVS) のトレーニングビデオも参照してください。

## 3. Web サイトやモバイルサイトにビデオをデプロイする

ビデオを Web サイトに統合するには、次のいずれかの操作を行います。

* 独自のポップアップウィンドウまたはモーダルウィンドウでビデオを表示します。その場合は、**[!UICONTROL URL をコピー]** 機能を使用します。

   ビデオの URL を取得するには、グリッドビューまたはリストビューの参照パネルでビデオを選択します。「**[!UICONTROL プレビュー]**」を選択し、「`Universal_HTML5_Viewer`」の右側にある「**[!UICONTROL URL をコピー]**」を選択します。

   「**[!UICONTROL URL をコピー]**」を選択すると、URL がクリップボードにコピーされます。 Web サイト、モバイルサイトまたはアプリケーションの HTML にこのコードを設定します。

   >[!NOTE]
   >
   >URL はビデオまたはアダプティブビデオセットを公開するまでアクティブになりません。

* Web ページに埋め込まれたビデオを表示します。この場合は、**[!UICONTROL 埋め込みコード]** 機能を使用します。

   ビデオの埋め込みコードを取得するには、グリッドビューまたはリストビューの参照パネルでビデオを選択します。**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]** に移動します。 表の「アクション」列で、「`Universal_HTML5_Video`」の右にある「**[!UICONTROL 埋め込みコード]**」を選択します。 コードの編集はできません。

   「**[!UICONTROL 閉じる]**」を選択し、埋め込みコードを Web ページに貼り付けます。

   >[!NOTE]
   >
   >埋め込みコードはビデオまたはアダプティブビデオセットを公開するまでアクティブになりません。

[Web サイトおよびモバイルサイトへのビデオのデプロイ ](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites) を参照してください。

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)

