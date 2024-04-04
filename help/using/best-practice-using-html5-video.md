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
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 9%

---

# HTML5 ビデオビューアの使用に関するベストプラクティス{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media ClassicHTML5 ビデオビューアプリセットは堅牢なビデオプレーヤーです。 プレーヤーのデザイン側では、標準の Web 開発ツールを使用して、ビデオプレーヤーの全機能を作成できます。 例えば、ボタン、コントロールおよびカスタムのポスター画像背景を HTML5 と CSS を使用して設計し、顧客にカスタマイズした外観を提供することができます。

ビューアの再生側では、ブラウザーのビデオ機能が自動的に検出されます。 次に、HLS（HTTP ライブストリーミング）（アダプティブビデオストリーミング）を使用してビデオを提供します。 または、その配信方法が存在しない場合は、代わりにHTML5 プログレッシブが使用されます。

1 人のプレーヤーに組み合わせることで、次の機能を利用できます。

* HTML5 と CSS を使用して設計された再生コンポーネント
* 埋め込み再生
* ブラウザーの機能に基づくアダプティブストリーミングとプログレッシブストリーミングの使用

リッチメディアコンテンツのリーチをデスクトップユーザーとモバイルユーザーに拡張できます。 また、ビデオエクスペリエンスの効率化もおこなえます。

関連トピック [HTML5 ビューアについて](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only) (『Adobeビューアリファレンスガイド』)。

関連トピック [ビューアプリセット](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&amp;emailurl=https://s7d5.scene7.com/s7/emailFriend&amp;serverUrl=https://s7d5.scene7.com/is/image/&amp;config=Scene7SharedAssets/Universal_HTML5_Video&amp;contenturl=https://s7d5.scene7.com/skins/&amp;asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS) トレーニングビデオ。

## Adobe Dynamic Media Classicビデオビューアを使用した、デスクトップコンピューターおよびモバイルデバイスでのビデオの再生 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

デスクトップおよびモバイルへのアダプティブビデオストリーミングの場合、ビットレートの切り替えに使用されるビデオは、アダプティブビデオセット内のすべての MP4 ビデオに基づいています。

ビデオ再生は、HLS またはプログレッシブビデオを使用しておこなわれます。 HLS（HTTP ライブストリーミング）は、Appleのアダプティブビデオストリーミングの標準規格で、ネットワーク帯域幅の容量に基づいて再生を自動的に調整します。 また、ビデオの残りのダウンロードを待たずに、ビデオ内の任意のポイントを「シーク」できます。 関連トピック [HTTP Live Streaming](https://developer.apple.com/streaming/). プログレッシブビデオは、ユーザーのデスクトップ画面またはモバイルデバイスにビデオをローカルにダウンロードして保存することで配信されます。

次の表に、Adobe Dynamic Media Classicビデオビューアを使用するデスクトップコンピューターおよびモバイルデバイスでのビデオのデバイス、ブラウザー、再生方法を示します。

| デバイス | ブラウザ | ビデオ再生モード |
|--- |--- |--- |
| デスクトップ | Internet Explorer 9 および 10 | プログレッシブダウンロード。 |
| デスクトップ | Internet Explorer 11 以降 | HLS ビデオストリーミング。 |
| デスクトップ | Firefox 23-44 | プログレッシブダウンロード。 |
| デスクトップ | Firefox 45 以降 | HLS ビデオストリーミング。 |
| デスクトップ | クロム | HLS ビデオストリーミング。 |
| デスクトップ | Safari (Mac) | HLS ビデオストリーミング。 |
| モバイル | Chrome(Android™ 6 以前 ) | プログレッシブダウンロード。 |
| モバイル | Chrome(Android™ 7 以降 ) | HLS ビデオストリーミング。 |
| モバイル | Android™（デフォルトのブラウザー） | プログレッシブダウンロード。 |
| モバイル | Safari (iOS) | HLS ビデオストリーミング。 |
| モバイル | Chrome(iOS) | HLS ビデオストリーミング。 |
| モバイル | BlackBerry® | HLS ビデオストリーミング。 |
