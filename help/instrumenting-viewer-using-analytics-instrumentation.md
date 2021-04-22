---
title: Adobe Analytics 計測キットを使用したビューアの計測
description: Adobe Analytics計測キットを使用してビューアを計測する方法を説明します。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Mediaクラシック
role: Data Engineer,Administrator,Business Practitioner
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
translation-type: tm+mt
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 28%

---

# Adobe Analytics 計測キットを使用したビューアの計測{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

HTML5ビューアをAdobe Analyticsと統合するには、Adobe Analytics計測キットを使用します。

定義済みのDynamic MediaクラシックHTML5ビューアプリセットのいずれかを使用する場合、そのプリセットには、Adobe Analyticsにデータを送信するためのすべての導入コードが既に含まれています。これ以上の計測は必要ありません。

## Dynamic Mediaクラシック{#set-up-adobe-analytics-tracking-from-scene-publishing-system}のAdobe Analyticsトラッキングを設定

すべてのHTML5ビューアに対して、次のJavaScript™をHTMLコンテナ（通常は&lt;head>要素）に追加します。

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

ここで`Dynamic Media Classic Company ID`は、Dynamic Mediaクラシック会社名に設定します。 また、会社プリセット名が`companypreset`でない限り、`&preset`はオプションです。 そのような場合は、`companypreset-1, companypreset-2`のようになります。 番号が大きいほど、プリセットの最新のインスタンスになります。正しい会社プリセット値の名前を指定するには、「**[!UICONTROL URLをコピー]**」をクリックし、`preset=`パラメーターを確認して会社プリセット名を探します。

次に、ビューアイベントをAdobe Analytics追跡コードに送信する関数を追加します。

コンテナ追加のHTML（またはJSP、ASPX、その他）に対する`s7ComponentEvent()`関数：

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

関数名では大文字と小文字が区別されます。 `s7componentEvent`に渡す唯一の必須パラメータは最後のパラメータです。`eventData`. ここで`s7track()`は、上記のs_code.jspで定義されています。 `s7track`は、各イベントごとにすべての追跡を処理します。 （Adobe Analytics に送信されるデータをさらにカスタマイズする場合は、この領域で行います）。

## HREF および ITEM イベントの有効化  {#enabling-href-and-item-events}

画像マップを編集することで、ビューアの HREF（ロールオーバー）および ITEM（マウスクリック／タッチ）イベントを有効にできます。ビューアコンテンツと関連付けられている画像マップ内で、HREF と ITEM の識別子を定義します。画像マ追加ップ内のHREF値の`&rolloverKey=`パラメータ。
