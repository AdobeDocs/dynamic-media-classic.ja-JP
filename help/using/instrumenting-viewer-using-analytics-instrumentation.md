---
title: Adobe Analytics Instrumentation Kitを使用してビューアを計装する
description: Adobe Dynamic Media ClassicのAdobe Analytics Instrumentation Kitを使用してビューアを計測する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/adobe_analytics_instrumentation_kit
feature: Dynamic Media Classic
role: Developer,Admin,User
exl-id: 9ea1546d-e6d1-4ba4-8fa1-26b4e69375ba
topic: Integrations, Development
level: Experienced
autotag-review: '2026-05-13T19:51:34.654Z'
TQID: 'https://experienceleague.adobe.com/veMzN35J6flKfCAFvdPfZPgxJ9oGy0LYYGhjr-hZLcY'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: d378ca77-2da1-4f39-ad92-1917fe974a38
topic_v2: id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 307
ht-degree: 14%

---

# Adobe Analytics Instrumentation Kitを使用してビューアを計装する{#instrumenting-a-viewer-using-the-adobe-analytics-instrumentation-kit}

Adobe Analytics Instrumentation Kitを使用して、HTML5 ビューアをAdobe Analyticsと統合できます。

定義済みのAdobe Dynamic Media Classic HTML 5 ビューアプリセットのいずれかを使用する場合、Adobe Analyticsにデータを送信するためのすべての実装コードが既に含まれています。 さらにインストルメントを追加する必要はありません。

## Adobe Dynamic Media ClassicからAdobe Analytics トラッキングを設定する {#set-up-adobe-analytics-tracking-from-scene-publishing-system}

すべてのHTML5 ビューアに対して、通常は&lt;head>要素に次のJavaScriptをHTML コンテナに追加します。

```as3
<!-- ***** Adobe Analytics Tracking ***** --><script type="text/javascript" src="https://s7d6.scene7.com/s7viewers/s_code.jsp?company=<Adobe Dynamic Media Classic Company ID>&preset=companypreset-1"></script>
```

ここで、`Adobe Dynamic Media Classic Company ID`はAdobe Dynamic Media Classicの会社名に設定されています。 `&preset`はオプションです。 会社のプリセット名が`companypreset`でない場合は、オプションではありません。 このような場合は、`companypreset-1, companypreset-2`などが考えられます。 番号が大きいほど、プリセットの最新のインスタンスになります。 正しい会社プリセットの値名を決定するには、**[!UICONTROL URLをコピー]**&#x200B;を選択し、`preset=` パラメーターを参照して会社プリセット名を見つけます。

続いて、ビューアイベントをAdobe Analytics トラッキングコードに送信する関数を追加します。

コンテナ HTML（またはJSP、またはASPXなど）に`s7ComponentEvent()`関数を追加します。

```as3
function s7ComponentEvent(objectId, componentClass, instanceName, timeStamp, eventData) {     s7track(eventData); }
```

関数名では大文字と小文字が区別されます。 必須の`s7componentEvent`に渡された唯一のパラメーターは、最後のパラメーターである`eventData`です。 ここで、`s7track()`は上記に含まれるs_code.jspで定義されています。 `s7track`は各イベントごとにすべてのトラッキングを処理します。 （Adobe Analyticsに送信されるデータは、この領域でカスタマイズできます）。

## HREF イベントとITEM イベントを有効にする {#enabling-href-and-item-events}

画像マップを編集することで、ビューアの HREF（ロールオーバー）および ITEM（マウスクリック／タッチ）イベントを有効にできます。 ビューアコンテンツと関連付けられている画像マップ内で、HREF と ITEM の識別子を定義します。 画像マップ内のHREF値に`&rolloverKey=` パラメーターを追加します。
