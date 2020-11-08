---
title: Adobe Analytics 計測キットを使用したビューアの計測
seo-title: Adobe Analytics 計測キットを使用したビューアの計測
description: 'null'
seo-description: Adobe Analytics計測キットを使用してビューアを計測する方法を説明します。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
translation-type: tm+mt
source-git-commit: 9424b392f85536dc75083d0ade255e4824755ed1
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 38%

---


# Adobe Analytics 計測キットを使用したビューアの計測{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

HTML5ビューアをAdobe Analyticsと統合するには、Adobe Analytics計測キットを使用します。

定義済みのDynamic Media Classic HTML5ビューアプリセットのいずれかを使用する場合は、Adobe Analyticsにデータを送信するのに必要な実装コードがすべて含まれていることに注意してください。これ以上の実装は必要ありません。

## Dynamic Media ClassicからのAdobe Analytics追跡の設定 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

すべてのHTML5ビューアに対して、次のJavaScriptをHTMLコンテナ（通常は&lt;head>要素）に追加します。

```as3
<!-- ***** Site Catalyst Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

`Company` は、Dynamic Media Classic会社名に設定されます。 `&preset` は、会社プリセット名がでない場合はオプションで `companypreset`す。 In such cases, it could be `companypreset-1, companypreset-2`, and so on. 番号が大きいほど、プリセットの最新のインスタンスになります。To determine the correct company preset value name, click **Copy URL** , and then look at the `preset=`parameter to find the company preset name.

次に、ビューアイベントを Adobe Analytics 追跡コードに送信する関数を追加します。

Add the `s7ComponentEvent()` function to the container HTML (or JSP, or ASPX or other):

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

関数名では大文字と小文字が区別されます。The only parameter passed to `s7componentEvent`that is required is the last one: `eventData`. `s7track()` は、上記に含まれるs_code.jspで定義されます。 `s7track` は、各イベントごとにすべての追跡を処理します。 （Adobe Analytics に送信されるデータをさらにカスタマイズする場合は、この領域で行います）。

## HREF および ITEM イベントの有効化 {#enabling-href-and-item-events}

画像マップを編集することで、ビューアの HREF（ロールオーバー）および ITEM（マウスクリック／タッチ）イベントを有効にできます。ビューアコンテンツと関連付けられている画像マップ内で、HREF と ITEM の識別子を定義します。Add a `&rolloverKey=` parameter to the HREF value within the Image Map.
