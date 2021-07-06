---
title: アセットを公開する前のテスト
description: アセットを公開する前にテストする方法を説明します。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic，アセット管理
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: df689ff5a127bfbc400ca5331168d1ff7bb0b42e
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 37%

---

# アセットを公開する前のテスト {#testing-assets-before-making-them-public}

セキュアテストは、セキュアなテスト環境を定義し、IPアドレスと範囲の設定可能なセットに基づいて、堅牢なB2Bソリューションを構築するのに役立ちます。 この機能を使用すると、Dynamic Media Classicのデプロイメントと、コンテンツ管理およびビジネスシステムのアーキテクチャを一致させることができます。

セキュアテストを実行すると、未公開のコンテンツを含むステージングバージョンの Web サイトをプレビューできます。

必要に応じて、次の理由でアセットを公開するのではなく、ステージング環境を作成します。

* 正式にリリースする前に、Web サイトをプレビュー（ステージング Web サイト）
* B2B Web アプリケーションで価格を表示する eCatalog のように、制限付きアクセスを必要とするアセットを提供。
* 製品情報管理システム、顧客サービスアプリケーション、トレーニングサイトなどの一部として、ファイアウォールの背後でアセットを使用。

>[!NOTE]
>
>セキュアテストは、Dynamic Media Classicへのアクセスに影響しません。 Dynamic Media Classicのセキュリティは引き続き一貫しており、Dynamic Media Classicおよび関連するWebサービスにアクセスするための通常の資格情報が必要です。

## テスト作業をセキュリティで保護する方法 {#how-secure-testing-works}

ほとんどの企業は自社のインターネットをファイアウォールの背後で動作させています。インターネットへのアクセスは、特定のルート経由で可能であり、通常は制限された範囲のパブリック IP アドレスを経由します。

企業のネットワークから、 https://whatismyip.comなどのWebサイトを使用して公開IPアドレスを見つけたり、企業のIT組織にこの情報を要求したりできます。

セキュアテストを使用すると、Dynamic Media Classicは、ステージング環境または内部アプリケーション用に専用の画像サーバーを確立します。 このサーバに対するあらゆる要求は、送信元 IP アドレスがチェックされます。着信要求が、承認された IP アドレスリストの中に含まれていない場合、失敗の応答が返されます。Dynamic Media Classicの会社管理者が、自社のセキュアテスト環境用に承認されたIPアドレスのリストを設定します。

元のリクエストの場所を確認する必要があるので、セキュアテストサービスのトラフィックは、パブリックDynamic Media Image Serverトラフィックのようなコンテンツ配布ネットワークを通じてルーティングされません。 セキュアテストサービスへのリクエストの待ち時間は、パブリックなDynamic Media Image Serverに比べて若干長くなります。

非公開のアセットは、セキュアテストサービスでは直ちに使用可能になり、公開の必要はありません。この方法では、公開されているImage Serverにアセットを公開する前にプレビューを実行できます。

>[!NOTE]
>
>セキュアテストサービスは、内部公開コンテキストで設定されたカタログサーバーを使用します。 したがって、会社がセキュアテストに公開するように設定されている場合、Dynamic Media Classicにアップロードされたアセットは、セキュアテストサービスですぐに使用できます。 この機能は、アセットがアップロード時に公開用にマークされているかどうかに関係なく、有効です。

セキュアテストサービスは、現在、次のアセットタイプと機能をサポートしています。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 画像.
* ビネット（Render Server の要求）。
* Render Serverリクエスト（サポート対象、ただしお客様が明示的にリクエストする必要あり）。
* 画像セット、eCatalog、レンダリングセットおよびメディアセットを含む各種セット。
* 標準のDynamic Media Classicリッチメディアビューア。
* Dynamic Media Classic OnDemand JSPページ。
* PDF ファイルやプログレッシブ配信ビデオのような静的コンテンツ。
* HTTP ビデオストリーミング。
* プログレッシブビデオストリーミング。

現時点で、以下のアセットタイプと機能はサポートされていません。

* RTMP ビデオストリーミング
* UGC サービス
* Web-to-Print
* Dynamic Media Classic情報またはeCatalog検索

