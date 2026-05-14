---
title: アップロードしたラスター画像アセットの削除
description: Adobe Dynamic Media Classicでアップロードしたアセットを削除する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: User
exl-id: d845bcb2-f914-4727-8df2-049dc172f266
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:44:43.552Z'
TQID: 'https://experienceleague.adobe.com/EVwriRMQMB9aO3j-cZeaFeZE3wVtbQmQZA67ioyUniI'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 141
ht-degree: 31%

---

# アップロードしたアセットの削除{#deleting-an-uploaded-asset}

この形式の`delete` パラメーターを使用して、アセットを削除できます。

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
| `shared_secret` | 必須 | 会社の共有秘密であるキー。 |
| `image_name` | 必須 | 削除するアセットの名前。 |

<!-- <li>For Vector:fxg_name</li> -->

>[!IMPORTANT]
>
>2023年5月1日（PT）以降、Dynamic MediaのUGC アセットは、アップロード日から最大60日間使用できるようになります。 60日後、アセットは削除されます。

>[!NOTE]
>
>Adobe Dynamic Media Classicでの新規または既存のUGC ベクター画像アセットのサポートは、2021年9月30日に終了しました。

**サンプル画像の URL：**

`https://s7ugc1.scene7.com/ugc/image?op=delete&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b602&image_name=1442564.tif`

<!-- 
**Sample vector URL:**

`https://s7ugc1.scene7.com/ugc/vector?op=delete&shared_secret=2160a8fa-cec6-45ba-8d59- ca595f6d2b47& &fxg_name=8875744.fxg` 
-->
