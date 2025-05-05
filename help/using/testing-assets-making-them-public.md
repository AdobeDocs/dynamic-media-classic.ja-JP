---
title: アセットを公開する前にテストする
description: アセットを公開する前にAdobe Dynamic Media Classicでテストする方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
source-git-commit: 29752cf9eca0fc9bb760c721e1c3dc8e4ef912c3
workflow-type: tm+mt
source-wordcount: '1061'
ht-degree: 19%

---

# アセットを公開する前にテストする {#testing-assets-before-making-them-public}

セキュアテストを使用すると、設定可能な一連の IP アドレスと範囲に基づいて、セキュアテスト環境を定義し、堅牢な B2B ソリューションを作成できます。 この機能を使用すると、Adobe Dynamic Media Classicのデプロイメントと、コンテンツ管理およびビジネスシステムのアーキテクチャを一致させることができます。

セキュアテストを実行すると、未公開のコンテンツを含むステージングバージョンの Web サイトをプレビューできます。

必要に応じて、次の理由でアセットを公開する代わりに、ステージング環境を作成します。

* 正式にリリースする前に、Web サイトをプレビュー（ステージング Web サイト）
* B2B web アプリケーションで価格を表示する eCatalog など、制限付きアクセスを必要とするアセットを提供する。
* 製品情報管理システム、顧客サービスアプリケーション、トレーニングサイトなどの一部として、ファイアウォールの内側にあるアセットを使用する。

>[!NOTE]
>
>セキュアテストは、Adobe Dynamic Media Classicへのアクセスに影響しません。 Adobe Dynamic Media Classicのセキュリティは一貫しており、Adobe Dynamic Media Classicや関連する web サービスにアクセスするための通常の資格情報が必要です。

## テスト作業をセキュリティで保護する方法 {#how-secure-testing-works}

ほとんどの企業は自社のインターネットをファイアウォールの背後で動作させています。インターネットへのアクセスは、特定のルート経由で可能であり、通常は制限された範囲のパブリック IP アドレスを経由します。

