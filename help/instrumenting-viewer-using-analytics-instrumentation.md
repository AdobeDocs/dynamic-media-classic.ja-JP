---
title: Adobe Analytics 計測キットを使用したビューアの計測
description: Adobe Analytics Instrumentation Kitを使用してビューアを実装する方法を説明します。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 28%

---

# Adobe Analytics 計測キットを使用したビューアの計測{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics Instrumentation Kitを使用して、HTML5ビューアをAdobe Analyticsと統合できます。

定義済みのDynamic Media Classic HTML5ビューアプリセットのいずれかを使用する場合、Adobe Analyticsにデータを送信するためのすべての実装コードが既に含まれています。これ以上の計測は必要ありません。

## Dynamic Media ClassicからのAdobe Analyticsトラッキングの設定 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

すべてのHTML5ビューアに対して、次のJavaScript™をHTMLコンテナ（通常は&lt;head>要素内）に追加します。

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

ここで、`Dynamic Media Classic Company ID`はDynamic Media Classicの会社名に設定します。 会社のプリセット名が`companypreset`でない限り、`&preset`はオプションです。 そのような場合は`companypreset-1, companypreset-2`などになります。 番号が大きいほど、プリセットの最新のインスタンスになります。正しい会社プリセット値の名前を判断するには、「 **[!UICONTROL URL]**&#x200B;をコピー`preset=` 」をクリックし、パラメーターを参照して会社プリセット名を探します。

続けて、ビューアイベントをAdobe Analyticsトラッキングコードに送信する関数を追加します。

コンテナのHTML（またはJSP、またはASPXなど）に`s7ComponentEvent()`関数を追加します。

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

関数名では大文字と小文字が区別されます。 `s7componentEvent`に渡される必須のパラメーターは最後のパラメーターのみです。`eventData`. ここで、`s7track()`は、上記に含まれるs_code.jspで定義されます。 `s7track`は、各イベントごとにすべての追跡を処理します。 （Adobe Analytics に送信されるデータをさらにカスタマイズする場合は、この領域で行います）。

## HREF および ITEM イベントの有効化 {#enabling-href-and-item-events}

画像マップを編集することで、ビューアの HREF（ロールオーバー）および ITEM（マウスクリック／タッチ）イベントを有効にできます。ビューアコンテンツと関連付けられている画像マップ内で、HREF と ITEM の識別子を定義します。画像マップ内のHREF値に`&rolloverKey=`パラメーターを追加します。
