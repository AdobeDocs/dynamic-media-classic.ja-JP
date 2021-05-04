---
title: アセットを公開する前のテスト
description: アセットを公開する前にテストする方法を説明します。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Mediaクラシック，アセット管理
role: Business Practitioner
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
translation-type: tm+mt
source-git-commit: 1beb30b9eda4487dcd549034906079dee0b3149a
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 37%

---

# アセットを公開する前のテスト {#testing-assets-before-making-them-public}

セキュアテストを使用すると、セキュアテスト環境を定義し、設定可能なIPアドレスと範囲に基づいて堅牢なB2Bソリューションを構築するのに役立ちます。 この機能により、Dynamic Mediaクラシックのデプロイメントをコンテンツ管理とビジネスシステムのアーキテクチャに一致させることができます。

セキュアテストを実行すると、未公開のコンテンツを含むステージングバージョンの Web サイトをプレビューできます。

次の理由でアセットを公開できるようにする代わりに、必要に応じてステージング環境を作成します。

* 正式にリリースする前に、Web サイトをプレビュー（ステージング Web サイト）
* B2B Web アプリケーションで価格を表示する eCatalog のように、制限付きアクセスを必要とするアセットを提供。
* 製品情報管理システム、顧客サービスアプリケーション、トレーニングサイトなどの一部として、ファイアウォールの背後でアセットを使用。

>[!NOTE]
>
>セキュアテストは、Dynamic Mediaクラシックへのアクセスに影響を与えません。 Dynamic Mediaクラシックのセキュリティは引き続き一貫しており、Dynamic Mediaクラシックおよび関連Webサービスへのアクセスに必要な通常の資格情報が必要です。

## テスト作業をセキュリティで保護する方法 {#how-secure-testing-works}

ほとんどの企業は自社のインターネットをファイアウォールの背後で動作させています。インターネットへのアクセスは、特定のルート経由で可能であり、通常は制限された範囲のパブリック IP アドレスを経由します。

会社のネットワークから、https://whatismyip.comなどのWebサイトを使用してパブリックIPアドレスを知るか、会社のIT組織にこの情報を要求できます。

セキュアテストを実行すると、Dynamic Mediaクラシックは、ステージング環境または内部アプリケーション用の専用のImage Serverを確立します。 このサーバに対するあらゆる要求は、送信元 IP アドレスがチェックされます。着信要求が、承認された IP アドレスリストの中に含まれていない場合、失敗の応答が返されます。Dynamic Mediaクラシック会社管理者は、会社のセキュアテスト環境用に承認されたリストのIPアドレスを設定します。

元の要求の場所を確認する必要があるので、セキュアテストサービスのトラフィックは、公開のDynamic MediaImage Serverトラフィックなどのコンテンツ配信ネットワークを経由しません。 セキュアテストサービスへの要求の待ち時間は、パブリックDynamic Mediaイメージサーバーと比較して若干長くなります。

非公開のアセットは、セキュアテストサービスでは直ちに使用可能になり、公開の必要はありません。この方法により、アセットを公開用Image Serverに公開する前に、プレビューを実行できます。

>[!NOTE]
>
>セキュアテストサービスは、内部公開コンテキストで設定されたカタログサーバを使用します。 したがって、会社がセキュアテストに発行するように設定されている場合、Dynamic Mediaクラシックでアップロードされたアセットは、セキュアテストサービスで直ちに使用できるようになります。 この機能は、アップロード時にアセットが公開用にマークされているかどうかに関係なく実行されます。

セキュアテストサービスでは、現在、次のアセットタイプと機能をサポートしています。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 画像.
* ビネット（Render Server の要求）。
* Render Serverリクエスト（サポート対象。ただし、お客様が明示的にリクエストする必要あり）
* 画像セット、eCatalog、レンダリングセットおよびメディアセットを含む各種セット。
* 標準のDynamic Mediaクラシックリッチメディアビューア。
* Dynamic MediaクラシックOnDemand JSPページ。
* PDF ファイルやプログレッシブ配信ビデオのような静的コンテンツ。
* HTTP ビデオストリーミング。
* プログレッシブビデオストリーミング。

現時点で、以下のアセットタイプと機能はサポートされていません。

