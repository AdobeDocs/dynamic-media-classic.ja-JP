---
title: アセットを公開する前にテストする
description: アセットを公開する前にAdobe Dynamic Media Classicでアセットをテストする方法を説明します。
uuid: 5e8f3bec-6cf1-408e-8ea1-aebde0012a70
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
discoiquuid: 52fadf99-7d11-46f7-8483-a9f87ffc2f67
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
source-git-commit: d43b0791e67d43ff56a7ab85570b9639c2375e05
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 31%

---

# アセットを公開する前にテストする {#testing-assets-before-making-them-public}

セキュアテストを使用すると、セキュアテスト環境を定義し、IP アドレスと範囲の設定可能なセットに基づいて、堅牢な B2B ソリューションを構築できます。 この機能を使用すると、Adobe Dynamic Media Classicのデプロイメントとコンテンツ管理およびビジネスシステムのアーキテクチャを一致させることができます。

セキュアテストを実行すると、未公開のコンテンツを含むステージングバージョンの Web サイトをプレビューできます。

必要に応じて、以下の理由でアセットを公開する代わりに、ステージング環境を作成します。

* 正式にリリースする前に、Web サイトをプレビュー（ステージング Web サイト）
* B2B Web アプリケーションで価格を表示する eCatalog のように、制限付きアクセスを必要とするアセットを提供。
* 製品情報管理システム、顧客サービスアプリケーション、トレーニングサイトなどの一部として、ファイアウォールの背後でアセットを使用。

>[!NOTE]
>
>セキュアテストは、Adobe Dynamic Media Classicへのアクセスに影響しません。 Adobe Dynamic Media Classicのセキュリティは一貫しており、Adobe Dynamic Media Classicおよび関連する Web サービスにアクセスするための通常の資格情報が必要です。

## テスト作業をセキュリティで保護する方法 {#how-secure-testing-works}

ほとんどの企業は自社のインターネットをファイアウォールの背後で動作させています。インターネットへのアクセスは、特定のルート経由で可能であり、通常は制限された範囲のパブリック IP アドレスを経由します。

