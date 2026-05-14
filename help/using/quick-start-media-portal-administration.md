---
title: クイックスタート：Media Portal
description: Adobe Dynamic Media ClassicでMedia Portalのテクニックと管理を使用して、すばやく起動して実行できるようにするための概要とMedia Portalのクイックスタートを提供します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Admin,User
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
topic: Collaboration, Content Management
level: Beginner
autotag-review: '2026-05-13T20:10:17.674Z'
TQID: 'https://experienceleague.adobe.com/FSvq-Pe4KTPk2wslzWUkBExR1rZNQAqB90Xw5e-QT-Q'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 81e92d0e8963cccb5b058328cb7601925f7ace4f
workflow-type: tm+mt
source-wordcount: 859
ht-degree: 35%

---

# クイックスタート：Media Portal{#quick-start-media-portal}

Media Portalを利用すれば、承認されたアセットを取得、管理し、外部パートナーやチャネル、社内ユーザーに簡単に配布できます。 このブラウザーベースの「セルフサービス」環境では、Adobe Dynamic Media Classic アセットへの管理者による「ビュー」がMedia Portal ユーザーに提供され、企業が承認した形式でアセットに簡単にアクセス、参照、検索、プレビュー、書き出しが可能になります。

管理者は、Media Portal でのアセットの表示、アクセス、使用方法を制御します。 さらに、Web サイトとブランドに合わせてMedia Portal インターフェイスをカスタマイズできます。 フォント、フォントカラー、フォントサイズを指定し、ロゴなどのブランディング要素をMedia Portal インターフェイスに組み込むことができます。

次のトレーニングビデオを参照してください。

* [Media Portalの概要](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/544_mp_overview1_converted%20renamed_Done-AVS)

* [&#x200B; メディア ポータル ツアー1](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/545_mp_tour1_user_converted%20renamed_Done-AVS)

* [&#x200B; メディア ポータル ツアー2](https://s7d5.scene7.com/s7viewers/html5/VideoViewer.html?videoserverurl=https://s7d5.scene7.com/is/content/&emailurl=https://s7d5.scene7.com/s7/emailFriend&serverUrl=https://s7d5.scene7.com/is/image/&config=Scene7SharedAssets/Universal_HTML5_Video&contenturl=https://s7d5.scene7.com/skins/&asset=S7tutorials/546_mp_tour2_admin_converted%20renamed_Done-AVS)

次のクイックスタートは、Media Portalの管理を迅速に行えるように設計されています。 各ステップの最後に、トピックリンクを選択して詳細を確認します。

## &#x200B;1. Media Portal ユーザーの役割について

Media Portal ユーザーは、user、contributor、user-contributorの3つの役割に分類されます。 役割ごとに実行できる作業は異なります。 例えば、寄稿者はファイルとフォルダの名前を変更したり、削除したりすることができますが、ユーザはこのどちらの作業も実行できません。 様々な役割を理解することで、ユーザを追加するときに、ユーザに付与する責任を理解できます。

詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

## &#x200B;2. ユーザーを管理するためのグループの作成

グループは、ユーザがアクセスするフォルダおよびファイル、これらのフォルダおよびファイルでユーザが実行できることおよび使用可能な画像プリセットを指定します。 管理者の最初の作業は、グループを作成することです。 各グループについて、グループメンバーがアクセスできるフォルダ、ファイルおよび画像プリセットを指定します。 また、読み取り、書き込みおよび削除の権限をグループメンバーに付与します。 これらの権限によって、メンバーが、アクセスできるフォルダとファイルを参照、編集、名前変更、削除できるかどうかが指定されます。

[Media Portal グループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)を参照してください。

## &#x200B;3. ユーザーを追加

ユーザを追加する際、ユーザに役割（ユーザ、寄稿者または寄稿者ユーザ）を割り当てます。 ユーザーを1つ以上のグループに割り当てることもできます。 ユーザの追加を速やかに行うため、ユーザリストを CSV ファイル形式でアップロードできます。 新しいユーザにはご案内の電子メールメッセージと Media Portal へのログオン手順が送信されます。

[Media Portal ユーザーの追加と管理](adding-media-portal-users.md#adding_and_managing_media_portal_users)を参照してください。

## &#x200B;4. FTP アカウントの管理

Media Portalに関連付けられた個別のFTP アカウントを持つことができます。 Adobe Dynamic Media Classic アカウント内の特定のフォルダーにマッピングできます。 この種の機能は、ユーザが個別の FTP アカウントを使用して、アカウントにデジタルアセットをアップロードできるようにすることを意味します。

[FTP アカウントの管理](ftp-accounts.md#managing_ftp_accounts)を参照してください。

>[!NOTE]
>
>Media Portal管理者のみが、これらのFTP アカウントを管理できます。 さらに、Media Portal 寄稿者ユーザの役割を持つユーザまたは Media Portal 寄稿者のみがファイルをアップロードできます。

詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

## &#x200B;5. 書き出しオプションの指定

Media Portal ユーザーは、ファイルを書き出す際に、ファイルを再フォーマットし、元のプライマリファイルを書き出すことができます。このアクセス権を付与した場合に限ります。 管理者は、ユーザによるファイルの書き出し方法を指定します。

[Media Portal ユーザーが使用できる書き出しオプションの指定](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)を参照してください。

## &#x200B;6. 画像プリセットの作成

画像プリセットは、定義済みの設定のコレクションです。 これらの設定により、書き出し時の画像のサイズ、画質、形式、解像度などの外観を変更できます。 画像プリセットを作成して、ユーザが書き出すときに画像の形式を変更する方法を制御できます。

[画像プリセットの作成と有効化](creating-enabling-image-presets.md#creating_and_enabling_image_presets)を参照してください。

## &#x200B;7. メタデータプリセットとユーザー定義メタデータフィールドの作成

メタデータは、ファイルを記述および識別します。 アセットの検索と整理に使用されます。 メタデータプリセットを作成して、メタデータを正しく入力し、データを必要とするメタデータフィールドが入力されていることを確認できます。 メタデータプリセットは、メタデータエントリの定義済みセットです。 操作するファイルを一意に記述するメタデータフィールドを作成することもできます。

詳しくは、[メタデータの使用の効率化](making-efficient-metadata.md#making_more_efficient_use_of_metadata)を参照してください。

## &#x200B;8. Media Portal ページのカスタマイズ

Media Portalのスタイル設定を使用すると、Media Portal ページを会社のロゴとカラーでブランディングできます。 スタイル設定を使用して、Media Portalで会社のブランディングを設定します。

[&#x200B; メディアポータル ページのカスタマイズ &#x200B;](customizing-media-portal-screen.md#customizing_the_media_portal_screen)を参照してください。