* RTMP ビデオストリーミング
* UGC サービス
* Web-to-Print
* Dynamic Mediaクラシック情報またはeCatalog検索

## セキュアテストサービスのテスト {#testing-the-secure-testing-service}

セキュアテストサービスをテストし、期待どおりに動作することを確認します。

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]*** - If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### アカウントの準備

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under “Prepare your account” 9/10/2012</p>

 -->

1. Adobeカスタマーケアに連絡し、お客様のアカウントでセキュアテストを有効にするようにリクエストします。
1. Dynamic Mediaクラシックのグローバルナビゲーションバーで、**[!UICONTROL セットアップ]**/**[!UICONTROL 公開設定]**/**[!UICONTROL Image Server]**&#x200B;をクリックします。
1. Image Server公開ページの&#x200B;**[!UICONTROL 公開コンテキスト]**&#x200B;ドロップダウンリストで、「**[!UICONTROL 画像サービングをテスト]**」を選択します。
1. 「クライアントアドレスフィルタ」で、**[!UICONTROL 「追加」]**&#x200B;をクリックします。
1. チェックボックスをオンにしてアドレスを有効（オン）にし、IPアドレスとネットマスクをそれぞれのテキストフィールドに入力します。

   >[!NOTE]
   >
   >1つのIPアドレスとネットマスクを追加すると、そのアドレスによってアセットが呼び出される場合があります。 ただし、追加するその他のIPアドレスおよびネットマスクは、アセット呼び出しを行うことはできません。 そのため、上記の手順のチェックボックスを無効（オフ）にして、IPアドレスとネットマスクを指定する機能をオフにすることを検討してください。 これにより、*すべての* IPアドレスに対してアセット呼び出しを行うことが効果的に許可され、すべてが表示されます。

1. 次のいずれかの操作を行います。
   * IPアドレスをさらに追加する必要がある場合は、前の2つの手順を繰り返します。
   * 次の手順に進みます。
1. Image Server公開ページの左下の「**[!UICONTROL 保存]**」をクリックします。
1. 目的の画像をDynamic Mediaクラシックアカウントにアップロードします。

   詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

1. 画像に公開用にマークされているものと、そうでないものがあることを確認してから、公開ジョブを送信します。

   詳しくは、[公開](publishing-files.md#publishing_files)を参照してください。

1. **[!UICONTROL 設定]**／**[!UICONTROL アプリケーション設定]**／**[!UICONTROL 全般設定]**&#x200B;をクリックして、セキュアテストサービスの名前を決定します。
1. アプリケーション全般設定ページのサーバグループの下で、**[!UICONTROL 「公開コンテキストのサーバ名のテスト」]**&#x200B;の右側にある名前を検索します。

サーバー名が見つからない場合や、AdobeへのURLが機能しない場合は、サーバーケアにお問い合わせください。

### Web サイトのバリエーションの準備

公開アセットと非公開アセットのそれぞれにリンクしている単一 Web サイトの 2 つのバリエーションが必要です。

* 公開バージョン — 従来のDynamic MediaクラシックURL構文を使用してアセットをリンクします。
* ステージングバージョン — 同じ構文を使用し、セキュアテストサイト名を持つリンクアセット。

### テストの実行

以下のテストを実行します。

1. 自社ネットワーク内でアセットが表示されるかどうかをチェックします。

   以前に定義したIPアドレスの範囲で識別された会社のネットワーク内では、公開のマークが付いているかどうかに関係なく、ステージングバージョンのWebサイトにすべての画像が表示されます。 したがって、プレビューの承認や製品の発売前に、画像を誤って使用可能にすることなく、テストを行うことができます。

   サイトの公開バージョンで、以前にDynamic Mediaクラシックで経験したとおりに公開アセットが表示されていることを確認します。

1. 会社のネットワークの外部からテストし、非公開アセット（つまり、公開用のマークが付いていないアセット）が第三者のアクセスから保護されていることを確認します。

   外部（自宅のコンピューターから、または 3G 接続経由）から会社のネットワークにアクセスし、サイトの公開バージョンですべての公開アセットが表示され、非公開コンテンツはいずれも表示されないことを確認します。

   ステージングバージョンで、どのアセットも表示されないことを確認します。承認されていない IP アドレスからセキュアテストサービスにアクセスしているからです。
