---
title: 「クイックスタート：Media Portal»
description: Media Portalの各種テクニックや管理をすばやく習得するための概要とクイックスタートガイドです。
uuid: 0dbd6146-b392-4e03-955b-0b323b654b9f
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/media_portal
discoiquuid: 1385a092-0b2c-4e05-ad1e-ce3685022300
feature: Dynamic Media Classic,Collaboration,Asset Management
role: Administrator,Business Practitioner
exl-id: bff613c8-a93b-4cca-94db-8cad1cc36296
source-git-commit: c5c8c4f96f18339734f4441733cdb1e7f34d3071
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 73%

---

# クイックスタート：Media Portal{#quick-start-media-portal}

Media Portalを使用すると、会社は承認されたアセットを容易に取得、制御し、外部のパートナーやチャネル、および会社の内部ユーザーに配布できます。 このブラウザーベースの「セルフサービス」環境は、Dynamic Media Classicアセットに管理者が制御した「表示」をMedia Portalユーザーに提供し、アセットに簡単にアクセス、参照、検索、プレビューおよび会社が承認した形式で書き出すことができます。

管理者は、Media Portal でのアセットの表示、アクセス、使用方法を制御します。また、Media Portal インターフェイスを Web サイトとブランドに一致するようにカスタマイズできます。フォント、フォントカラー、フォントサイズを指定し、ロゴなどのブランディング要素をMedia Portalインターフェイスに組み込むことができます。

ここでは、Media Portal の管理方法をすばやく習得できるように、手順について簡潔に説明します。各手順の最後に、トピックのリンクをクリックして詳細を確認します。

## 1. Media Portal ユーザの役割について

Media Portal ユーザには、ユーザ、寄稿者、寄稿者ユーザの 3 つの役割があります。役割ごとに実行できる作業は異なります。例えば、寄稿者はファイルとフォルダの名前を変更したり、削除したりすることができますが、ユーザはこのどちらの作業も実行できません。様々な役割を理解することで、ユーザを追加するときに、ユーザに付与する責任を理解できます。

詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

## 2. ユーザ管理のためのグループの作成

グループは、ユーザがアクセスするフォルダおよびファイル、これらのフォルダおよびファイルでユーザが実行できることおよび使用可能な画像プリセットを指定します。管理者の最初の作業は、グループを作成することです。各グループについて、グループメンバーがアクセスできるフォルダ、ファイルおよび画像プリセットを指定します。また、読み取り、書き込みおよび削除の権限をグループメンバーに付与します。これらの権限によって、メンバーが、アクセスできるフォルダとファイルを参照、編集、名前変更、削除できるかどうかが指定されます。

詳しくは、[Media Portal グループの作成と管理](creating-media-portal-groups.md#creating_and_managing_media_portal_groups)を参照してください。

## 3. ユーザの追加

ユーザを追加する際、ユーザに役割（ユーザ、寄稿者または寄稿者ユーザ）を割り当てます。また、ユーザを 1 つまたは複数のグループに割り当てます。ユーザの追加を速やかに行うため、ユーザリストを CSV ファイル形式でアップロードできます。新しいユーザにはご案内の電子メールメッセージと Media Portal へのログオン手順が送信されます。

詳しくは、[Media Portal ユーザの追加と管理](adding-media-portal-users.md#adding_and_managing_media_portal_users)を参照してください。

## 4. FTP アカウントの管理

Media Portalに関連付けられ、Dynamic Media Classicアカウントの特定のフォルダーにマッピングされた個別のFTPアカウントを持つことができます。 この種の機能は、ユーザが個別の FTP アカウントを使用して、アカウントにデジタルアセットをアップロードできるようにすることを意味します。

[FTP アカウントの管理](ftp-accounts.md#managing_ftp_accounts)を参照してください。

>[!NOTE]
>
>Media Portal 管理者のみが、これらの FTP アカウントを管理できます。さらに、Media Portal 寄稿者ユーザの役割を持つユーザまたは Media Portal 寄稿者のみがファイルをアップロードできます。

詳しくは、[Media Portal ユーザの役割](media-portal-user-roles.md#media_portal_user_roles)を参照してください。

## 5. 書き出しオプションの指定

Media Portal ユーザは、ファイルを書き出すときに、ファイルの形式を変更してオリジナルのマスターファイルを書き出すことができます。ただし、ユーザにその権限があることが条件です。管理者は、ユーザによるファイルの書き出し方法を指定します。

詳しくは、[Media Portal ユーザが使用できる書き出しオプションの指定](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)を参照してください。

## 6. 画像プリセットの作成

画像プリセットは、画像を書き出すときにサイズ、画質、形式、解像度およびその他の画像の外観を変更する、一連の定義済みの設定です。画像プリセットを作成して、ユーザが書き出すときに画像の形式を変更する方法を制御できます。

詳しくは、[画像プリセットの作成と有効化](creating-enabling-image-presets.md#creating_and_enabling_image_presets)を参照してください。

## 7. メタデータプリセットとユーザ定義メタデータフィールドの作成

メタデータは、ファイルを記述し、識別します。アセットの検索と整理に使用されます。メタデータが正しく入力され、データを必要とするメタデータフィールドに値が入力されるようにするため、メタデータプリセットを作成できます。メタデータプリセットは、メタデータエントリの定義済みセットです。操作するファイルを一意に記述するメタデータフィールドを作成することもできます。

詳しくは、[メタデータの使用の効率化](making-efficient-metadata.md#making_more_efficient_use_of_metadata)を参照してください。

## 8. Media Portalページのカスタマイズ

Media Portalスタイル設定を使用すると、Media Portalページに会社のロゴと色をブランディングできます。 スタイル設定を使用して、会社のブランディングをMedia Portalに配置します。

[Media Portalページのカスタマイズ](customizing-media-portal-screen.md#customizing_the_media_portal_screen)を参照してください。
