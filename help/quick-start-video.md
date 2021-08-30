---
title: 「クイックスタート：Dynamic Media ClassicAdobeのビデオ»
description: Dynamic Media Classicの概要とAdobeのクイックスタートビデオを参照してください。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: 1157400c-b33a-422e-848c-258660ddc748
source-git-commit: 36f9aa3c2b4dc66e4cb851c2ce6837ae0ad4f64c
workflow-type: tm+mt
source-wordcount: '1444'
ht-degree: 35%

---

# クイックスタート：Dynamic Media ClassicAdobeのビデオ{#quick-start-video}

AdobeDynamic Media Classic Videoは、デスクトップ、iOS、Android™、BlackBerry®、Windows®の各モバイルデバイスを含む複数の画面にストリーミング用の高品質なアダプティブビデオを簡単に公開できるエンドツーエンドのソリューションです。 アダプティブビデオセットは、同じビデオを異なるビットレート（400 kbps、800 kbps および 1000 kbps）やフォーマットでエンコードしたバージョンをグループ化します。デスクトップコンピュータまたは携帯端末は、使用可能な帯域幅を検出します。

例えば、iOS の携帯端末では、3G、4G または Wi-Fi などの帯域幅を検出します。それに基づき、アダプティブビデオセットに含まれる各種ビデオビットレートの中から適切にエンコードされたビデオを自動的に選択します。ビデオはデスクトップ、携帯端末またはタブレットにストリーミングされます。

さらに、デスクトップまたは携帯端末上でネットワークの状態が変化した場合は、ビデオ画質が自動的に動的に切り替わります。また、顧客がデスクトップでフルスクリーンモードに切り替えると、アダプティブビデオセットはより高い解像度を使用して応答し、顧客の表示エクスペリエンスが向上します。 アダプティブビデオセットを使用すると、複数の画面やデバイスでAdobeDynamic Media Classicビデオを再生するお客様に最適な再生が可能になります。

どのエンコードされたビデオを再生するか決定したり、どのエンコードされたビデオを再生中に選択するか決定するためにビデオプレーヤーが使用するロジックは、次のアルゴリズムに基づいています。

1. ビデオプレーヤーは、プレーヤー自体の「初期ビットレート」に設定された値に最も近いビットレートに基づいて、初期ビデオフラグメントを読み込みます。
1. ビデオプレーヤーは、次の条件を使用して、帯域幅の速度に対する変更に基づいて切り替えます。

   1. プレーヤーは、推定帯域幅以下で最も高い帯域幅ストリームを選択します。
   1. プレーヤーは、使用可能な帯域幅の80%しか考慮しません。 ただし、上に切り替える場合は、帯域幅を大きく見積もりすぎず、すぐに元に戻す必要があるので、より控えめな70%の見積もりです。

