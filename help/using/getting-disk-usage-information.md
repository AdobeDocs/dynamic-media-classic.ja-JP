---
title: ディスク使用量情報の取得
description: Adobe Dynamic Media Classicでディスク使用量情報を取得する方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
topic: Administration, Content Management
level: Intermediate
source-git-commit: f054057d383b26e9088582f418f62504c3f327d8
workflow-type: tm+mt
source-wordcount: '91'
ht-degree: 42%

---

# ディスク使用量情報の取得 {#get-disk-usage-information}

以下を使用すると、 `disk_info` 次の例に示すように、会社のディスク容量使用量に関する情報を取得するためのパラメーター。

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

応答は次のようになります。

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content - Images</serviceName> 
            <version>1.0.0</version> 
            <operationName>disk_info</operationName> 
            <serviceStatus>SUCCESS</serviceStatus> 
            <title>Disk Information for d03b7e0b-c9dc-4c6c-af0b-419beeea1c63</title> 
            <message>Total Space available = 1395402342400 bytes. Total Space used = 0 bytes.</message> 
        </response> 
    </user_generated_content> 
</scene7>
```

URL クエリ文字列で以下のフィールドを使用して、ディスク使用状況に関する情報を取得できます。

| URL パラメータ | 必須／オプション | 値 |
| --- | --- | --- |
| op | 必須 | disk_info |
| shared_secret | 必須 | 会社の共有秘密鍵であるキー |

以下のサンプルコードでは、000Company のディスク情報を取得します。

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
