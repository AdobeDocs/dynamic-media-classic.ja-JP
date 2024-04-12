---
title: ビデオ SEO（検索エンジン最適化）
description: Adobe Dynamic Media Classicでビデオ SEO を設定する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: b2a6aeb1aab420803a8b7dafb0fdeda495e2a69b
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 30%

---

# ビデオ SEO（検索エンジン最適化）{#video-seo-search-engine-optimization}

検索エンジン最適化（SEO）は、検索エンジンから Web サイトへのトラフィック量を改善するための処理です。検索エンジンは、テキストベースのコンテンツに関する情報の収集には優れていますが、ビデオに関する情報は、検索エンジン向けに提供されていない場合には十分に取得できません。

Adobe Dynamic Media Classic Video SEO を使用すると、ビデオメタデータを適用して、ビデオの説明を検索エンジンに提供できます。 Adobe Dynamic Media Classicでは、ビデオサイトマップと mRSS フィードを作成できます。 検索エンジンにビデオ情報を送信するには、次の標準 XML ファイルを使用します。

* **ビデオサイトマップ** - サイト上のビデオコンテンツの場所と内容をGoogleに正確に伝えます。 そのため、ビデオはGoogleで完全に検索できます。 例えば、ビデオサイトマップでビデオの実行時間とカテゴリを指定できます。ビデオサイトマップについて詳しくは、を参照してください。 [ビデオサイトマップとビデオサイトマップの代替](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS （Media Really Simple Syndication）フィード** - コンテンツ発行者がメディアファイルを Yahoo！にフィードするために使用されます ビデオ検索にフィードするために使用されます。mRSS フィードについては、を参照してください。 [ビデオサイトマップとビデオサイトマップの代替](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google は、情報を検索エンジンに送信するためのビデオサイトマップおよび mRSS フィードプロトコルの両方をサポートしています。

Adobe Dynamic Media Classicは、各ビデオと共に保存されるメタデータからビデオサイトマップと mRSS フィードを生成できます。 ビデオサイトマップおよび mRSS フィードを作成する場合は、ビデオファイルから抽出するメタデータフィールドを指定します。この方法では、ビデオを検索エンジンに説明し、検索エンジンが web サイト上のビデオにより正確にトラフィックを誘導できるようにします。

>[!NOTE]
>
>ビデオサイトマップまたは mRSS フィードを作成する前に、XML ファイル内で検索エンジンが必要とするフィールドとそれらのフィールドの構成を確認します。ビデオサイトマップまたは mRSS フィードを正常に作成するには、検索エンジンの要件を満たす必要があります。

ビデオサイトマップと mRSS フィードを生成すると、Adobe Dynamic Media Classicはそれらに関するレポートを作成します。 これらのレポートは、ビデオ SEO レポート ページで利用できます。

>[!NOTE]
>
>ビデオサイトマップおよび mRSS フィードの場合、Adobe Dynamic Media Classicは、公開用にマークされたビデオからのみメタデータを取得します。 公開するビデオをマークして、ビデオサイトマップや mRSS フィードにメタデータを含めます。

## ビデオ SEO 設定の選択

でビデオサイトマップと mRSS フィードのビデオ SEO 設定を選択する **[!UICONTROL ビデオ検索エンジンの最適化設定]** ページ。 このページを開くには、グローバル ナビゲーション バーで次に移動します： **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビデオ SEO]** > **[!UICONTROL 設定]**.

が含まれる **[!UICONTROL 一般設定]** 領域で、ビデオサイトマップ、mRSS フィード、またはその両方を生成するかどうかを選択します。 が含まれる **[!UICONTROL 生成設定]** 領域で、メタデータフィールドを入力フィールドにマッピングします。

設定を選択した後、 **[!UICONTROL 保存]** （または **[!UICONTROL 保存して生成]**）、ビデオサイトマップ、mRSS フィード、またはその両方を作成します。

### 一般設定の指定 {#choosing-general-settings}

日 **[!UICONTROL 生成モード]** ドロップダウンリストから、レポートモードを選択します。

* **ビデオサイトマップ** - ビデオサイトマップを作成します。

* **mRSS フィード** - メディア RSS （mRSS）フィードを作成します。

* **両方** - 2 種類の XML ファイルを作成します。

* **オフ** - ビデオサイトマップとメディア RSS （mRSS）フィードの生成を停止するには、このオプションを選択します。

日 **[!UICONTROL 自動/手動モード]** ドロップダウンリストで、自動生成するか手動生成するかを選択します。

* **自動モード** - Adobe Dynamic Media Classicは、毎日、1 つのビデオサイトマップ、1 つのメディア RSS （mRSS）フィード、またはその両方を自動生成します。 「」を選択します **[!UICONTROL 公開用にマーク]** Adobe Dynamic Media Classicが生成する XML ファイルを公開用に自動的にマークするオプション。

   * **公開用にマーク** 生成された XML ファイルを公開するためのマークです。

* **手動モード** - Adobe Dynamic Media Classicは、選択すると、ビデオサイトマップ、メディア RSS （mRSS）フィード、またはその両方を生成します **[!UICONTROL Generate]** または **[!UICONTROL 保存して生成]** ビデオ検索最適化設定画面で、 以下のオプションも同様に選択します。

   * **その他の設定はありません**  – 生成された XML ファイルを公開用にマークしません。

   * **公開用にマーク**  – 生成された XML ファイルを公開するためのマーク。

   * **部分生成を許可**  – すべてのビデオの完全なメタデータ情報が XML ファイルに含まれていない場合、検索エンジンがその XML ファイルを拒否することがあります。 このオプションは、一部のビデオでメタデータを使用できない場合でも XML ファイルを生成します。 この場合、レポート画面に警告が登録されます。XML ファイルを書き出した後で、欠落している情報を手動で処理する場合は、このオプションを選択します。

### 生成設定の選択 {#choosing-generation-settings}

生成設定エリアには、ビデオサイトマップや mRSS フィードまたはその両方の入力フィールドと、メタデータパネルにあるメタデータフィールドの名前が一覧表示されます。 生成設定領域を使用して、入力フィールドをメタデータフィールドに割り当てます。これにより、ビデオサイトマップや mRSS フィードのメタデータを取得する場所をAdobe Dynamic Media Classicに指示します。

1. メタデータビューメニューで、メタデータビューを選択します。表示を選択すると、メタデータフィールドの名前がメタデータパネルに表示されます。
詳しくは、[メタデータビュー](application-setup.md#metadata_views)を参照してください。
1. メタデータフィールド名をメタデータパネルから「ランディングページ」、「タイトル」、「説明」、「タグ」、「カテゴリ」の各入力フィールドにドラッグします。「ランディングページ」、「タイトル」および「説明」フィールドは必須です。

   >[!NOTE]
   >
   >データを入力フィールドに手動で入力することもできます。

1. 次のいずれかの操作を行います。

   * XML ファイルを生成せずに設定を保存するには、次を選択します **[!UICONTROL 保存]**.
   * ファイルを保存して生成するには、次を選択します **[!UICONTROL 保存して生成]**.

     XML ファイルが生成され、ジョブログに記録されます。ビデオサイトマップ（video-sitemap）およびメディア RSS（mRSS）フィード（mrss-feed）ファイルは、会社のルートフォルダに保存されます。

>[!NOTE]
>
>検索エンジンに送信する前に、ビデオサイトマップまたは mRSS フィードを公開します。 ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。必要に応じてこれらの XML ファイルを公開用にマークし、を選択します。 **[!UICONTROL 公開]**.

## 検索エンジンへのビデオサイトマップおよび mRSS フィードファイルの送信 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

これらの URL のいずれかを検索エンジンの web マスターツールにコピーして、ビデオサイトマップまたはメディア RSS （mRSS）フィードファイルを検索エンジンに送信します。

## ビデオ SEO レポートを表示 {#viewing-video-seo-reports}

ビデオ検索エンジン最適化レポートページでビデオ SEO レポートを表示します。 このページを開くには、グローバル ナビゲーション バーで次に移動します： **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビデオ SEO]** > **[!UICONTROL 報告書]**.

レポートの生成時にエラーが発生した場合は、レポート ページにエラーが一覧表示されます。
