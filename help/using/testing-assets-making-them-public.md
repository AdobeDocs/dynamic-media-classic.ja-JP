---
title: アセットを公開する前にテストする
description: Adobe Dynamic Media Classicでアセットを公開する前にテストする方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/upload_and_publish_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: fd78d535-391e-43eb-a8aa-25fa6c2885cb
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T20:14:28.361Z'
TQID: 'https://experienceleague.adobe.com/cu99kXj4FjNzR74kGCoACFPst0snM2EGyYifu7a8Drs'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 1070
ht-degree: 21%

---

# アセットを公開する前にテストする {#testing-assets-before-making-them-public}

セキュアテストは、設定可能なIP アドレスと範囲のセットに基づいて、安全なテスト環境を定義し、堅牢なB2B ソリューションを構築するのに役立ちます。 この機能により、Adobe Dynamic Media Classicのデプロイメントと、CMSのアーキテクチャを一致させることができます。

セキュアテストを実行すると、未公開のコンテンツを含むステージングバージョンの Web サイトをプレビューできます。

必要に応じて、次の理由でアセットを公開するのではなく、ステージング環境を作成します。

* 正式にリリースする前に、Web サイトをプレビュー（ステージング Web サイト）
* B2B Web アプリケーションで価格を表示する電子カタログなど、アクセス制限のあるアセットを提供します。
* ファイアウォールの背後にあるアセットを、製品情報管理システム、カスタマーサービスアプリケーション、トレーニングサイトなどの一部として使用します。

>[!NOTE]
>
>セキュアテストは、Adobe Dynamic Media Classicへのアクセスには影響しません。 Adobe Dynamic Media Classicのセキュリティは一貫性を維持し、Adobe Dynamic Media Classicおよび関連するWeb サービスにアクセスするには、通常の資格情報が必要です。

## テスト作業をセキュリティで保護する方法 {#how-secure-testing-works}

ほとんどの企業は自社のインターネットをファイアウォールの背後で動作させています。 インターネットへのアクセスは、特定のルート経由で可能であり、通常は制限された範囲のパブリック IP アドレスを経由します。

企業ネットワークから、[https://www.whatismyip.com](https://www.whatismyip.com/)などのweb サイトを使用してパブリック IP アドレスを確認するか、企業のIT組織にこの情報を依頼できます。

セキュアテストでは、Adobe Dynamic Media Classicはステージング環境または内部アプリケーション用の専用Image Serverを確立します。 このサーバに対するあらゆる要求は、送信元 IP アドレスがチェックされます。 着信要求が、承認された IP アドレスリストの中に含まれていない場合、失敗の応答が返されます。 Adobe Dynamic Media Classic Company Administratorは、自社のセキュアテスト環境の承認済みIP アドレスのリストを設定します。

元のリクエストの場所を確認する必要があるため、セキュアテストサービスのトラフィックは、パブリック Dynamic Media Image Server トラフィックなどのコンテンツ配信ネットワークを介してルーティングされません。 セキュアテストサービスへのリクエストは、公開のDynamic Media Image Serverと比較して、若干高い遅延が発生します。

非公開のアセットは、セキュアテストサービスでは直ちに使用可能になり、公開の必要はありません。 これにより、アセットが公開される前に、プレビューを実行して、公開された画像サーバーにアセットを公開できます。

>[!NOTE]
>
>セキュアテストサービスでは、内部公開コンテキストで設定されたカタログサーバーを使用します。 したがって、会社がセキュアテストに公開するように設定されている場合、Adobe Dynamic Media Classicでアップロードされたアセットは、セキュアテストサービスですぐに利用できます。 この機能は、アセットがアップロード時に公開用にマークされているかどうかに関係なく当てはまります。

セキュアテストサービスは、現在、次のアセットタイプと機能をサポートしています。

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>Added videos to list below 9/11/2012. Moved "Render Server requests" from unsupported to supported, listed below on 3/15/2016 as per email from Cynthia March 11, 2016)</p>

 -->

* 画像：
* ビネット（Render Server の要求）。
* レンダーサーバーリクエスト（サポートされていますが、お客様は明示的にリクエストする必要があります）。
* 画像セット、eCatalog、レンダリングセットおよびメディアセットを含む各種セット。
* 標準のAdobe Dynamic Media Classic リッチメディアビューア。
* Adobe Dynamic Media Classic OnDemand JSP ページ。
* PDF ファイルやプログレッシブ配信ビデオのような静的コンテンツ。
* HTTP ビデオストリーミング。
* プログレッシブビデオストリーミング。

現時点で、以下のアセットタイプと機能はサポートされていません。

* Adobe Dynamic Media Classicの情報またはe カタログ検索
* RTMP ビデオストリーミング
* Web-to-Print
* UGC （ユーザー生成コンテンツ）サービス

