---
title: Adobe Analytics 計測キットを使用したビューアの計測
seo-title: Adobe Analytics 計測キットを使用したビューアの計測
description: 'null'
seo-description: Adobe Analytics計測キットを使用してビューアを実装する方法について説明します。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
geptopics: SG_ SCESTESEVENT_ PK/categories/adobe_ analytics_ recurtion_ kit
discoiquuid: a2824244-1755-42de- a167-42af117cf038
translation-type: tm+mt
source-git-commit: 32f5e03766466ceaafe58780e9e80dbdd4a0c3dd

---


# Adobe Analytics 計測キットを使用したビューアの計測{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics計測キットを使用して、HTML5ビューアをAdobe Analyticsと統合できます。

定義済みのDynamic Media Classic HTML5ビューアプリセットのいずれかを使用する場合、Adobe Analyticsにデータを送信するために必要なすべての実装コードが含まれていることに注意してください——その他の計測値は必要ありません。

## Scene7 Publishing System からの Adobe Analytics 追跡の設定 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

すべてのHTML5ビューアで、次のJavaScriptをHTMLコンテナに追加します。通常は&lt; head&gt;要素に追加します。

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<SPS Company ID>&preset=companypreset-1"></script>
```

`Company` は SPS 会社名に設定します。`&preset` は、会社プリセット名がない場合はオプション `companypreset`です。In such cases, it could be `companypreset-1, companypreset-2`, and so on. 番号が大きいほど、プリセットの最新のインスタンスになります。To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

次に、ビューアイベントを Adobe Analytics 追跡コードに送信する関数を追加します。

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

関数名では大文字と小文字が区別されます。The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` は、上記のs_ code. jspに定義されています。`s7track` は、各イベントごとにすべてのトラッキングを処理します。（Adobe Analytics に送信されるデータをさらにカスタマイズする場合は、この領域で行います）。

## HREF および ITEM イベントの有効化 {#enabling-href-and-item-events}

画像マップを編集することで、ビューアの HREF（ロールオーバー）および ITEM（マウスクリック／タッチ）イベントを有効にできます。ビューアコンテンツと関連付けられている画像マップ内で、HREF と ITEM の識別子を定義します。Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
