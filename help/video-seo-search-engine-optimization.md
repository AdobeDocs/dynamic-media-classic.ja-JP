---
title: ビデオ SEO（検索エンジン最適化）
description: Dynamic Media ClassicでビデオのSEO設定を行う方法について説明します。
uuid: bac2c6a9-8466-4b8f-b835-6cb0b4168513
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/setup
discoiquuid: 34ecd868-775f-452b-b26e-d139f0e280ae
feature: Dynamic Media Classic
role: Admin
exl-id: f76b0e09-f148-46aa-b710-ec35bfebcb37
source-git-commit: 8bc49ae3704f0551c70d68a0ddd63725bdcc645c
workflow-type: tm+mt
source-wordcount: '1037'
ht-degree: 37%

---

# ビデオ SEO（検索エンジン最適化）{#video-seo-search-engine-optimization}

検索エンジン最適化（SEO）は、検索エンジンから Web サイトへのトラフィック量を改善するための処理です。検索エンジンは、テキストベースのコンテンツに関する情報の収集には優れていますが、ビデオに関する情報は、検索エンジン向けに提供されていない場合には十分に取得できません。

AdobeDynamic Media Classic Video SEOを使用すると、ビデオメタデータを適用して、ビデオの説明を検索エンジンに提供できます。 AdobeDynamic Media Classicでは、ビデオサイトマップとmRSSフィードを作成できます。 次の標準XMLファイルは、ビデオ情報を検索エンジンに送信する際に使用されます。

* **ビデオサイトマップ**  — サイト上のビデオコンテンツがどこに、何かをGoogleに正確に通知します。Google上でビデオを完全に検索できます 例えば、ビデオサイトマップでビデオの実行時間とカテゴリを指定できます。ビデオサイトマップについて詳しくは、[ビデオサイトマップとビデオサイトマップの代替](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1)を参照してください。

