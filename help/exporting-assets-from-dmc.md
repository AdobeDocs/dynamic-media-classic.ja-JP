---
title: Dynamic Media Classicからのアセットの書き出し
description: Dynamic Media Classicからアセットを書き出す方法を説明します。
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic，アセット管理
role: Business Practitioner
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: 27d9a9b9f158846b54e4318119aec9e4dc9c4c0d
workflow-type: tm+mt
source-wordcount: '426'
ht-degree: 63%

---

# Dynamic Media Classicからのアセットの書き出し{#exporting-assets-from-dmc}

Dynamic Media Classicで編集したアセットをローカルネットワークドライブに保存できます。 書き出されたアセットは、ダウンロード用または電子メールでの送信用に ZIP ファイルにまとめられます。

書き出しジョブの場合、圧縮 ZIP ファイルの最大ファイルサイズは 1 GB です。また、1つの書き出しジョブに許可されるアセットの合計は最大500個です。

Dynamic Media Classicは、ジョブ画面に書き出しジョブの記録を保持します。

**Dynamic Media Classicからアセットを書き出すには：**

1. 書き出すアセットを選択し、**[!UICONTROL ファイル]**／**[!UICONTROL 書き出し]**&#x200B;を選択します。
1. 選択したアセットを書き出しウィンドウで、**「イメージ」オプション**&#x200B;をクリックしてから、次のオプションを指定します（ユーザが指定できるオプションは管理者が決定します）。

   * **プリセット**  — オプションで、アセットの書き出し時の形式を設定する「画像プリセット」を選択します。「画像プリセット」を選択した場合、アセットは画像プリセットで定義されている形式を採用するため、その他の形式オプションを選択できなくなります。

   * **変換**  — アセットファイルまたは元の画像を変換します。

   * **サイズ**  — 標準サイズを選択できます。または、サイズドロップダウンリストから&#x200B;**[!UICONTROL その他]**&#x200B;をクリックして、希望の測定単位を選択してから、幅と高さを指定します。****

      詳しくは、[Media Portal ユーザが使用できる書き出しオプションの指定](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users)も参照してください。

   * **形式**  — 画像形式を選択します。

   * **カラー**  - RGB、CMYKまたはグレーを選択します。

   * **解像度**  - 72 ppi、150 ppiまたは300 ppiを選択します。

   * **ジョブ名**  — エクスポートにジョブ名を割り当てることができます。

   * **電子メールの送信先**  — オプションで、アセットを電子メールで送信する電子メールアドレスを入力します。電子メールには URL が記載されていて、受信者はこの URL にアクセスしてアセットをダウンロードすることができます。

1. **[!UICONTROL 「ファイルのエクスポート」]**&#x200B;をクリックします。

次の 3 つの基本的な書き出し操作がサポートされています。

* 元のファイル（アセットの元のファイルを書き出す）
* プリセットを使用した変換（画像プリセットを使用してアセットをフォーマット）
* プリセットなしの変換（書き出しダイアログを使用して画像修飾子を指定）

次のアセットタイプは書き出せません。それ以外の場合は、書き出しが生成されます。

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
* PDF（変換後のページを生成）
* PostScript®

書き出し対象として様々なアセットタイプを大量に選択すると、次のような動作になります。

* ジョブの送信前に、書き出せないすべてのアセットタイプがリストから削除されます。
* 変換が要求されている場合、変換可能なすべてのタイプは変換され、それ以外のすべては元のまま書き出されます。