## セキュアテストサービスのテスト {#testing-the-secure-testing-service}

セキュアテストサービスをテストして、期待どおりに動作することを確認します。

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

1. Adobeカスタマーケアに連絡し、お客様のアカウントでセキュアテストを有効にするよう依頼します。
1. Dynamic Media Classicのグローバルナビゲーションバーで、**[!UICONTROL セットアップ]** / **[!UICONTROL 公開設定]** / **[!UICONTROL Image Server]**&#x200B;をクリックします。
1. Image Server公開ページの「**[!UICONTROL 公開コンテキスト]**」ドロップダウンリストで、「**[!UICONTROL 画像サービングをテスト]**」を選択します。
1. 「クライアントアドレスフィルタ」で、**[!UICONTROL 「追加」]**&#x200B;をクリックします。
1. チェックボックスをオンにしてアドレスを有効（オン）にし、各テキストフィールドにIPアドレスとネットマスクを入力します。

   >[!NOTE]
   >
   >1つのIPアドレスとネットマスクを追加すると、そのアドレスがアセット呼び出しをおこなう可能性があります。 ただし、追加するその他のIPアドレスおよびネットマスクは、アセット呼び出しをおこなうことはできません。 そのため、上記の手順のチェックボックスを無効（オフ）にして、IPアドレスとネットマスクを指定する機能をオフにすることを検討してください。 これにより、*すべての* IPアドレスがアセット呼び出しを実行でき、すべてのIPアドレスが表示されます。

1. 次のいずれかの操作を行います。
   * IPアドレスをさらに追加する必要がある場合は、上記の2つの手順を繰り返します。
   * 次の手順に進みます。
1. Image Server公開ページの左下にある「**[!UICONTROL 保存]**」をクリックします。
1. 目的の画像をDynamic Media Classicアカウントにアップロードします。

   詳しくは、[ファイルのアップロード](uploading-files.md#uploading_files)を参照してください。

1. 画像に公開用にマークされているものと、そうでないものがあることを確認してから、公開ジョブを送信します。

   詳しくは、[公開](publishing-files.md#publishing_files)を参照してください。

1. **[!UICONTROL 設定]**／**[!UICONTROL アプリケーション設定]**／**[!UICONTROL 全般設定]**&#x200B;をクリックして、セキュアテストサービスの名前を決定します。
1. アプリケーション全般設定ページのサーバグループの下で、**[!UICONTROL 「公開コンテキストのサーバ名のテスト」]**&#x200B;の右側にある名前を検索します。

Adobe名が見つからない場合や、サーバーへのURLが機能しない場合は、サーバーケアにお問い合わせください。

### Web サイトのバリエーションの準備

公開アセットと非公開アセットのそれぞれにリンクしている単一 Web サイトの 2 つのバリエーションが必要です。

* 公開バージョン — 従来のDynamic Media Classic URL構文を使用してアセットをリンクします。
* ステージングバージョン — 同じ構文を使用しながら、セキュアテストサイト名を使用してアセットをリンクします。

### テストの実行

以下のテストを実行します。

1. 自社ネットワーク内でアセットが表示されるかどうかをチェックします。

   以前に定義したIPアドレス範囲で識別された企業ネットワーク内から、Webサイトのステージングバージョンには、公開用にマークされているかどうかに関わらず、すべての画像が表示されます。 そのため、プレビューの承認や製品の発売の前に、誤って画像を使用可能にすることなく、テストをおこなうことができます。

   サイトの公開バージョンに、以前にDynamic Media Classicで経験した公開済みアセットが表示されることを確認します。

1. 会社のネットワークの外部からテストし、非公開アセット（つまり、公開用のマークが付いていないアセット）が第三者のアクセスから保護されていることを確認します。

   外部（自宅のコンピューターから、または 3G 接続経由）から会社のネットワークにアクセスし、サイトの公開バージョンですべての公開アセットが表示され、非公開コンテンツはいずれも表示されないことを確認します。

   ステージングバージョンで、どのアセットも表示されないことを確認します。承認されていない IP アドレスからセキュアテストサービスにアクセスしているからです。
