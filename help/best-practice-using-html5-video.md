---
title: HTML5ビデオビューア使用のベストプラクティス
description: HTML5ビデオビューアの使用に関するベストプラクティスを説明します。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Mediaクラシック，ビューア，ビデオ
role: 開業医
translation-type: tm+mt
source-git-commit: 3def4a02eda8dc36f2811b3d4f0e870fff1994e4
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 12%

---


# HTML5ビデオビューア{#best-practice-using-the-html-video-viewer}の使用に関するベストプラクティス

Dynamic MediaクラシックHTML5ビデオビューアプリセットは堅牢なビデオプレーヤーです。 プレーヤーの設計の点では、標準のWeb開発ツールを使用してビデオプレーヤーの全機能を作成できます。 例えば、ボタン、コントロールおよびカスタムのポスター画像背景を HTML5 と CSS を使用して設計し、顧客にカスタマイズした外観を提供することができます。

ビューアの再生の点では、ブラウザーのビデオ機能が自動的に検出されます。次に、HLS（アダプティブビデオストリーミング）を使用してビデオを提供します。 または、その配信メソッドが存在しない場合は、代わりにHTML5プログレッシブが使用されます。

単一のプレーヤーに組み合わせることで、次のような機能を実現できます。

* HTML5とCSSを使用して設計された再生コンポーネント
* 埋め込み再生
* ブラウザの機能に基づくアダプティブストリーミングとプログレッシブストリーミングの使用

リッチメディアコンテンツの提供先を、デスクトップユーザーとモバイルユーザーに拡張できます。 また、ビデオエクスペリエンスを合理化することもできます。

Adobeビューアリファレンスガイドの[HTML5ビューアについて](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only)も参照してください。

## Dynamic Mediaクラシックビデオビューアを使用したデスクトップコンピューターおよび携帯端末でのビデオ再生{#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

デスクトップおよびモバイル向けのアダプティブビデオストリーミングの場合、ビットレートの切り替えに使用するビデオは、アダプティブビデオセット内のすべてのMP4ビデオに基づきます。

ビデオ再生は、HLSまたはプログレッシブビデオを使用して行われます。 HLS(HTTP Live Streaming)は、アダプティブビデオストリーミングのAppleの標準で、ネットワーク帯域幅容量に基づいて再生を自動調整します。 また、残りのビデオがダウンロードされるまで待たなくても、顧客はビデオ内の任意の時点を「検索」できます。 [HTTPライブストリーミング](https://developer.apple.com/streaming/)も参照してください。 プログレッシブビデオは、ビデオをローカルにダウンロードして保存することで配信されます。プログレッシブビデオは、ユーザーのデスクトップ画面または携帯端末にローカルに保存されます。

次の表に、Dynamic Mediaクラシックビデオビューアを使用するデスクトップコンピューターおよび携帯端末でのビデオのデバイス、ブラウザー、再生方法を示します。

| デバイス | ブラウザ | ビデオ再生モード |
|--- |--- |--- |
| デスクトップ | Internet Explorer 9および10 | プログレッシブダウンロード |
| デスクトップ | Internet Explorer 11+ | HLSビデオストリーミング。 |
| デスクトップ | Firefox 23-44 | プログレッシブダウンロード |
| デスクトップ | Firefox 45以降 | HLSビデオストリーミング。 |
| デスクトップ | クロム | HLSビデオストリーミング。 |
| デスクトップ | Safari(Mac) | HLSビデオストリーミング。 |
| モバイル | Chrome（Android™ 6以前） | プログレッシブダウンロード |
| モバイル | Chrome（Android™ 7以降） | HLSビデオストリーミング。 |
| モバイル | Android™（デフォルトのブラウザ） | プログレッシブダウンロード |
| モバイル | Safari(iOS) | HLSビデオストリーミング。 |
| モバイル | Chrome(iOS) | HLSビデオストリーミング。 |
| モバイル | BlackBerry® | HLSビデオストリーミング。 |
