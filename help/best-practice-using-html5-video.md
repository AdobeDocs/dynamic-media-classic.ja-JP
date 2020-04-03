---
title: '"ベストプラクティス：HTML5 ビデオビューアの使用"'
seo-title: '"ベストプラクティス：HTML5 ビデオビューアの使用"'
description: 'null'
seo-description: HTML5ビデオビューアの使用に関するベストプラクティスを説明します。
uuid: 3c8924dc-7bea-4c25-b77b-005f57b71b64
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
geptopics: SG_SCENESEVENONDEMAND_PK/categories/video
discoiquuid: 4b11cab7-88cf-42dd-8554-2eea530753bb
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# ベストプラクティス：HTML5 ビデオビューアの使用{#best-practice-using-the-html-video-viewer}

ダイナミックメディアクラシックHTML5ビデオビューアのプリセットは、堅牢なビデオプレーヤーです。 プレーヤーのデザインの面では、標準のWeb開発ツールを使用して、ビデオプレーヤーのすべての機能を作成できます。 例えば、ボタン、コントロールおよびカスタムのポスター画像背景を HTML5 と CSS を使用して設計し、顧客にカスタマイズした外観を提供することができます。

ビューアの再生の点では、ブラウザーのビデオ機能が自動的に検出されます。次に、HLS（アダプティブビデオストリーミング）を使用してビデオを配信します。 または、その配信メソッドが存在しない場合は、代わりにHTML5プログレッシブが使用されます。

HTML5 と CSS を使用した再生コンポーネントの設計、再生の埋め込み、およびブラウザーの機能に基づくアダプティブストリーミングおよびプログレッシブストリーミングの使用ができる機能を単一のプレーヤーに統合することで、リッチメディアコンテンツをデスクトップユーザーとモバイルユーザーの両方に提供し、ビデオ配信の効率化を確実に行うことができます。

『Adobe Viewers Reference Guide [』の](https://marketing.adobe.com/resources/help/en_US/s7/viewers_ref/c_html5_viewers_about.html) 「HTML5ビューアについて」も参照してください。

## ダイナミックメディアクラシックビデオビューアを使用したデスクトップコンピューターおよび携帯端末でのビデオの再生 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

デスクトップおよびモバイルのアダプティブビデオストリーミングの場合、ビットレートの切り替えに使用されるビデオは、アダプティブビデオセット内のすべてのMP4ビデオに基づきます。

ビデオ再生は、HLSまたはプログレッシブビデオを使用して行われます。 HLS(HTTP Live Streaming)は、ネットワークの帯域幅容量に基づいて再生を自動調整する、アダプティブビデオストリーミングのAppleの標準です。 また、残りのビデオがダウンロードされるのを待つ必要なく、顧客がビデオ内の任意の時点を「検索」できるようにします( [HTTPライブストリーミングも参照](#UnresolvedLink-https://developer.apple.com/streaming/))。 プログレッシブビデオは、ビデオをローカルにダウンロードし、ユーザーのデスクトップ画面または携帯端末に保存することで配信されます。

次の表に、ダイナミックメディアクラシックビデオビューアを使用するデスクトップコンピューターおよび携帯端末でのビデオのデバイス、ブラウザー、再生方法を示します。

| デバイス | ブラウザ | ビデオ再生モード |
|--- |--- |--- |
| デスクトップ | Internet Explorer 9および10 | プログレッシブダウンロード。 |
| デスクトップ | Internet Explorer 11+ | HLSビデオストリーミング。 |
| デスクトップ | Firefox 23-44 | プログレッシブダウンロード。 |
| デスクトップ | Firefox 45以降 | HLSビデオストリーミング。 |
| デスクトップ | クロム | HLSビデオストリーミング。 |
| デスクトップ | Safari(Mac OS) | HLSビデオストリーミング。 |
| モバイル | Chrome（Android 6以前） | プログレッシブダウンロード。 |
| モバイル | Chrome（Android 7以降） | HLSビデオストリーミング。 |
| モバイル | Android（デフォルトのブラウザー） | プログレッシブダウンロード。 |
| モバイル | Safari(iOS) | HLSビデオストリーミング。 |
| モバイル | Chrome(iOS) | HLSビデオストリーミング。 |
| モバイル | Blackberry | HLSビデオストリーミング。 |