技術情報については、[https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp](https://android.googlesource.com/platform/frameworks/av/+/master/media/libstagefright/httplive/LiveSession.cpp)にあるアルゴリズムのロジックを参照してください。

単一のビデオおよびアダプティブビデオセットの管理に関して、AdobeDynamic Media Classicでは次の機能をサポートしています。

* 多数あるサポート対象のビデオ形式およびオーディオ形式のビデオを、複数の画面で再生できる MP4 H.264 形式でアップロードします。定義済みAdobeのDynamic Media Classicアダプティブビデオプリセット、単一のビデオエンコーディングプリセットを使用するか、独自のエンコーディングをカスタマイズしてビデオの品質とサイズを制御することができます。

   アダプティブビデオセットが生成されると、MP4ビデオが含まれます。

   >[!NOTE]
   >
   >マスター/ソースビデオおよびその他のソース形式のビデオは、アダプティブビデオセットに&#x200B;*追加されません*。

* Universal_HTML5_Video、Universal_HTML5_MixedMedia_darkおよびUniversal_HTML5_MixedMedia_lightビューアとUniversal_HTML5_MixedMedia_darkおよびUniversal_HTML5_MixedMedia_Mediaのビデオチャプトナビゲーションライトビューア

   [ビデオにキャプションを追加する](adding-captions-video.md)を参照してください。

   [ビデオへのチャプターマーカーの追加](adding-chapter-markers-video.md)を参照してください。

* 完全なメタデータサポートにより、ビデオを整理、参照および検索して、ビデオアセットの効率的な管理を実現します。
* アダプティブビデオセットをWebやデスクトップ、およびiPhone、iPad、Android™、BlackBerry®、Windows® Phoneなどのモバイルデバイスに配信します。

   アダプティブビデオのストリーミングは、様々なiOSプラットフォームでサポートされています。

   『[Adobeビューアリファレンスガイド](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources.html)』の最新のサポートを参照してください。

   AdobeDynamic Media Classicは、MP4 H.264ビデオのモバイルビデオ再生をサポートしています。 このビデオ形式をサポートするBlackBerry®デバイスは、次のWebサイトで確認できます。

   [BlackBerry®](https://support.blackberry.com/kb/articleDetail?ArticleNumber=000005482)でサポートされているビデオ形式を参照してください。

   このビデオ形式をサポートするWindows®デバイスは、次の場所にあります。

   [Windows® Phoneでサポートされているビデオ形式](https://docs.microsoft.com/en-us/)を参照してください。

* 以下を含むAdobeDynamic Media Classicビューアプリセットを使用してビデオを再生します。

   * 単一のビデオビューア。
   * ビデオコンテンツと画像コンテンツの両方を組み合わせた混在メディアビューア。

* ブランドニーズに合わせてビデオプレーヤーを設定します。
* 簡素な URL または埋め込みコードを使用して、ビデオを Web サイト、モバイルサイトまたはモバイルアプリケーションに統合します。

**クイックスタート**

次のワークフローの手順説明は、AdobeDynamic Media Classicのアダプティブビデオセットをすばやく使い始めるためのものです。 各手順の最後に、それぞれの内容について詳しく説明している見出しの参照先を示しています。

## 1.ビデオのアップロードとエンコード

次の 2 つのシナリオのうちいずれかを使用して、アダプティブビデオセットをアップロードおよび生成します。

* **事前エンコードされたビデオのアップロード**  — ビデオが既にAdobeDynamic Media Classicの外部でエンコードされている場合、グローバルナビゲーションバーの「アップロード」を選択し **** て、MP4ビデオファイルを参照し、AdobeDynamic Media Classicに直接アップロードします。次に、**[!UICONTROL ビルド]** / **[!UICONTROL アダプティブビデオセット]**&#x200B;に移動します。 ビデオファイルを参照します。目的のビデオファイルを「アダプティブビデオセット」テーブルにドラッグアンドドロップし、セットを保存します。
* **マスターソースビデオのアップロード**  — ビデオがエンコードされていない場合、グローバルナビゲーションバーの「アップロード」を選択し **** て、マスタービデオソースファイル（MP4以外）をアップロードします。AdobeDynamic Media Classicは、それらをMP4ファイルにエンコードします。 **[!UICONTROL アップロードオプション]**&#x200B;ダイアログボックスの「**[!UICONTROL EVideoオプション]**」で、「**[!UICONTROL アダプティブビデオ]**」を選択します。

   これは推奨されているオプションで、アップロードしたビデオのサイズに合わせて、ビデオに適切なエンコーディングプリセット（16:9 または 4:3）を自動的に適用するアダプティブビデオセットを作成できます。アップロードジョブを送信すると、アダプティブビデオセットが自動的に作成されます。このセットには、正しい縦横比の3つのエンコードビデオ設定が含まれています。

   または、同じ&#x200B;**[!UICONTROL ジョブオプション]**&#x200B;ダイアログボックスの「**[!UICONTROL EVideoオプション]**」で、「**[!UICONTROL 単一エンコーディングプリセット]**」を展開します。MP4ファイルを作成するために、 **デスクトップ**、 **モバイル(iPhone、iPad、Android™)**&#x200B;および&#x200B;**タブレット(iPad、Android™)**&#x200B;から、必要な個々のビデオエンコーディングプリセットを選択します。

* または、**[!UICONTROL 再処理]**&#x200B;機能を使用して、マスタービデオを再処理することもできます。 新しくエンコードされたビデオは、既存のアダプティブビデオセットに追加されます。

[ビデオのアップロードとエンコード](uploading-encoding-videos.md#uploading_and_encoding_videos)を参照してください。

**オプション**

AdobeDynamic Media Classicでは、定義済みのビデオエンコーディングプリセットを多数用意しています。 これらの事前定義済みプリセットは、現在使用されている最も一般的なビデオエンコーディング設定を反映し、ターゲットページでの再生用に最適化されています。

ただし、さらにカスタマイズする必要がある場合は、管理者はビデオプリセットを作成して、エンドユーザー向けのビデオのサイズと再生操作をカスタマイズすることもできます。管理者は、 **[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL ビデオプリセット]** / **[!UICONTROL 単一のエンコーディングプリセット]**&#x200B;で利用できるビデオプリセットページでビデオプリセットを追加および管理できます。 ビデオプリセットページには、ビデオプリセットの追加、編集、削除およびアクティブ化を行うオプションがあります。

[ビデオエンコーディングプリセットの操作](uploading-encoding-videos.md#working_with_video_encoding_presets)を参照してください。

## 2.ビデオビューアでビデオをプレビューする

デスクトップ、Webサイトまたはモバイルデバイスでエンドユーザーがビデオを再生する方法を確認するには、参照パネルでビデオを選択し、「**[!UICONTROL プレビュー]**」を選択します。

[ビデオビューアでのビデオのプレビュー](previewing-videos-video-viewer.md#previewing_videos_in_a_video_viewer)を参照してください。

ビデオはプレビューページで再生できます。 また、異なるビデオビューアを選択して、異なるプレーヤーでのビデオの表示方法を確認することもできます。 ベストプラクティスとして、デスクトップ、タブレットおよび携帯端末でのマルチ画面再生には HTML5 ビデオプレーヤーを使用します。

**オプション**

ビューアプリセットのカスタマイズ —AdobeDynamic Media Classicには、ビデオを配信するための定義済みのビューアプリセットが用意されています。 これらのプリセットは、ビューアの外観と、その再生コントロールの動作を決定します。管理者はビデオビューアをカスタマイズするために、ビューアプリセットページでビューアプリセットを追加および管理することができます。このページを開くには、AdobeDynamic Media Classicの右上隅にある&#x200B;**[!UICONTROL 設定]** / **[!UICONTROL ビューアプリセット]**&#x200B;に移動します。 ビューアプリセットページには、ビューアプリセットの追加、編集、削除およびアクティブ化を行うコマンドがあります。

[ビデオビューアプリセットの操作](previewing-videos-video-viewer.md#working_with_video_viewer_presets)を参照してください。

## 3. Webサイトやモバイルサイトにビデオをデプロイする

ビデオを Web サイトに統合するには、次のいずれかの操作を行います。

* ビデオを独自のポップアップウィンドウまたはモーダルウィンドウに表示します。その場合は、URL ]**をコピー機能を使用します。**[!UICONTROL 

   ビデオの URL を取得するには、グリッドビューまたはリストビューの参照パネルでビデオを選択します。「**[!UICONTROL プレビュー]**」を選択し、「`Universal_HTML5_Viewer`」の右側にある「**[!UICONTROL URLをコピー]**」を選択します。

   「**[!UICONTROL URLをコピー]**」を選択すると、URLがクリップボードにコピーされます。 Web サイト、モバイルサイトまたはアプリケーションの HTML にこのコードを設定します。

   >[!NOTE]
   >
   >URL はビデオまたはアダプティブビデオセットを公開するまでアクティブになりません。

* Webページに埋め込まれたビデオを表示します。この場合は、**[!UICONTROL 埋め込みコード]**&#x200B;機能を使用します。

   ビデオの埋め込みコードを取得するには、グリッドビューまたはリストビューの参照パネルでビデオを選択します。**[!UICONTROL プレビュー]** > **[!UICONTROL ビューアリスト]**&#x200B;に移動します。 表の「アクション」列で、「`Universal_HTML5_Video`」の右側にある「**[!UICONTROL 埋め込みコード]**」を選択します。 コードの編集はできません。

   「**[!UICONTROL 閉じる]**」を選択し、埋め込みコードをWebページに貼り付けます。

   >[!NOTE]
   >
   >埋め込みコードはビデオまたはアダプティブビデオセットを公開するまでアクティブになりません。

[Webサイトおよびモバイルサイトへのビデオのデプロイ](deploying-video-websites-mobile-sites.md#deploying_video_to_your_websites_and_mobile_sites)を参照してください。

>[!MORELIKETHIS]
>
>* [ビデオのエンコーディングのベストプラクティス](uploading-encoding-videos.md#best_practices_for_video_encoding)