企業ネットワークから、[https://www.whatismyip.com](https://www.whatismyip.com/) などの web サイトを使用してパブリック IP アドレスを把握するか、企業の IT 組織にこの情報をリクエストします。

セキュアテストを使用すると、Adobe Dynamic Media Classicは、ステージング環境または内部アプリケーション用に専用の Image Server を設定します。 このサーバに対するあらゆる要求は、送信元 IP アドレスがチェックされます。受信リクエストが IP アドレスの承認済みリストに含まれていない場合は、失敗の応答が返されます。 Adobe Dynamic Media Classic Company Administrator は、自社のセキュアテスト環境用の承認済み IP アドレスリストを設定します。

元のリクエストの場所を確認する必要があるので、セキュアテストサービスのトラフィックは、パブリックなDynamic Media Image Server トラフィックのようにコンテンツ配信ネットワークを通じてルーティングされません。 セキュアテストサービスへのリクエストの待ち時間は、パブリックなDynamic Media Image Server に比べて若干長くなります。

非公開のアセットは、セキュアテストサービスでは直ちに使用可能になり、公開の必要はありません。この方法では、公開されている Image Server にアセットを公開する前にプレビューを実行できます。

>[!NOTE]
>
>セキュアテストサービスは、内部公開コンテキストで設定されたカタログサーバーを使用します。 そのため、セキュアテストに公開するように会社が設定されている場合、Adobe Dynamic Media Classicにアップロードされたアセットは、セキュアテストサービスですぐに使用できます。 この機能は、アセットがアップロード時に公開用にマークされているかどうかに関係なく当てはまります。

セキュアテストサービスは、現在、次のアセットのタイプと機能をサポートしています。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 画像。
* ビネット（Render Server の要求）。
* Render Server リクエスト（サポート対象、ただし顧客が明示的にリクエストする必要あり）。
* 画像セット、eCatalog、レンダリングセットおよびメディアセットを含む各種セット。
* 標準のAdobe Dynamic Media Classic リッチメディアビューア。
* Adobe Dynamic Media Classic オンデマンド JSP ページ。
* PDF ファイルやプログレッシブ配信ビデオのような静的コンテンツ。
* HTTP ビデオストリーミング。
* プログレッシブビデオストリーミング。

現時点で、以下のアセットタイプと機能はサポートされていません。

* Adobe Dynamic Media Classic Info または eCatalog 検索
* RTMP ビデオストリーミング
* Web-to-Print
* UGC （ユーザー生成コンテンツ）サービス

>[!IMPORTANT]
>
>Adobe Dynamic Media Classicでの新規または既存の UGC ベクター画像アセットのサポートは、2021 年 9 月 30 日（PT）に終了しました。

## セキュアテストサービスのテスト {#testing-the-secure-testing-service}

セキュアテストサービスをテストして、期待どおりに動作することを確認できます。

<!-- >[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. -->

### アカウントの準備

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. Adobeのカスタマーケアに問い合わせ、お使いのアカウントでセキュアテストを有効にするようリクエストしてください。
1. Adobe Dynamic Media Classicのグローバルナビゲーションバーで、**[!UICONTROL 設定]**/**[!UICONTROL 2&rbrace;Publish設定]**/Image Server **に移動します。**
1. Image Server Publish ページの **[!UICONTROL `Publish Context`]** ドロップダウンリストで、「**[!UICONTROL 画像サービングをテスト]**」を選択します。
1. 「Client Address Filter」で「**[!UICONTROL Add]**」を選択します。
1. チェックボックスをオンにしてアドレスを有効にし、それぞれのテキストフィールドに IP アドレスとネットマスクを入力します。

   >[!NOTE]
   >
   >1 つの IP アドレスとネットマスクを追加すると、そのアドレスからアセットが呼び出される可能性があります。 ただし、追加したその他の IP アドレスおよびネットマスクでは、アセット呼び出しを行うことはできません。 そのため、上記の手順のチェックボックスを無効（オフ）にして、IP アドレスとネットマスクを指定する機能をオフにすることを検討します。 これにより、実質的に *すべて* の IP アドレスにアセット呼び出しを行うことが許可され、それらがすべて表示されます。

1. 次のいずれかの操作を行います。
   * さらに IP アドレスを追加する必要がある場合は、前の 2 つの手順を繰り返します。
   * 次の手順に進みます。
1. Image Server Publishページの左下で、「**[!UICONTROL 保存]**」を選択します
1. 目的の画像をAdobe Dynamic Media Classic アカウントにアップロードします。

   [ ファイルのアップロード ](uploading-files.md#uploading_files) を参照してください。

1. 一部の画像が公開用にマークされており、他の画像がマークされていないことを確認し、公開ジョブを送信します。

   [Publish ファイル ](publishing-files.md#publishing_files) を参照してください。

1. **[!UICONTROL 設定]**/**[!UICONTROL アプリケーション設定]**/**[!UICONTROL 一般設定]** に移動して、セキュアテストサービスの名前を決定します。
1. アプリケーション全般設定ページのサーバグループの下で、**[!UICONTROL 「公開コンテキストのサーバ名のテスト」]**&#x200B;の右側にある名前を検索します。

サーバー名がない場合またはサーバーへの URL が機能しない場合は、Adobeケアにお問い合わせください。

### Web サイトのバリエーションの準備

公開アセットと非公開アセットのそれぞれにリンクしている単一 Web サイトの 2 つのバリエーションが必要です。

* 公開バージョン：従来のAdobe Dynamic Media Classic URL 構文を使用してアセットをリンクします。
* ステージングバージョン：同じ構文でアセットをリンクしますが、セキュアテストサイト名を使用します。

### テストの実行

以下のテストを実行します。

1. 自社ネットワーク内でアセットが表示されるかどうかをチェックします。

   事前に定義した IP アドレス範囲によって識別される企業ネットワーク内からであれば、ステージングバージョンの web サイトは、公開用にマークされているかどうかにかかわらずすべての画像を表示します。 そのため、プレビューの承認や製品の発売前に、誤って画像を公開することなくテストできます。

   Adobe Dynamic Media Classicで以前に確認したように、公開バージョンのサイトに公開済みアセットが表示されていることを確認します。

1. 企業ネットワークの外部から、非公開のアセット（つまり、公開用にマークされていないアセット）がサードパーティのアクセスから保護されていることを確認します。

   外部（ホームコンピューターや 3G 接続など）からネットワークにアクセスし、公開バージョンのサイトに公開済みのアセットがすべて表示され、非公開のコンテンツは表示されないことを確認します。

   ステージングバージョンで、どのアセットも表示されないことを確認します。承認されていない IP アドレスからセキュアテストサービスにアクセスしているからです。
