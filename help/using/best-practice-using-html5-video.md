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
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 499
ht-degree: 8%

---

# HTML5 ビデオビューアの使用に関するベストプラクティス{#best-practice-using-the-html-video-viewer}

Adobe Dynamic Media Classic HTML5 ビデオビューアプリセットは、堅牢なビデオプレーヤーです。 プレーヤーのデザイン側では、標準のWeb開発ツールを使用して、ビデオプレーヤーの機能全体を作成できます。 例えば、ボタン、コントロールおよびカスタムのポスター画像背景を HTML5 と CSS を使用して設計し、顧客にカスタマイズした外観を提供することができます。

ビューアの再生側では、ブラウザーのビデオ機能が自動的に検出されます。 次に、アダプティブビデオストリーミングとも呼ばれるHLS（HTTP Live Streaming）を使用してビデオを配信します。 または、その配信方法が存在しない場合は、代わりにHTML 5 プログレッシブが使用されます。

1つのプレイヤーに以下の機能を組み合わせることで：

* HTML5とCSSを使用して設計された再生コンポーネント
* 埋め込み再生
* ブラウザーの機能に基づくアダプティブストリーミングとプログレッシブストリーミングの使用

リッチメディアコンテンツのリーチをデスクトップおよびモバイルユーザーに拡大できます。 また、合理化された動画体験を実現できます。

Adobe ビューアリファレンスガイドの「[HTML5 ビューアについて](https://experienceleague.adobe.com/en/docs/dynamic-media-developer-resources/library/viewers-for-aem-assets-only/c-html5-aem-asset-viewers#viewers-for-aem-assets-only)」も参照してください。

[&#x200B; ビューアプリセット &#x200B;](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/550_viewer-presets_converted%20renamed_Done-AVS)のトレーニングビデオも参照してください。

## Adobe Dynamic Media Classic Video Viewerを使用したデスクトップコンピューターおよびモバイルデバイスでのビデオの再生 {#playback-of-video-on-desktop-computers-and-mobile-devices-using-the-scene-video-viewer}

デスクトップおよびモバイルアダプティブビデオストリーミングの場合、ビットレートの切り替えに使用されるビデオは、アダプティブビデオセット内のすべてのMP4 ビデオに基づいています。

ビデオの再生は、HLSまたはプログレッシブビデオを使用して行われます。 HLS（HTTP Live Streaming）は、ネットワーク帯域幅の処理能力に基づいて再生を自動的に調整するアダプティブビデオストリーミング用のApple規格です。 また、ビデオの残りの部分がダウンロードされるのを待たずに、顧客がビデオ内の任意のポイントに「シーク」することもできます。 [HTTP ライブストリーミング &#x200B;](https://developer.apple.com/streaming/)も参照してください。 プログレッシブビデオは、ユーザーのデスクトップ画面またはモバイルデバイスにビデオをダウンロードしてローカルに保存することで配信されます。

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
