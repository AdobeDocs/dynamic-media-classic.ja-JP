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
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 15%

---

# Adobe Analytics Instrumentation Kit を使用したビューアのインストルメント{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics Instrumentation Kit を使用して、HTML5 ビューアをAdobe Analyticsと統合できます。

事前定義済みのAdobe Dynamic Media Classic HTML5 ビューアプリセットのいずれかを使用すると、データをAdobe Analyticsに送信するためのすべての実装コードが既に含まれます。 それ以上のインストルメンテーションを追加する必要はありません。

## Adobe Dynamic Media ClassicからのAdobe Analytics トラッキングの設定 {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

すべてのHTML5 ビューアで、次のJavaScriptをHTML コンテナ（通常は &lt;head> 要素）に追加します。

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

ここで、`Adobe Dynamic Media Classic Company ID` はAdobe Dynamic Media Classicの会社名に設定されます。 また、`&preset` はオプションです。 会社のプリセット名が `companypreset` でない場合は、オプションではありません。 このような場合は、`companypreset-1, companypreset-2` など、様々な影響が考えられます。 番号が大きいほど、プリセットの最新のインスタンスになります。正しい会社プリセット値の名前を決定するには、「**[!UICONTROL URL をコピー]**」を選択し、`preset=` パラメーターを確認して、会社プリセット名を見つけます。

続いて、ビューアイベントをAdobe Analytics トラッキングコードに送信する関数を追加します。

コンテナ HTML（または JSP、ASPX など）に `s7ComponentEvent()` 関数を追加します。

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

関数名では大文字と小文字が区別されます。 `s7componentEvent` に渡される必須のパラメーターは、最後のパラメーター `eventData` のみです。 ここで、`s7track()` は上記に含まれた s_code.jsp で定義されます。 また、`s7track` は各イベントごとにすべてのトラッキングを処理します。 （Adobe Analyticsに送信されるデータは、この領域でさらにカスタマイズできます）。

## HREF および項目イベントを有効にする {#enabling-href-and-item-events}

画像マップを編集することで、ビューアの HREF（ロールオーバー）および ITEM（マウスクリック／タッチ）イベントを有効にできます。ビューアコンテンツと関連付けられている画像マップ内で、HREF と ITEM の識別子を定義します。画像マップ内の HREF 値に `&rolloverKey=` パラメーターを追加します。
