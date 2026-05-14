---
title: Adobe Dynamic Media Classicからのアセットの書き出し
description: Adobe Dynamic Media Classicからアセットを書き出す方法について説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
autotag-review: '2026-05-13T19:47:10.191Z'
TQID: 'https://experienceleague.adobe.com/wE2C1kA1I2fYIkXCqMvw-hPWIV5GMcj1Y0-dgkALyyc'
product_v2:
  - id: beaff0dd-a904-4c6b-8290-b527cd877d75
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 0d05ca7402db1d8894db1127088905143fb97cff
workflow-type: tm+mt
source-wordcount: 443
ht-degree: 38%

---

# Adobe Dynamic Media Classicからのアセットの書き出し{#exporting-assets-from-dmc}

Adobe Dynamic Media Classicで編集したアセットは、ローカルネットワークドライブに保存できます。 書き出されたアセットは、ダウンロード用または電子メールでの送信用に ZIP ファイルにまとめられます。

書き出しジョブの場合、圧縮 ZIP ファイルの最大ファイルサイズは 1 GB です。 また、1つの書き出しジョブにつき、合計で最大500個のアセットを使用できます。

Adobe Dynamic Media Classicは、ジョブ画面にジョブを書き出す記録を保持します。

**Adobe Dynamic Media Classicからアセットを書き出すには：**

1. 書き出すアセットを選択し、**[!UICONTROL ファイル]**/**[!UICONTROL 書き出し]**&#x200B;に移動します。
1. 選択したアセットを書き出しウィンドウで、**[!UICONTROL 「イメージ」オプション]**&#x200B;をクリックしてから、次のオプションを指定します（ユーザが指定できるオプションは管理者が決定します）。

   * **[!UICONTROL プリセット]**：オプションで、書き出す際にアセットをフォーマットする画像プリセットを選択します。 「画像プリセット」を選択した場合、アセットは画像プリセットで定義されている形式を採用するため、その他の形式オプションを選択できなくなります。

   * **[!UICONTROL 変換]**: アセットファイルまたは元の画像を変換します。

   * **[!UICONTROL サイズ]**：標準サイズを選択できます。 または、**[!UICONTROL サイズ]** ドロップダウンリストから&#x200B;**[!UICONTROL その他]**&#x200B;を選択し、目的の測定単位を選択してから、幅と高さを指定できます。

     [Media Portal ユーザーが使用できる書き出しオプションの指定](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)も参照してください。

   * **[!UICONTROL 形式]**：画像形式を選択します。

   * **[!UICONTROL カラー]**: RGB、CMYK、またはグレーを選択します。

   * **[!UICONTROL 解決策]**: 72 ppi、150 ppi、または300 ppiを選択してください。

   * **[!UICONTROL ジョブ名]**: エクスポートにジョブ名を割り当てることができます。

   * **[!UICONTROL メールの送信先]**: オプション。 アセットを電子メールで送信する場合は、電子メールアドレスを入力します。 電子メールには URL が記載されていて、受信者はこの URL にアクセスしてアセットをダウンロードすることができます。

1. 「**[!UICONTROL 書き出し]**」を選択します。

次の 3 つの基本的な書き出し操作がサポートされています。

* 元のファイル（アセットの元のファイルを書き出す）
* プリセットを使用して変換（画像プリセットを使用してアセットをフォーマット）
* プリセットなしの変換（書き出しダイアログを使用して画像修飾子を指定）

次のアセットタイプは書き出せません。 その他の人は書き出しを生成します。

* 画像セット
* レンダリングセット
* スピンセット
* メディアセット
* マルチビットレートセット
* eCatalog

また、テンプレートを「元のファイル」として書き出すことはできません。

変換を使用して次のアセットタイプを書き出すことができます。

* 画像
* テンプレート
* 調整した画像
* PDF（変換されたページを生成）
* PostScript®

書き出し対象として様々なアセットタイプを大量に選択すると、次のような動作になります。

* 書き出すことができないすべてのアセットタイプは、ジョブの送信前にリストから削除されます
* 変換が要求された場合、変換できるすべてのタイプはオリジナルとして書き出されます
