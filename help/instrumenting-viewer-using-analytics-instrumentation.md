---
title: Adobe Analytics Instrumentation Kit を使用したビューアの実装
description: Adobe Dynamic Media ClassicのAdobe Analytics Instrumentation Kit を使用してビューアを実装する方法を説明します。
uuid: cf9a4002-966d-4641-9cd0-2ee8b5454f60
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
discoiquuid: a2824244-1755-42de-a167-42af117cf038
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 20%

---

# Adobe Analytics Instrumentation Kit を使用したビューアの実装{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics Instrumentation Kit を使用して、HTML5 ビューアをAdobe Analyticsと統合できます。

事前定義済みのAdobe Dynamic Media ClassicHTML5 ビューアプリセットのいずれかを使用する場合、Adobe Analyticsにデータを送信するすべての実装コードが既に含まれています。これ以上の計測は必要ありません。

## Adobe Dynamic Media ClassicからのAdobe Analyticsトラッキングの設定 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

すべてのHTML5 ビューアについて、次の JavaScript をHTMLコンテナ ( 通常は &lt;head> 要素：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

ここで、 `Adobe Dynamic Media Classic Company ID` がAdobe Dynamic Media Classicの会社名に設定されている。 および `&preset` は、会社プリセット名が `companypreset`. このような場合、 `companypreset-1, companypreset-2`など。 番号が大きいほど、プリセットの最新のインスタンスになります。正しい会社プリセット値の名前を判断するには、 **[!UICONTROL URL をコピー]** をクリックし、 `preset=`パラメーターを使用して会社プリセット名を検索します。

続けて、ビューアイベントをAdobe Analyticsトラッキングコードに送信する関数を追加します。

を `s7ComponentEvent()` 関数をコンテナHTML（または JSP、または ASPX など）に追加します。

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

関数名では、大文字と小文字が区別されます。 に渡される唯一のパラメーター `s7componentEvent`これが最後の要件です。 `eventData`. ここで、 `s7track()` は、上記に含まれる s_code.jsp で定義されます。 および `s7track` は、各イベントごとにすべての追跡を処理します。 （Adobe Analytics に送信されるデータをさらにカスタマイズする場合は、この領域で行います）。

## HREF および ITEM イベントの有効化 {#enabling-href-and-item-events}

画像マップを編集することで、ビューアの HREF（ロールオーバー）および ITEM（マウスクリック／タッチ）イベントを有効にできます。ビューアコンテンツと関連付けられている画像マップ内で、HREF と ITEM の識別子を定義します。を追加します。 `&rolloverKey=` パラメーターを画像マップ内の HREF 値に設定します。