>[!IMPORTANT]
>
>Adobe Dynamic Media Classicでの新規または既存のUGC ベクター画像アセットのサポートは、2021年9月30日に終了しました。

## セキュアテストサービスのテスト {#testing-the-secure-testing-service}

セキュアテストサービスをテストして、期待どおりに動作することを確認します。

<!-- 
>[!NOTE]
>
>*If you do not mention any IPs under **[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]** > **[!UICONTROL Test Image Service]***: If you add an IP only, that IP is able to call the assets and no other IP are allowed to make the calls. As long there is no IP mentioned under that section, all IPs are allowed to make the calls for the assets, and they show up. 
-->

### アカウントの準備

<!-- 

Comment Type: remark
Last Modified By: unknown unknown 
Last Modified Date: 

<p>RB: Rewrote entire steps under "Prepare your account" 9/10/2012</p>

 -->

1. Adobe カスタマーケアにお問い合わせいただき、お客様のアカウントでセキュアテストを有効にするようリクエストしてください。
1. Adobe Dynamic Media Classicのグローバルナビゲーションバーで、**[!UICONTROL Setup]** > **[!UICONTROL Publish Setup]** > **[!UICONTROL Image Server]**&#x200B;に移動します。
1. Image Server公開ページの&#x200B;**[!UICONTROL `Publish Context`]** ドロップダウンリストで、**[!UICONTROL 画像サービングのテスト]**&#x200B;を選択します。
1. クライアントのアドレスフィルターで、**[!UICONTROL 追加]**&#x200B;を選択します。
1. アドレスが有効（オン）になるようにチェックボックスを選択し、それぞれのテキストフィールドにIP アドレスとネットマスクを入力します。

   >[!NOTE]
   >
   >1つのIP アドレスとネットマスクを追加すると、そのアドレスがアセット呼び出しを行うことができます。 ただし、追加したその他のIP アドレスとネットマスクは、アセット呼び出しを行うことができません。 そのため、IP アドレスとネットマスクを指定する機能をオフにするには、上記の手順のチェックボックスを無効にする（オフにする）ことを検討してください。 これにより、*すべての*&#x200B;個のIP アドレスにアセット呼び出しを行う権限が効果的に付与され、すべて表示されます。

1. 次のいずれかの操作を行います。
   * IP アドレスをさらに追加する必要がある場合は、前の2つの手順を繰り返します。
   * 次のステップに進みます。
1. Image Server公開ページの左下にある「**[!UICONTROL 保存]**」を選択します
1. 目的の画像をAdobe Dynamic Media Classic アカウントにアップロードします。

   [ ファイルのアップロード ](uploading-files.md#uploading_files)を参照してください。

1. 一部の画像が公開用にマークされていることを確認し、他の画像がマークされていないことを確認してから、公開ジョブを送信します。

   [ ファイルの公開](publishing-files.md#publishing_files)を参照してください。

1. セキュアテストサービスの名前を決定するには、**[!UICONTROL Setup]** > **[!UICONTROL Application Setup]** > **[!UICONTROL General Settings]**&#x200B;に移動します。
1. アプリケーション全般設定ページのサーバグループの下で、**[!UICONTROL 「公開コンテキストのサーバ名のテスト」]**&#x200B;の右側にある名前を検索します。

サーバー名が見つからない場合や、サーバーへのURLが機能しない場合は、Adobeケアにお問い合わせください。

### Web サイトのバリエーションの準備

公開アセットと非公開アセットのそれぞれにリンクしている単一 Web サイトの 2 つのバリエーションが必要です。

* パブリックバージョン：従来のAdobe Dynamic Media Classic URL構文を使用してアセットをリンクします。
* ステージングバージョン：同じ構文を使用しますが、セキュアテストサイト名を使用してアセットをリンクします。

### テストの実行

以下のテストを実行します。

1. 自社ネットワーク内でアセットが表示されるかどうかをチェックします。

   以前に定義したIP アドレス範囲で識別された企業ネットワーク内から、web サイトのステージング版には、公開用にマークされているかどうかにかかわらず、すべての画像が表示されます。 そのため、プレビューの承認や製品のローンチの前に、誤って画像を使用可能にすることなくテストすることができます。

   公開済みサイトが、Adobe Dynamic Media Classicで以前に使用した公開済みアセットであることを確認します。

1. 企業ネットワーク外から、非公開アセット（公開用にマークされていないアセット）がサードパーティのアクセスから保護されていることを確認します。

   外部（ホームコンピューターや3G接続など）からネットワークにアクセスし、公開バージョンのサイトにすべての公開済みアセットが表示されますが、未公開のコンテンツが表示されないことを確認します。

   ステージングバージョンで、どのアセットも表示されないことを確認します。承認されていない IP アドレスからセキュアテストサービスにアクセスしているからです。
