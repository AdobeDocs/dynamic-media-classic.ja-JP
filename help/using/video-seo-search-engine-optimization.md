---
title: ビデオ SEO（検索エンジン最適化）
description: Adobe Dynamic Media Classicでビデオ SEO を設定する方法を説明します。
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
topic: Content Management
level: Intermediate
source-git-commit: 51c05c62448b39a75facb2e90cc9da5d0f26ab45
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 35%

---

# ビデオ SEO（検索エンジン最適化）{#video-seo-search-engine-optimization}

検索エンジン最適化（SEO）は、検索エンジンから Web サイトへのトラフィック量を改善するための処理です。検索エンジンは、テキストベースのコンテンツに関する情報の収集には優れていますが、ビデオに関する情報は、検索エンジン向けに提供されていない場合には十分に取得できません。

Adobe Dynamic Media Classic Video SEO を使用すると、ビデオメタデータを適用して、ビデオの説明を検索エンジンに提供できます。 Adobe Dynamic Media Classicでは、ビデオサイトマップと mRSS フィードを作成できます。 次の標準 XML ファイルは、ビデオ情報を検索エンジンに送信するために使用されます。

* **ビデオサイトマップ** :Googleに、サイト上のビデオコンテンツの場所と内容を正確に通知します。 そのため、ビデオはGoogleで完全に検索できます。 例えば、ビデオサイトマップでビデオの実行時間とカテゴリを指定できます。ビデオサイトマップについて詳しくは、 [ビデオサイトマップとビデオサイトマップの代替策](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

* **mRSS(Media Really Simple Syndication) フィード**  — コンテンツ発行者がメディアファイルを Yahoo! ビデオ検索にフィードするために使用されます。mRSS フィードについて詳しくは、 [ビデオサイトマップとビデオサイトマップの代替策](https://developers.google.com/search/docs/crawling-indexing/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1).

>[!NOTE]
>
>Google は、情報を検索エンジンに送信するためのビデオサイトマップおよび mRSS フィードプロトコルの両方をサポートしています。

Adobe Dynamic Media Classicは、各ビデオと共に保存されるメタデータからビデオサイトマップおよび mRSS フィードを生成できます。 ビデオサイトマップおよび mRSS フィードを作成する場合は、ビデオファイルから抽出するメタデータフィールドを指定します。このように、ビデオの説明を検索エンジンに提供することで、検索エンジンはトラフィックをより正確に Web サイト上のビデオに導くことができます。.

>[!NOTE]
>
>ビデオサイトマップまたは mRSS フィードを作成する前に、XML ファイル内で検索エンジンが必要とするフィールドとそれらのフィールドの構成を確認します。ビデオサイトマップまたは mRSS フィードを正常に作成するには、検索エンジンの要件を満たす必要があります。

ビデオサイトマップと mRSS フィードに関するレポートは、生成後にAdobe Dynamic Media Classicが作成します。 これらのレポートは、ビデオ SEO レポートページで使用できます。

>[!NOTE]
>
>ビデオサイトマップおよび mRSS フィードの場合、Adobe Dynamic Media Classicは公開用にマークされたビデオからのみメタデータをキャプチャします。 ビデオサイトマップおよび mRSS フィードにメタデータを含めるビデオを公開用にマークします。

## ビデオ SEO 設定を選択 {#choosing-video-seo-settings}

でビデオサイトマップおよび mRSS フィードのビデオ SEO 設定を選択します。 **[!UICONTROL ビデオ検索エンジン最適化設定]** ページに貼り付けます。 このページを開くには、グローバルナビゲーションバーで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビデオ SEO]** > **[!UICONTROL 設定]**.

Adobe Analytics の **[!UICONTROL 一般設定]** 領域で、ビデオサイトマップ、mRSS フィード、またはその両方を生成するかどうかを選択します。 Adobe Analytics の **[!UICONTROL 生成設定]** 「 」領域で、メタデータフィールドを入力フィールドにマッピングします。

設定を選択した後、 **[!UICONTROL 保存]** ( または **[!UICONTROL 保存して生成]**) をクリックして、ビデオサイトマップ、mRSS フィードまたはその両方を作成します。

### 一般設定の設定 {#choosing-general-settings}

次の日： **[!UICONTROL 生成モード]** ドロップダウンリストから、レポートモードを選択します。

* **ビデオサイトマップ**  — ビデオサイトマップを作成します。

* **mRSS フィード**  — メディア RSS(mRSS) フィードを作成します。

* **両方**  — 両方のタイプの XML ファイルを作成します。

* **オフ**  — ビデオサイトマップおよびメディア RSS(mRSS) フィードの生成を停止するには、このオプションを選択します。

次の日： **[!UICONTROL 自動/手動モード]** ドロップダウンリストで、自動生成するか手動で生成するかを選択します。

* **自動モード** - Adobe Dynamic Media Classicは毎日、1 つのビデオサイトマップ、メディア RSS(mRSS) フィード、またはその両方を自動的に生成します。 を選択します。 **[!UICONTROL 公開用にマーク]** Adobe Dynamic Media Classicが生成する XML ファイルを自動的に公開用にマークするオプション。

   * **公開用にマーク** 生成された XML ファイルを公開するためのマーク。

* **手動モード** - Adobe Dynamic Media Classicは、 **[!UICONTROL 生成]** または **[!UICONTROL 保存して生成]** （ビデオ検索の最適化設定画面）をクリックします。 以下のオプションも同様に選択します。

   * **その他の設定はありません**  — 生成される XML ファイルを公開するようにマークしません。

   * **公開用にマーク**  — 生成された XML ファイルを公開するためのマーク。

   * **部分生成を許可**  — すべてのビデオの完全なメタデータ情報が含まれていない場合、検索エンジンは XML ファイルを拒否できます。 このオプションを選択すると、一部のビデオでメタデータを使用できない場合でも XML ファイルが生成されます。 この場合、レポート画面に警告が登録されます。XML ファイルを書き出した後で、欠落している情報を手動で処理する場合は、このオプションを選択します。

### 生成設定の選択 {#choosing-generation-settings}

生成設定領域には、ビデオサイトマップや mRSS フィードの入力フィールド（またはその両方）が表示され、メタデータパネルにメタデータフィールドの名前が表示されます。 生成設定領域を使用して、入力フィールドをメタデータフィールドに割り当てます。これにより、ビデオサイトマップや mRSS フィードのメタデータを取得する場所をAdobe Dynamic Media Classicに指示します。

1. メタデータビューメニューで、メタデータビューを選択します。ビューを選択したら、メタデータパネルにメタデータフィールドの名前が表示されます詳しくは、[メタデータビュー](application-setup.md#metadata_views)を参照してください。
1. メタデータフィールド名をメタデータパネルから「ランディングページ」、「タイトル」、「説明」、「タグ」、「カテゴリ」の各入力フィールドにドラッグします。「ランディングページ」、「タイトル」および「説明」フィールドは必須です。

   >[!NOTE]
   >
   >データを入力フィールドに手動で入力することもできます。

1. 次のいずれかの操作を行います。

   * XML ファイルを生成せずに設定を保存するには、 **[!UICONTROL 保存]**.
   * ファイルを保存して生成するには、 **[!UICONTROL 保存して生成]**.

     XML ファイルが生成され、ジョブログに記録されます。ビデオサイトマップ（video-sitemap）およびメディア RSS（mRSS）フィード（mrss-feed）ファイルは、会社のルートフォルダに保存されます。

>[!NOTE]
>
>ビデオサイトマップまたは mRSS フィードを公開してから、検索エンジンに送信します。 ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。必要に応じて、公開用にこれらの XML ファイルをマークし、「 」を選択します。 **[!UICONTROL 公開]**.

## ビデオサイトマップおよび mRSS-Feed ファイルを検索エンジンに送信 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

これらの URL の 1 つを検索エンジンの Web マスターツールにコピーして、ビデオサイトマップまたはメディア RSS(mRSS) フィードファイルを検索エンジンに送信します。

## ビデオ SEO レポートを表示 {#viewing-video-seo-reports}

ビデオ検索エンジン最適化レポートページでビデオ SEO レポートを表示します。 このページを開くには、グローバルナビゲーションバーで、に移動します。 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL ビデオ SEO]** > **[!UICONTROL レポート]**.

レポートの生成時にエラーが発生した場合は、それらのエラーがレポートページに表示されます。
