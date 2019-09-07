---
title: アップロードしたアセットの削除
seo-title: アップロードしたアセットの削除
description: 'null'
seo-description: アップロードされたアセットを削除する方法について説明します。
uuid: edd2b688- c377-4be1- ba16- d2dd2e6f716d
contentOwner: 管理者
content-type: 参照
products: SG_ PREPERNEMENTMANAGER/Dynamic- Media- Scene-7
discoiquuid: dd338c8c-06c6-44d5-8493- dc2087eeafb
translation-type: tm+mt
source-git-commit: 75f006fd81b0fe2dad5479cdd98e45eaada46b2a

---


# アップロードしたアセットの削除{#deleting-an-uploaded-asset}

`delete` パラメータをこの形式で使用すると、アセットを削除できます。

```as3
https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif
```

次に、画像アセットを削除した場合の応答例を示します。

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
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
|--- |--- |--- |
| op | 必須 | 削除 |
| shared_secret | 必須 | 会社の共有秘密キー. |
| <ul><li>画像の場合:image_ name</li><li>ベクトル：fxg_name</li></ul> | 必須 | 削除するアセットの名前。 |

**サンプル画像の URL：**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

**ベクトル URL例：**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg`
