---
title: HTML5ビデオビューアの使用に関するベストプラクティス
description: HTML5ビデオビューアを使用する際のベストプラクティスについて説明します。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
feature: Dynamic Media Classic，ビューア，ビデオ
role: User
exl-id: ce49e4ce-8dc0-41e1-865a-249f23757553
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 12%

---

# HTML5ビデオビューアの使用に関するベストプラクティス{#best-practice-using-the-html-video-viewer}

Dynamic Media Classic HTML5ビデオビューアプリセットは堅牢なビデオプレーヤーです。 プレーヤーのデザイン側では、標準のWeb開発ツールを使用してビデオプレーヤーの全機能を作成できます。 例えば、ボタン、コントロールおよびカスタムのポスター画像背景を HTML5 と CSS を使用して設計し、顧客にカスタマイズした外観を提供することができます。

ビューアの再生の点では、ブラウザーのビデオ機能が自動的に検出されます。次に、HLS（HTTPライブストリーミング）を使用してビデオを配信します。これはアダプティブビデオストリーミングとも呼ばれます。 または、その配信方法が存在しない場合は、代わりにHTML5プログレッシブが使用されます。

を1人のプレーヤーに組み合わせることで、次の機能を実現します。

* HTML5とCSSを使用して設計された再生コンポーネント
* 埋め込み再生
* ブラウザーの機能に基づくアダプティブストリーミングとプログレッシブストリーミングの使用

リッチメディアコンテンツのリーチをデスクトップユーザーとモバイルユーザーに拡張できます。 また、ビデオエクスペリエンスの効率化も図れます。

『Adobeビューアリファレンスガイド』の[HTML5ビューアについて](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers.html?lang=en#viewers-for-aem-assets-only)も参照してください。

## Dynamic Media Classicビデオビューアを使用したデスクトップコンピューターおよびモバイルデバイスでのビデオの再生 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

デスクトップおよびモバイルのアダプティブビデオストリーミングの場合、ビットレートの切り替えに使用されるビデオは、アダプティブビデオセット内のすべてのMP4ビデオに基づいています。

ビデオ再生は、HLSまたはプログレッシブビデオを使用しておこなわれます。 HLS（HTTPライブストリーミング）は、アダプティブビデオストリーミングのApple標準で、ネットワーク帯域幅の容量に基づいて再生を自動調整します。 また、お客様は、ビデオの残りのダウンロードを待たずに、ビデオ内の任意のポイントを「シーク」できます。 [HTTPライブストリーミング](https://developer.apple.com/streaming/)も参照してください。 プログレッシブビデオは、ユーザーのデスクトップ画面またはモバイルデバイスにビデオをローカルにダウンロードして保存することで配信されます。

次の表に、Dynamic Media Classicビデオビューアを使用するデスクトップコンピューターおよびモバイルデバイスでのビデオのデバイス、ブラウザー、再生方法を示します。

| デバイス | ブラウザ | ビデオ再生モード |
|--- |--- |--- |
| デスクトップ | Internet Explorer 9および10 | プログレッシブダウンロード。 |
| デスクトップ | Internet Explorer 11以降 | HLSビデオストリーミング。 |
| デスクトップ | Firefox 23-44 | プログレッシブダウンロード。 |
| デスクトップ | Firefox 45以降 | HLSビデオストリーミング。 |
| デスクトップ | クロム | HLSビデオストリーミング。 |
| デスクトップ | Safari(Mac OS) | HLSビデオストリーミング。 |
| モバイル | Chrome(Android™ 6以前) | プログレッシブダウンロード。 |
| モバイル | Chrome(Android™ 7以降) | HLSビデオストリーミング。 |
| モバイル | Android™（デフォルトのブラウザー） | プログレッシブダウンロード。 |
| モバイル | Safari(iOS) | HLSビデオストリーミング。 |
| モバイル | Chrome(iOS) | HLSビデオストリーミング。 |
| モバイル | BlackBerry® | HLSビデオストリーミング。 |