* **mRSS(Media Really Simple Syndication)フィード**  — コンテンツ発行者がメディアファイルをYahoo！にフィードするために使用します。ビデオ検索にフィードするために使用されます。mRSSフィードについて詳しくは、[ビデオサイトマップとビデオサイトマップの代替](https://developers.google.com/search/docs/advanced/sitemaps/video-sitemaps?visit_id=637558394348624754-567115452&amp;rd=1)を参照してください。

>[!NOTE]
>
>Google は、情報を検索エンジンに送信するためのビデオサイトマップおよび mRSS フィードプロトコルの両方をサポートしています。

AdobeDynamic Media Classicでは、各ビデオと共に保存されるメタデータからビデオサイトマップおよびmRSSフィードを生成できます。 ビデオサイトマップおよび mRSS フィードを作成する場合は、ビデオファイルから抽出するメタデータフィールドを指定します。このように、ビデオの説明を検索エンジンに提供することで、検索エンジンはトラフィックをより正確に Web サイト上のビデオに導くことができます。

>[!NOTE]
>
>ビデオサイトマップまたは mRSS フィードを作成する前に、XML ファイル内で検索エンジンが必要とするフィールドとそれらのフィールドの構成を確認します。ビデオサイトマップまたは mRSS フィードを正常に作成するには、検索エンジンの要件を満たす必要があります。

AdobeDynamic Media Classicは、ビデオサイトマップとmRSSフィードに関するレポートを生成後に作成します。 これらのレポートは、ビデオSEOレポートページで利用できます。

>[!NOTE]
>
>ビデオサイトマップおよびmRSSフィードの場合、AdobeDynamic Media Classicは、公開用にマークされたビデオのメタデータのみをキャプチャします。 ビデオサイトマップおよび mRSS フィードにメタデータを含めるビデオを公開用にマークします。

## ビデオSEO設定の選択 {#choosing-video-seo-settings}

**[!UICONTROL ビデオ検索エンジン最適化設定]**&#x200B;ページで、ビデオサイトマップおよびmRSSフィードのビデオSEO設定を選択します。 このページを開くには、グローバルナビゲーションバーで、**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL ビデオSEO]** / **[!UICONTROL 設定]**&#x200B;に移動します。

「**[!UICONTROL 一般設定]**」領域で、ビデオサイトマップを生成するか、mRSSフィードを生成するか、両方を生成するかを選択します。 「**[!UICONTROL 生成設定]**」領域で、メタデータフィールドを入力フィールドにマッピングします。

設定を選択した後、「**[!UICONTROL 保存]**」（または&#x200B;**[!UICONTROL 保存して生成]**）を選択して、ビデオサイトマップ、mRSSフィード、またはその両方を作成します。

### 一般設定の設定 {#choosing-general-settings}

「**[!UICONTROL 生成モード]**」ドロップダウンリストで、レポートモードを選択します。

* **ビデオサイトマップ**  — ビデオサイトマップを作成します。

* **mRSSフィード**  — メディアRSS(mRSS)フィードを作成します。

* **両方**  — 両方のタイプのXMLファイルを作成します。

* **オフ**  — ビデオサイトマップおよびメディアRSS(mRSS)フィードの生成を停止するには、このオプションを選択します。

**[!UICONTROL 自動/手動モード]**&#x200B;ドロップダウンリストで、自動生成するか手動で生成するかを選択します。

* **自動モード**  -AdobeDynamic Media Classicは、毎日1つのビデオサイトマップ、メディアRSS(mRSS)フィード、またはその両方を自動的に生成します。「**[!UICONTROL 公開用にマーク]**」オプションを選択すると、Dynamic Media Classicで生成されるXMLファイルを公開用に自動的にマークされます。

   * **生成されたXML** ファイルを発行するためのPublishMarks用のマーク。

* **手動モード**  -AdobeDynamic Media Classicは、ビデオ検索の最適化設定画面で「生成」または「保存して生成」を選択すると、ビデオサイトマップ、メディアRSS(mRSS)フィードまたはその両方を生成しま ****  **** す。以下のオプションも同様に選択します。

   * **それ以上の設定はありません**  — 生成されたXMLファイルを公開するようにマークしません。

   * **公開用にマーク**  — 生成されたXMLファイルを公開用のマーク。

   * **部分生成を許可**  — すべてのビデオの完全なメタデータ情報が含まれていない場合、検索エンジンはXMLファイルを拒否できます。このオプションを選択すると、一部のビデオでメタデータを使用できない場合でもXMLファイルが生成されます。 この場合、レポート画面に警告が登録されます。XML ファイルを書き出した後で、欠落している情報を手動で処理する場合は、このオプションを選択します。

### 生成設定の選択 {#choosing-generation-settings}

「生成設定」領域には、ビデオサイトマップ、mRSSフィード、またはその両方の入力フィールドがリストされ、メタデータパネルには、メタデータフィールドの名前が表示されます。 生成設定領域を使用して、入力フィールドをメタデータフィールドに割り当てます。これにより、AdobeDynamic Media Classicに、ビデオサイトマップやmRSSフィードのメタデータを取得する場所を指定します。

1. メタデータビューメニューで、メタデータビューを選択します。ビューを選択したら、メタデータパネルにメタデータフィールドの名前が表示されます詳しくは、[メタデータビュー](application-setup.md#metadata_views)を参照してください。
1. メタデータフィールド名をメタデータパネルから「ランディングページ」、「タイトル」、「説明」、「タグ」、「カテゴリ」の各入力フィールドにドラッグします。「ランディングページ」、「タイトル」および「説明」フィールドは必須です。

   >[!NOTE]
   >
   >データを入力フィールドに手動で入力することもできます。

1. 次のいずれかの操作を行います。

   * XMLファイルを生成せずに設定を保存するには、「**[!UICONTROL 保存]**」を選択します。
   * ファイルを保存して生成するには、「**[!UICONTROL 保存して生成]**」を選択します。

      XML ファイルが生成され、ジョブログに記録されます。ビデオサイトマップ（video-sitemap）およびメディア RSS（mRSS）フィード（mrss-feed）ファイルは、会社のルートフォルダに保存されます。

>[!NOTE]
>
>ビデオサイトマップまたはmRSSフィードを公開してから、検索エンジンに送信します。 ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。必要に応じて、これらのXMLファイルを公開用にマークし、「**[!UICONTROL 公開]**」を選択します。

## ビデオサイトマップおよびmRSSフィードファイルを検索エンジンに送信 {#submitting-video-sitemap-and-mrss-feed-files-to-search-engines}

ビデオサイトマップおよびメディア RSS（mRSS）フィードファイルは、会社のルートフォルダに保存されます。

* `https://{publish-server}/is/content/{companyname}/mrss-feed.xml`
* `https://{publish-server}/is/content/{companyname}/video-sitemap.xml`

これらの URL のいずれかを検索エンジンの Web マスターツールにコピーして、ビデオサイトマップまたはメディア RSS（mRSS）フィードファイルを検索エンジンに送信します。

## ビデオSEOレポートを表示 {#viewing-video-seo-reports}

ビデオ検索エンジン最適化レポートページでビデオSEOレポートを表示します。 このページを開くには、グローバルナビゲーションバーで、**[!UICONTROL 設定]** / **[!UICONTROL アプリケーション設定]** / **[!UICONTROL ビデオSEO]** / **[!UICONTROL レポート]**&#x200B;に移動します。

レポートの生成時にエラーが発生した場合は、そのエラーがレポートページに表示されます。
