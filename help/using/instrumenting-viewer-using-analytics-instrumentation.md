---
title: Adobe Analytics Instrumentation Kit を使用したビューアのインストルメント
description: Adobe Dynamic Media ClassicのAdobe Analytics Instrumentation Kit を使用してビューアをインストルメント化する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Data Engineer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
source-git-commit: 163eb32112ec6fbefd1dacf48212353ff3053d54
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 15%

---

# Adobe Analytics Instrumentation Kit を使用したビューアのインストルメント{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics Instrumentation Kit を使用して、HTML5 ビューアをAdobe Analyticsと統合できます。

事前定義済みのAdobe Dynamic Media Classic HTML5 ビューアプリセットを使用すると、Adobe Analyticsにデータを送信するためのすべての実装コードが既に含まれます。 それ以上のインストルメンテーションを追加する必要はありません。

## Adobe Dynamic Media ClassicからのAdobe Analytics トラッキングの設定 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

すべてのHTML5 ビューアで、HTMLコンテナに次の JavaScript を追加します。通常は、次の場所に追加します。 &lt;head> 要素：

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

ここで、 `Adobe Dynamic Media Classic Company ID` は、Adobe Dynamic Media Classicの会社名に設定されます。 および `&preset` はオプションです。 会社プリセット名が `companypreset`を選択した場合、これはオプションではありません。 このような場合、次の可能性があります。 `companypreset-1, companypreset-2`など。 番号が大きいほど、プリセットの最新のインスタンスになります。正しい会社プリセット値の名前を決定するには、を選択します **[!UICONTROL URL をコピー]**&#x200B;を選択し、次のを確認します `preset=`パラメーターを指定して、会社のプリセット名を検索します。

続いて、ビューアイベントをAdobe Analytics トラッキングコードに送信する関数を追加します。

を追加 `s7ComponentEvent()` コンテナHTML（または JSP、ASPX またはその他）に対する機能を次に示します。

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

関数名では大文字と小文字が区別されます。 に渡される唯一のパラメーター `s7componentEvent`要求されるのは最後の要求です。 `eventData`. ここで、 `s7track()` は、上記に含まれた s_code.jsp で定義されます。 および `s7track` 各イベントごとのすべてのトラッキングを処理します。 （Adobe Analyticsに送信されるデータは、この領域でさらにカスタマイズできます）。

## HREF および項目イベントを有効にする {#enabling-href-and-item-events}

画像マップを編集することで、ビューアの HREF（ロールオーバー）および ITEM（マウスクリック／タッチ）イベントを有効にできます。ビューアコンテンツと関連付けられている画像マップ内で、HREF と ITEM の識別子を定義します。を追加 `&rolloverKey=` 画像マップ内の HREF 値に対するパラメーター。
