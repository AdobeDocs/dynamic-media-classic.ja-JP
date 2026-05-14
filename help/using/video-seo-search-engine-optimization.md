---
title: ビデオ SEO（検索エンジン最適化）
description: Adobe Dynamic Media Classicでビデオ SEO設定を行う方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:17:45.884Z'
TQID: 'https://experienceleague.adobe.com/I9wTnanImSLtXv4Nff2uW92cNkMhoGf5hc8cXsPFNYc'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: c2296997-5d79-4905-b32e-99b5aa892429
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 1054
ht-degree: 28%

---

# ビデオ SEO（検索エンジン最適化）{#video-seo-search-engine-optimization}

検索エンジン最適化（SEO）は、検索エンジンから Web サイトへのトラフィック量を改善するための処理です。 検索エンジンはテキストベースのコンテンツに関する情報収集に優れていますが、動画に関する情報を十分に取得することはできません。 提供できるようになりました。

Adobe Dynamic Media Classic Video SEOを使用すれば、動画のメタデータを適用して、検索エンジンに動画の説明を提供できます。 Adobe Dynamic Media Classicでは、ビデオサイトマップとmRSS フィードを作成できます。 これらの標準XML ファイルは、検索エンジンにビデオ情報を送信するために使用されます。

* **ビデオサイトマップ**: サイト上のビデオコンテンツの場所と内容をGoogleに正確に通知します。 そのため、Googleでは動画を完全に検索できます。 例えば、ビデオサイトマップでビデオの実行時間とカテゴリを指定できます。 ビデオサイトマップについて詳しくは、[&#x200B; ビデオサイトマップとビデオサイトマップの代替案](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1)を参照してください。

* **mRSS （Media Really Simple Syndication）フィード**：コンテンツ発行者がYahoo! ビデオ検索にフィードするために使用されます。 mRSS フィードについて詳しくは、[&#x200B; ビデオサイトマップとビデオサイトマップの代替案](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1)を参照してください。

>[!NOTE]
>
>Google は、情報を検索エンジンに送信するためのビデオサイトマップおよび mRSS フィードプロトコルの両方をサポートしています。

Adobe Dynamic Media Classicでは、各動画に保存されているメタデータから動画サイトマップとmRSS フィードを生成できます。 ビデオサイトマップおよび mRSS フィードを作成する場合は、ビデオファイルから抽出するメタデータフィールドを指定します。 このように、検索エンジンに動画を説明することで、検索エンジンがweb サイト上の動画へのトラフィックをより正確に誘導できるようにします。

>[!NOTE]
>
>ビデオサイトマップまたは mRSS フィードを作成する前に、XML ファイル内で検索エンジンが必要とするフィールドとそれらのフィールドの構成を確認します。 ビデオサイトマップまたは mRSS フィードを正常に作成するには、検索エンジンの要件を満たす必要があります。

Adobe Dynamic Media Classicでは、ビデオ サイトマップとmRSS フィードの作成後に、これらのレポートを作成します。 これらのレポートは、ビデオ SEO レポートページで入手できます。

>[!NOTE]
>
>ビデオサイトマップおよびmRSS フィードの場合、Adobe Dynamic Media Classicは、公開用にマークされたビデオからのみメタデータをキャプチャします。 公開用のビデオにマークを付けて、ビデオサイトマップやmRSS フィードにメタデータを含めます。

## ビデオ SEO設定の選択

**[!UICONTROL ビデオ検索エンジン最適化設定]** ページで、ビデオサイトマップとmRSS フィードのビデオ SEO設定を選択します。 このページを開くには、グローバルナビゲーションバーで、**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Settings]**&#x200B;に移動します。

**[!UICONTROL 一般設定]**&#x200B;領域で、ビデオサイトマップ、mRSS フィード、またはその両方を生成するかどうかを選択します。 **[!UICONTROL 生成設定]**&#x200B;領域で、メタデータフィールドを入力フィールドにマッピングします。

設定を選択したら、**[!UICONTROL 保存]** （または&#x200B;**[!UICONTROL 保存と生成]**）を選択して、ビデオサイトマップ、mRSS フィード、またはその両方を作成します。

### 一般設定の設定 {#choosing-general-settings}

**[!UICONTROL 生成モード]** ドロップダウンリストで、レポートモードを選択します。

* **ビデオサイトマップ**：ビデオサイトマップを作成します。

* **mRSS フィード**: Media RSS （mRSS） フィードを作成します。

* **両方**：両方のタイプのXML ファイルを作成します。

* **オフ**：ビデオサイトマップおよびMedia RSS （mRSS）フィードの生成を停止するには、このオプションを選択します。

**[!UICONTROL 自動/手動モード]** ドロップダウンリストで、自動生成と手動生成のどちらかを選択します。

* **自動モード**: Adobe Dynamic Media Classicは、毎日1つのビデオサイトマップ、Media RSS （mRSS）フィード、またはその両方を自動的に生成します。 「**[!UICONTROL 公開用にマーク]**」オプションを選択すると、Adobe Dynamic Media Classicが生成するXML ファイルを自動的に公開用にマークできます。

   * **公開用にマーク**&#x200B;生成されたXML ファイルを公開用にマークします。

* **手動モード**: ビデオ検索最適化設定画面で「**[!UICONTROL 生成]**」または「**[!UICONTROL 保存と生成]**」を選択すると、Adobe Dynamic Media Classicによってビデオサイトマップ、Media RSS （mRSS）フィード、またはその両方が生成されます。 以下のオプションも同様に選択します。

   * **その他の設定はありません**：生成されたXML ファイルを公開するためのマークが付きません。

   * **公開用にマーク**：生成されたXML ファイルを公開用にマークします。

   * **部分生成を許可**：検索エンジンは、すべてのビデオの完全なメタデータ情報が含まれていないXML ファイルを拒否できます。 このオプションは、一部のビデオでメタデータが使用できない場合でも、XML ファイルを生成します。 この場合、レポート画面に警告が登録されます。 XML ファイルを書き出した後で、欠落している情報を手動で処理する場合は、このオプションを選択します。

### 生成設定の選択 {#choosing-generation-settings}

「生成設定」領域には、ビデオサイトマップ、mRSS フィード、またはその両方の入力フィールドが一覧表示されます。 メタデータパネルには、メタデータフィールドの名前が表示されます。 生成設定領域を使用して、入力フィールドをメタデータフィールドに割り当てます。 そうすることで、ビデオサイトマップやmRSS フィードのメタデータを取得する場所をAdobe Dynamic Media Classicに伝えることができます。

1. メタデータビューメニューで、メタデータビューを選択します。 ビューを選択したら、メタデータパネルにメタデータフィールドの名前が表示されます
詳しくは、[メタデータビュー](application-setup.md#metadata_views)を参照してください。
1. メタデータフィールド名をメタデータパネルから「ランディングページ」、「タイトル」、「説明」、「タグ」、「カテゴリ」の各入力フィールドにドラッグします。 「ランディングページ」、「タイトル」および「説明」フィールドは必須です。

   >[!NOTE]
   >
   >データを入力フィールドに手動で入力することもできます。

1. 次のいずれかの操作を行います。

   * XML ファイルを生成せずに設定を保存するには、**[!UICONTROL 保存]**&#x200B;を選択します。
   * ファイルを保存して生成するには、**[!UICONTROL 保存して生成]**&#x200B;を選択します。

     XML ファイルが生成され、ジョブログに記録されます。 ビデオサイトマップ（video-sitemap）およびメディア RSS（mRSS）フィード（mrss-feed）ファイルは、会社のルートフォルダに保存されます。

>[!NOTE]
>
>検索エンジンに送信する前に、ビデオサイトマップまたはmRSS フィードを公開します。 ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。 必要に応じて、これらのXML ファイルに公開用のマークを付け、**[!UICONTROL 公開]**&#x200B;を選択します。

## ビデオサイトマップとmRSS フィードのファイルを検索エンジンに送信 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

これらのURLの1つを検索エンジンのweb マスターツールにコピーして、ビデオサイトマップまたはMedia RSS （mRSS）フィードファイルを検索エンジンに送信します。

## 動画を見るSEO レポート {#viewing-video-seo-reports}

ビデオ検索エンジン最適化レポートページでビデオ SEO レポートを表示します。 このページを開くには、グローバルナビゲーションバーで、**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Video SEO]** > **[!UICONTROL Reports]**&#x200B;に移動します。

レポートの生成時にエラーが発生した場合は、レポート ページに表示されます。
