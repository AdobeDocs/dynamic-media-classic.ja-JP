---
title: ディスク使用情報の取得
description: Adobe Dynamic Media Classicでディスク使用状況を取得する方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
feature: Dynamic Media Classic
role: Admin,User
exl-id: 337a4681-ac9a-40d9-82e8-1999bbed980c
topic: Administration, Content Management
level: Intermediate
autotag-review: '2026-05-13T19:50:49.049Z'
TQID: 'https://experienceleague.adobe.com/g-mRoL2yYGRH-uFr2ACD2qOxBAGUlMMtKKuKtsv2pQk'
product_v2: id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2: id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 92
ht-degree: 42%

---

# ディスク使用情報の取得 {#get-disk-usage-information}

次の例に示すように、`disk_info` パラメーターを使用して、会社のディスク容量の使用状況に関する情報を取得できます。

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=d03b7e0b-c9dc-4c6c-af0b-419beeea1c63
```

応答は次のようになります。

```as3
<?xml version="1.0" encoding="UTF-8" standalone="no" ?> 
<scene7> 
    <user_generated_content> 
        <response> 
            <serviceName>User Generated Content: Images</serviceName> 
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
| shared_secret | 必須 | 会社の共有秘密であるキー |

以下のサンプルコードでは、000Company のディスク情報を取得します。

```as3
https://s7ugc1.scene7.com/ugc/image?op=disk_info&shared_secret=fece4b21-87ee-47fc-9b99-2e29b78b9602
```
