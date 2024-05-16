---
title: HTML5 ビデオビューアの使用のベストプラクティス
description: HTML5 ビデオビューアを使用する際のベストプラクティスについて説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
feature: Dynamic Media Classic,Viewers,Video
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
topic: Content Management
level: Intermediate
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 9%

---

# HTML5 ビデオビューア使用のベストプラクティス{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5 ビデオビューアプリセットは、堅牢なビデオプレーヤーです。 プレーヤーの設計面では、標準の web 開発ツールを使用してビデオプレーヤーの機能全体を作成できます。 例えば、ボタン、コントロールおよびカスタムのポスター画像背景を HTML5 と CSS を使用して設計し、顧客にカスタマイズした外観を提供することができます。

ビューアの再生側では、ブラウザーのビデオ機能を自動的に検出します。 その後、アダプティブビデオストリーミングとも呼ばれる HLS （HTTP ライブストリーミング）を使用してビデオを提供します。 または、その配信方法が使用できない場合は、代わりにHTML5 プログレッシブが使用されます。

単一のプレーヤーに以下の能力を組み合わせる：

* HTML5 と CSS を使用して設計された再生コンポーネント
* 埋め込み再生
* ブラウザーの機能に基づくアダプティブストリーミングおよびプログレッシブストリーミングの使用

リッチメディアコンテンツの配信範囲をデスクトップユーザーとモバイルユーザーに拡大できます。 また、ビデオエクスペリエンスを確実に効率化できます。

関連トピック [HTML5 ビューアについて](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) （Adobeビューアリファレンスガイド）を参照してください。

関連トピック [ビューアプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

## Adobe Dynamic Media Classic ビデオビューアを使用した、デスクトップコンピューターおよびモバイルデバイスでのビデオ再生 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

デスクトップおよびモバイルへのアダプティブビデオストリーミングの場合、ビットレートの切り替えに使用されるビデオは、アダプティブビデオセット内のすべての MP4 ビデオに基づいています。

ビデオ再生は、HLS ビデオまたはプログレッシブビデオを使用して行われます。 HLS （HTTP ライブストリーミング）は、アダプティブビデオストリーミングのApple標準で、ネットワーク帯域幅に基づいて再生を自動調整します。 また、ビデオの残りがダウンロードされるまで待たなくても、ビデオ内の任意のポイントを「シーク」できます。 関連トピック [HTTP ライブストリーミング](https://developer.apple.com/streaming/). プログレッシブビデオは、ユーザーのデスクトップ画面やモバイルデバイスにダウンロードしてローカルに保存することで配信されます。

デスクトップコンピューターおよびモバイルデバイスでAdobe Dynamic Media Classic ビデオビューアを使用してビデオを再生する場合の、デバイス、ブラウザーおよび再生方法を次の表に示します。

| デバイス | ブラウザ | ビデオ再生モード |
|--- |--- |--- |
| デスクトップ | Internet Explorer 9 および 10 | プログレッシブダウンロード。 |
| デスクトップ | Internet Explorer 11+ | HLS ビデオストリーミング。 |
| デスクトップ | Firefox 23-44 | プログレッシブダウンロード。 |
| デスクトップ | Firefox 45 以降 | HLS ビデオストリーミング。 |
| デスクトップ | Chrome | HLS ビデオストリーミング。 |
| デスクトップ | Safari （Mac） | HLS ビデオストリーミング。 |
| モバイル | Chrome （Android™ 6 以前） | プログレッシブダウンロード。 |
| モバイル | Chrome （Android™ 7 以降） | HLS ビデオストリーミング。 |
| モバイル | Android™ （デフォルトブラウザー） | プログレッシブダウンロード。 |
| モバイル | Safari （iOS） | HLS ビデオストリーミング。 |
| モバイル | Chrome （iOS） | HLS ビデオストリーミング。 |
| モバイル | BlackBerry® | HLS ビデオストリーミング。 |
