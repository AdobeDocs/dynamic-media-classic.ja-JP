---
title: アップロードしたラスター画像アセットの削除
description: Adobe Dynamic Media Classicでアップロードしたアセットを削除する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 33%

---

# アップロードしたアセットの削除{#deleting-an-uploaded-asset}

`delete` の形式のパラメーターを使用してアセットを削除できます。

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

次に、画像アセットを削除した場合の応答例を示します。

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>delete</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Delete request for1442564.tif</title> 
            <message>Your file was successfully deleted</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

URL クエリ文字列で以下のフィールドを使用して、アセットを削除できます。

| URL パラメータ | 必須／オプション | 値 |
| --- | --- | --- |
| `op` | 必須 | 削除 |
| `shared_secret` | 必須 | 会社の共有暗号鍵。 |
| `image_name` | 必須 | 削除するアセット名。 |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>2023 年 5 月 1 日（PT）以降、Dynamic Mediaの UGC アセットは、アップロード日から最大 60 日間使用できます。 60 日後にアセットが削除されます。

>[!NOTE]
>
>Adobe Dynamic Media Classicでの新規または既存の UGC ベクター画像アセットのサポートは、2021 年 9 月 30 日（PT）に終了しました。

**サンプル画像の URL：**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- **Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` -->
