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
source-git-commit: 61665faba1e6bb711aae5becf0150d1ebe3105c0
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 27%

---

# ビデオ SEO（検索エンジン最適化）{#video-seo-search-engine-optimization}

検索エンジン最適化（SEO）は、検索エンジンから Web サイトへのトラフィック量を改善するための処理です。検索エンジンは、テキストベースのコンテンツに関する情報の収集に優れていますが、ビデオに関する情報を適切に取得できません。 その情報は彼らに提供されなければなりません。

Adobe Dynamic Media Classic Video SEO を使用すると、ビデオメタデータを適用して、ビデオの説明を検索エンジンに提供できます。 Adobe Dynamic Media Classicでは、ビデオサイトマップと mRSS フィードを作成できます。 検索エンジンにビデオ情報を送信するには、次の標準 XML ファイルを使用します。

* **ビデオサイトマップ**：サイト上のビデオコンテンツの場所と内容をGoogleに正確に伝えます。 そのため、ビデオはGoogleで完全に検索できます。 例えば、ビデオサイトマップでビデオの実行時間とカテゴリを指定できます。ビデオサイトマップについて詳しくは、「[ ビデオサイトマップとビデオサイトマップの代替 ](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1)」を参照してください。

* **mRSS （Media Really Simple Syndication）フィード**：コンテンツ発行者がメディアファイルを Yahoo！にフィードするために使用します。 ビデオ検索にフィードするために使用されます。mRSS フィードについて詳しくは、「[ ビデオサイトマップとビデオサイトマップの代替 ](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&rd=1)」を参照してください。

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

**[!UICONTROL ビデオ検索エンジン最適化設定]** ページで、ビデオサイトマップと mRSS フィードのビデオ SEO 設定を選択します。 このページを開くには、グローバルナビゲーションバーで **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL ビデオ SEO]**/**[!UICONTROL 設定]** に移動します。

**[!UICONTROL 一般設定]** 領域で、ビデオサイトマップ、mRSS フィードまたはその両方を生成するかどうかを選択します。 「**[!UICONTROL 生成設定]**」領域で、メタデータフィールドを入力フィールドにマッピングします。

設定を選択したら、「**[!UICONTROL 保存]**」（または「**[!UICONTROL 保存して生成]**」を選択して、ビデオサイトマップ、mRSS フィード、またはその両方を作成します。

### 一般設定の指定 {#choosing-general-settings}

「**[!UICONTROL 生成モード]**」ドロップダウンリストで、レポートモードを選択します。

* **ビデオサイトマップ**：ビデオサイトマップを作成します。

* **mRSS フィード**: メディア RSS （mRSS）フィードを作成します。

* **両方**：両方のタイプの XML ファイルを作成します。

* **オフ**：ビデオサイトマップとメディア RSS （mRSS）フィードの生成を停止するには、このオプションを選択します。

**[!UICONTROL 自動/手動モード]** ドロップダウンリストで、自動生成するか手動生成するかを選択します。

* **自動モード**:Adobe Dynamic Media Classicでは、毎日 1 つのビデオサイトマップ、メディア RSS （mRSS）フィード、またはその両方が自動的に生成されます。 **[!UICONTROL 公開用にマーク]** オプションをオンにすると、Adobe Dynamic Media Classicで生成される XML ファイルを公開用に自動的にマークできます。

   * **公開用にマーク** 生成された XML ファイルを公開するためにマークします。

* **手動モード**: ビデオ検索最適化の設定画面で「**[!UICONTROL 生成]**」または「**[!UICONTROL 保存して生成]**」を選択すると、Adobe Dynamic Media Classicは、ビデオサイトマップ、メディア RSS （mRSS）フィード、またはその両方を生成します。 以下のオプションも同様に選択します。

   * **その他の設定なし**：生成された XML ファイルを公開するようにマークしません。

   * **公開用にマーク**：生成された XML ファイルを公開するためのマークです。

   * **部分生成を許可**：すべてのビデオの完全なメタデータ情報が含まれていない XML ファイルを、検索エンジンが却下することがあります。 このオプションは、一部のビデオでメタデータを使用できない場合でも XML ファイルを生成します。 この場合、レポート画面に警告が登録されます。XML ファイルを書き出した後で、欠落している情報を手動で処理する場合は、このオプションを選択します。

### 生成設定の選択 {#choosing-generation-settings}

「生成設定」領域に、ビデオサイトマップと mRSS フィードのいずれかまたは両方の入力フィールドが一覧表示されます。 メタデータパネルに、メタデータフィールドの名前が一覧表示されます。 生成設定領域を使用して、入力フィールドをメタデータフィールドに割り当てます。これにより、ビデオサイトマップや mRSS フィードのメタデータを取得する場所をAdobe Dynamic Media Classicに指示します。

1. メタデータビューメニューで、メタデータビューを選択します。表示を選択すると、メタデータフィールドの名前がメタデータパネルに表示されます。
詳しくは、[メタデータビュー](application-setup.md#metadata_views)を参照してください。
1. メタデータフィールド名をメタデータパネルから「ランディングページ」、「タイトル」、「説明」、「タグ」、「カテゴリ」の各入力フィールドにドラッグします。「ランディングページ」、「タイトル」および「説明」フィールドは必須です。

   >[!NOTE]
   >
   >データを入力フィールドに手動で入力することもできます。

1. 次のいずれかの操作を行います。

   * XML ファイルを生成せずに設定を保存するには、「**[!UICONTROL 保存]**」を選択します。
   * ファイルを保存して生成するには、「**[!UICONTROL 保存して生成]**」を選択します。

     XML ファイルが生成され、ジョブログに記録されます。ビデオサイトマップ（video-sitemap）およびメディア RSS（mRSS）フィード（mrss-feed）ファイルは、会社のルートフォルダに保存されます。

>[!NOTE]
>
>検索エンジンに送信する前に、ビデオサイトマップまたは mRSS フィードを公開します。 ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。必要に応じてこれらの XML ファイルを公開用にマークし、「**[!UICONTROL 公開]**」を選択します。

## 検索エンジンへのビデオサイトマップおよび mRSS フィードファイルの送信 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

これらの URL のいずれかを検索エンジンの web マスターツールにコピーして、ビデオサイトマップまたはメディア RSS （mRSS）フィードファイルを検索エンジンに送信します。

## ビデオ SEO レポートを表示 {#viewing-video-seo-reports}

ビデオ検索エンジン最適化レポートページでビデオ SEO レポートを表示します。 このページを開くには、グローバルナビゲーションバーで **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL ビデオ SEO]**/**[!UICONTROL レポート]** に移動します。

レポートの生成時にエラーが発生した場合は、レポート ページにエラーが一覧表示されます。
