---
title: Webページへのズームビューアのリンク
description: ズームビューアをWebページにリンクする方法については、AdobeDynamic Media Classicを参照してください。
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/zoom
feature: Dynamic Media Classic,Viewers,Zoom
role: User
exl-id: 2073d95b-1600-481f-8038-d29e8acacf7d
source-git-commit: 1d71cbe6e2493ac8d47e837a20e194b6ae7a22d4
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 34%

---

# Webページへのズームビューアのリンク{#linking-zoom-viewers-to-your-web-pages}

Webサイトやアプリケーションは、URL文字列または埋め込みコードを使用して、マスター画像や関連するズームターゲットなどのDynamic Media Image Serverコンテンツやズームビューアプリセットにアクセスします。 この URL 文字列は、公開処理中にアクティブになります。これらのURL文字列または埋め込みコードをWebページやアプリケーションに配置するには、AdobeDynamic Media ClassicからURL文字列または埋め込みコードをコピーします。

>[!NOTE]
>
>URL は、アセットを公開するまでアクティブになりません。

## ズームビューアのURLのコピー {#copying-a-zoom-viewer-url}

1. 左側のアセットライブラリパネルで、コピーする URL を持つズームビューアを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * 「**[!UICONTROL グリッドビュー]**」または「**[!UICONTROL リストビュー]**」を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側のURLと埋め込みコードパネルで、目的のビューアの右側にある「**[!UICONTROL URL]**&#x200B;をコピー」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の下にある「**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]**」に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL 

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の右側にある&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL 

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細ビュー]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** /**[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「URLをコピー&#x200B;]**」を選択します。**[!UICONTROL 

## WebページへのズームビューアのURLの追加 {#adding-zoom-viewer-urls-to-your-web-page}

通常、訪問者は、Webサイト上の画像をズームする際に、最初にズームアイコン（多くの場合、アイコンには虫眼鏡の画像が表示されます）を選択します。 このアイコンを選択すると、ポップアップウィンドウで画像を表示する動的 Web ページ（ASP または JSP）が起動します。このポップアップウィンドウが、閲覧者が実際に画像をズームする場所となります。

詳細とコードサンプルについては、『Adobeビューアリファレンスガイド』の[HTML5基本ズームビューアの埋め込み](https://experienceleague.adobe.com/docs/dynamic-media-developer-resources/library/viewers-aem-assets-dmc/basic-zoom/c-html5-20-basic-zoom-viewer-about.html#section-e1c3106f5b3e445d9b95be337c2f94e2)を参照してください。

## ズームビューアの埋め込みコピーをコピーする {#copying-the-embed-copy-of-a-zoom-viewer}

埋め込みコード機能を使用すると、選択したズームビューアのビューアコードをレビューすることができます。コードをクリップボードにコピーして、ビューアを配信する Web ページにペーストすることもできます。埋め込みコードダイアログボックスでは、コードの編集はできません。

**ズームビューアの埋め込みコードをコピーするには:**

1. 左側のアセットライブラリパネルで、コピーする埋め込みコードを持つズームビューアを含むアセットフォルダに移動します。
1. アセットの参照パネルの上のツールバーの右側で、次のいずれかの操作を行います。

   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで、1 つのアセットをダブルクリックし、アセットを詳細ビューで開きます。右側のURLと埋め込みコードパネルで、目的のビューアの右側にある「**[!UICONTROL 埋め込みコード]**」を選択します。
   * **[!UICONTROL グリッドビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の下にある「**[!UICONTROL プレビュー]**/**[!UICONTROL ビューアリスト]**」に移動します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL リストビュー]**&#x200B;を選択します。 アセットの参照パネルで1つのアセットを選択し、サムネール画像の右側にある&#x200B;**[!UICONTROL プレビュー]** / **[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

   * **[!UICONTROL グリッドビュー]**、**[!UICONTROL リストビュー]**、または&#x200B;**[!UICONTROL 詳細ビュー]**&#x200B;を選択します。 同じツールバーで、**[!UICONTROL プレビュー]** /**[!UICONTROL ビューアリスト]**&#x200B;に移動します。

      ビューアリストページの表の「アクション」列で、「**[!UICONTROL 埋め込みコード]**」を選択します。

1. 埋め込みコードダイアログボックスで、「**[!UICONTROL クリップボードにコピー]**」を選択します。

   埋め込みコードダイアログボックスでは、コードを編集することはできません。

1. **[!UICONTROL 閉じる]**&#x200B;を選択します。
