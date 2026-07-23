---
title: HTML5 ビデオビューアの使用に関するベストプラクティス
description: HTML5 ビデオビューアの使用に関するベストプラクティスについて説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T17:39:23.475Z'
TQID: 'https://experienceleague.adobe.com/wGnoHGEOQLVV-rnoKBOE8wzphK3VaM-vr9YB1Y-gT8c'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 5fdabd28c4d0defdf9f145b581c89640cc1f6118
workflow-type: tm+mt
source-wordcount: 482
ht-degree: 2%

---

# HTML5 ビデオビューアの使用に関するベストプラクティス{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5 ビデオビューアプリセットは、高性能なビデオプレーヤーです。 プレーヤーのデザインでは、標準のWeb開発ツールを使用して、ビデオプレーヤーの機能全体を作成できます。 外観をカスタマイズするには、HTML5とCSSを使用して、ボタン、コントロール、およびカスタムポスター画像をデザインします。

ビューア再生では、ブラウザーのビデオ機能が自動的に検出されます。 次に、アダプティブビデオストリーミングとも呼ばれるHLS（HTTP Live Streaming）を使用してビデオを配信します。 または、その配信方法が存在しない場合は、代わりにHTML5 プログレッシブが使用されます。

以下の機能を1人のプレイヤーに組み合わせることで：

* HTML5とCSSを使用して設計された再生コンポーネント。
* 埋め込み再生：
* ブラウザーの機能に基づくアダプティブストリーミングとプログレッシブストリーミングの使用。

リッチメディアコンテンツをデスクトップおよびモバイルユーザー向けに提供できるようになります。 また、合理化された動画体験を実現できます。

Adobe ビューアリファレンスガイドの「[HTML5 ビューアについて](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only)」も参照してください。

[ ビューアプリセット ](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS)のトレーニングビデオも参照してください。

## Adobe Dynamic Media Classic Video Viewerを使用したデスクトップコンピューターおよびモバイルデバイスでのビデオの再生 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

デスクトップおよびモバイルアダプティブビデオストリーミングの場合、ビットレートの切り替えに使用されるビデオは、アダプティブビデオセット内のすべてのMP4 ビデオに基づいています。

ビデオの再生は、HLSまたはプログレッシブビデオを使用して行われます。 HLS（HTTP Live Streaming）は、ネットワーク帯域幅の処理能力に基づいて再生を自動的に調整するアダプティブビデオストリーミング用のApple規格です。 また、利用者は、動画の残りの部分がダウンロードされるのを待つことなく、動画内の任意のポイントに移動することもできます。 [HTTP ライブストリーミング ](https://developer.apple.com/streaming/)も参照してください。 このシステムは、ユーザーのデスクトップ画面またはモバイルデバイスにローカルにダウンロードして保存することで、プログレッシブビデオを配信します。

次の表では、Adobe Dynamic Media Classic Video Viewerを使用したデスクトップコンピューターおよびモバイルデバイスでのビデオのデバイス、ブラウザー、再生方法について説明します。

| デバイス | ブラウザ | ビデオ再生モード |
|--- |--- |--- |
| デスクトップ | Internet Explorer 9および10 | プログレッシブダウンロード。 |
| デスクトップ | Internet Explorer 11以降 | HLS動画ストリーミング： |
| デスクトップ | Firefox 23-44 | プログレッシブダウンロード。 |
| デスクトップ | Firefox 45以降 | HLS動画ストリーミング： |
| デスクトップ | Chrome | HLS動画ストリーミング： |
| デスクトップ | Safari （Mac） | HLS動画ストリーミング： |
| モバイル | Chrome（Android™ 6以前） | プログレッシブダウンロード。 |
| モバイル | Chrome（Android™ 7以降） | HLS動画ストリーミング： |
| モバイル | Android™ （デフォルトブラウザー） | プログレッシブダウンロード。 |
| モバイル | Safari （iOS） | HLS動画ストリーミング： |
| モバイル | Chrome（iOS） | HLS動画ストリーミング： |
| モバイル | BlackBerry® | HLS動画ストリーミング： |