企業ネットワークから、 [https://www.whatismyip.com](https://www.whatismyip.com/) または、企業の IT 組織にこの情報を要求します。

セキュアテストを使用して、Adobe Dynamic Media Classicはステージング環境または内部アプリケーション用に専用の画像サーバーを確立します。 このサーバに対するあらゆる要求は、送信元 IP アドレスがチェックされます。着信要求が、承認された IP アドレスリストの中に含まれていない場合、失敗の応答が返されます。Adobe Dynamic Media Classicの会社管理者が、自社のセキュアテスト環境で使用する承認済み IP アドレスリストを設定します。

元のリクエストの場所を確認する必要があるので、セキュアテストサービスのトラフィックは、パブリックDynamic Media Image Server トラフィックのようなコンテンツ配布ネットワークを通じてルーティングされません。 セキュアテストサービスへのリクエストの待ち時間は、パブリックなDynamic Media Image Server に比べて若干長くなります。

非公開のアセットは、セキュアテストサービスでは直ちに使用可能になり、公開の必要はありません。この方法では、公開されている Image Server にアセットを公開する前にプレビューを実行できます。

>[!NOTE]
>
>セキュアテストサービスは、内部公開コンテキストで設定されたカタログサーバを使用します。 したがって、セキュアテストに公開するように会社が設定されている場合、Adobe Dynamic Media Classicでアップロードされたアセットは、セキュアテストサービスですぐに使用できるようになります。 この機能は、アセットがアップロード時に公開用にマークされているかどうかに関係なく当てはまります。

セキュアテストサービスは、現在、次のアセットのタイプと機能をサポートしています。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved “Render Server requests” from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 画像.
* ビネット（Render Server の要求）。
* Render Server リクエスト（サポート対象、ただしお客様が明示的にリクエストする必要あり）。
* 画像セット、eCatalog、レンダリングセットおよびメディアセットを含む各種セット。
* 標準のAdobe Dynamic Media Classicリッチメディアビューア
* Adobe Dynamic Media Classic OnDemand JSP ページ。
* PDF ファイルやプログレッシブ配信ビデオのような静的コンテンツ。
* HTTP ビデオストリーミング。
* プログレッシブビデオストリーミング。

現時点で、以下のアセットタイプと機能はサポートされていません。

* Adobe Dynamic Media Classic Info または eCatalog 検索
* RTMP ビデオストリーミング
* Web-to-Print
* UGC（ユーザー生成コンテンツ）サービス

>[!IMPORTANT]
>
>Adobe Dynamic Media Classicでの新規または既存の UGC ベクトル画像アセットのサポートは、2021 年 9 月 30 日に終了しました。

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

1. Adobeカスタマーケアに問い合わせ、お使いのアカウントでセキュアテストを有効にするよう依頼します。
1. Adobe Dynamic Media Classicのグローバルナビゲーションバーで、 **[!UICONTROL 設定]** > **[!UICONTROL 公開設定]** > **[!UICONTROL Image Server]**.
1. Image Server 公開ページの **[!UICONTROL 公開コンテキスト]** ドロップダウンリストで、「 **[!UICONTROL 画像サービングをテスト]**.
1. [ クライアントアドレスフィルタ ] で、 **[!UICONTROL 追加]**.
1. このチェックボックスをオンにしてアドレスを有効（オン）にし、それぞれのテキストフィールドに IP アドレスとネットマスクを入力します。

   >[!NOTE]
   >
   >単一の IP アドレスとネットマスクを追加すると、そのアドレスがアセット呼び出しをおこなうことができます。 ただし、追加するその他の IP アドレスおよびネットマスクは、アセット呼び出しをおこなうことはできません。 そのため、上記の手順でチェックボックスを無効（オフ）にして、IP アドレスとネットマスクを指定する機能をオフにすることを検討します。 これを有効に行うことは、許可を与える *すべて* アセット呼び出しをおこなう IP アドレス。すべて表示されます。

1. 次のいずれかの操作を行います。
   * IP アドレスをさらに追加する必要がある場合は、上の 2 つの手順を繰り返します。
   * 次の手順に進みます。
1. Image Server 公開ページの左下で、を選択します。 **[!UICONTROL 保存]**
1. 目的の画像をAdobe Dynamic Media Classicアカウントにアップロードします。

   詳しくは、 [ファイルをアップロード](uploading-files.md#uploading_files).

1. 画像に公開用にマークされているものと、そうでないものがあることを確認してから、公開ジョブを送信します。

   詳しくは、 [ファイルを公開](publishing-files.md#publishing_files).

1. セキュアテストサービスの名前を決定するには、 **[!UICONTROL 設定]** > **[!UICONTROL アプリケーション設定]** > **[!UICONTROL 一般設定]**.
1. アプリケーション全般設定ページのサーバグループの下で、**[!UICONTROL 「公開コンテキストのサーバ名のテスト」]**&#x200B;の右側にある名前を検索します。

Adobeケアに問い合わせて、サーバー名が見つからないか、サーバーへの URL が機能しない場合。

### Web サイトのバリエーションの準備

公開アセットと非公開アセットのそれぞれにリンクしている単一 Web サイトの 2 つのバリエーションが必要です。

* 公開バージョン — 従来のAdobe Dynamic Media Classic URL 構文を使用してアセットをリンクします。
* ステージングバージョン — 同じ構文を使用し、セキュアテストサイト名を使用してアセットをリンクします。

### テストの実行

以下のテストを実行します。

1. 自社ネットワーク内でアセットが表示されるかどうかをチェックします。

   以前に定義した IP アドレス範囲で識別される企業ネットワーク内から、Web サイトのステージングバージョンには、公開用にマークされているかどうかに関わらず、すべての画像が表示されます。 したがって、プレビューの承認や製品の起動の前に、誤って画像を使用可能にすることなくテストできます。

   サイトの公開バージョンに、以前にAdobe Dynamic Media Classicで実行された公開済みアセットが表示されることを確認します。

1. 会社のネットワークの外部からテストし、非公開アセット（つまり、公開用のマークが付いていないアセット）が第三者のアクセスから保護されていることを確認します。

   外部（自宅のコンピューターから、または 3G 接続経由）から会社のネットワークにアクセスし、サイトの公開バージョンですべての公開アセットが表示され、非公開コンテンツはいずれも表示されないことを確認します。

   ステージングバージョンで、どのアセットも表示されないことを確認します。承認されていない IP アドレスからセキュアテストサービスにアクセスしているからです。
