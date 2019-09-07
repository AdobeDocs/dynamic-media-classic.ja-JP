---
title: '"ベストプラクティス：HTML5 ビデオビューアの使用"'
seo-title: '"ベストプラクティス：HTML5 ビデオビューアの使用"'
description: 'null'
seo-description: HTML5ビデオビューアのベストプラクティスについて説明します。
uuid: 3c8924dc-7bea-4c25- b77b-005f57b71b64
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK_ PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2ea530753bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# ベストプラクティス：HTML5 ビデオビューアの使用{#best-practice-using-the-html-video-viewer}

ダイナミックメディアクラシックHTML5ビデオビューアプリセットは堅牢なビデオプレーヤーです。プレーヤーのデザイン側では、標準的なWeb開発ツールを使用して、すべてのビデオプレーヤーの機能を作成できます。例えば、ボタン、コントロールおよびカスタムのポスター画像背景を HTML5 と CSS を使用して設計し、顧客にカスタマイズした外観を提供することができます。

ビューアの再生の点では、ブラウザーのビデオ機能が自動的に検出されます。その後、HLS（アダプティブビデオストリーミング）を使用してビデオを提供します。または、その配信方法が存在しない場合は、代わりにHTML5プログレッシブが使用されます。

HTML5 と CSS を使用した再生コンポーネントの設計、再生の埋め込み、およびブラウザーの機能に基づくアダプティブストリーミングおよびプログレッシブストリーミングの使用ができる機能を単一のプレーヤーに統合することで、リッチメディアコンテンツをデスクトップユーザーとモバイルユーザーの両方に提供し、ビデオ配信の効率化を確実に行うことができます。

"Adobeビューアリファレンスガイド」の"HTML5ビューア [](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) について」も参照してください。

## Dynamic Media Classicビデオビューアを使用したデスクトップコンピューターおよび携帯端末でのビデオの再生 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

デスクトップおよびモバイルアダプティブビデオストリーミングの場合、ビットレートの切り替えに使用されるビデオは、アダプティブビデオセット内のすべてのMP4ビデオに基づきます。

HLSまたはプログレッシブビデオを使用してビデオ再生が発生します。HLS（HTTP Live Streaming）は、ネットワーク帯域幅容量に基づいて再生を自動調整するアダプティブビデオストリーミングのApple標準です。また、ビデオの残りの部分を待機することなく、ビデオの任意の時点まで「シーク」できます（ [HTTP Live Streaming](#UnresolvedLink-https://developer.apple.com/streaming/)も参照）。プログレッシブビデオは、ビデオをダウンロードしてユーザーのデスクトップ画面または携帯端末にローカルに保存することによって配信されます。

次の表に、Dynamic Media Classicビデオビューアを使用したデスクトップコンピューターおよび携帯端末上のビデオのデバイス、ブラウザーおよび再生メソッドを示します。

| デバイス | ブラウザ | ビデオ再生モード |
|--- |--- |--- |
| Deskop | Internet Explorer9および10 | プログレッシブダウンロード。 |
| デスクトップ | Internet Explorer11+ | HLSビデオストリーミング |
| デスクトップ | Firefox23-44 | プログレッシブダウンロード。 |
| デスクトップ | Firefox45以降 | HLSビデオストリーミング |
| デスクトップ | Chrome | HLSビデオストリーミング |
| デスクトップ | Safari（Mac） | HLSビデオストリーミング |
| モバイル | Chrome（Android6以前） | プログレッシブダウンロード。 |
| モバイル | Chrome（Android7以降） | HLSビデオストリーミング |
| モバイル | Android（デフォルトのブラウザー） | プログレッシブダウンロード。 |
| モバイル | Safari（iOS） | HLSビデオストリーミング |
| モバイル | Chrome（iOS） | HLSビデオストリーミング |
| モバイル | Blackberry | HLSビデオストリーミング |
