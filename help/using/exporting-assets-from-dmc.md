---
title: Adobe Dynamic Media Classicからのアセットの書き出し
description: Adobe Dynamic Media Classicからアセットを書き出す方法を説明します。
uuid: d42b7a73-80c0-4a9a-a04e-7ef53e6fcf22
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
discoiquuid: eb850ec7-a669-41ea-b2b0-4c9178e34f95
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
source-git-commit: 65e3b69bdcbd651a5f9ab100592217e61a8c05ef
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 51%

---

# Adobe Dynamic Media Classicからのアセットの書き出し{#exporting-assets-from-dmc}

Adobe Dynamic Media Classicで編集したアセットをローカルネットワークドライブに保存できます。 書き出されたアセットは、ダウンロード用または電子メールでの送信用に ZIP ファイルにまとめられます。

書き出しジョブの場合、圧縮 ZIP ファイルの最大ファイルサイズは 1 GB です。また、書き出しジョブあたり最大 500 個のアセットを指定できます。

Adobe Dynamic Media Classicは、ジョブ画面に書き出しジョブの記録を保持します。

**Adobe Dynamic Media Classicからアセットを書き出すには：**

1. 書き出すアセットを選択し、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL 書き出し]**.
1. 選択したアセットを書き出しウィンドウで、**[!UICONTROL 「イメージ」オプション]**&#x200B;をクリックしてから、次のオプションを指定します（ユーザが指定できるオプションは管理者が決定します）。

   * **[!UICONTROL プリセット]**  — オプションで、アセットを書き出す際の形式を設定する画像プリセットを選択します。 「画像プリセット」を選択した場合、アセットは画像プリセットで定義されている形式を採用するため、その他の形式オプションを選択できなくなります。

   * **[!UICONTROL コンバージョン]**  — アセットファイルまたは元の画像を変換します。

   * **[!UICONTROL サイズ]**  — 標準サイズを選択できます。 または、 **[!UICONTROL その他]** から **[!UICONTROL サイズ]** 」ドロップダウンリストから、目的の単位を選択し、幅と高さを指定します。

      関連トピック [Media Portal ユーザーが使用できる書き出しオプションを指定します](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL 形式]**  — 画像形式を選択します。

   * **[!UICONTROL カラー]** - 「RGB」、「CMYK」または「グレー」を選択します。

   * **[!UICONTROL 解像度]** - 72 ppi、150 ppi、または 300 ppi を選択します。

   * **[!UICONTROL ジョブ名]** ：書き出しにジョブ名を割り当てることができます。

   * **[!UICONTROL メール送信先]**  — アセットを電子メールで送信する場合は、必要に応じて電子メールアドレスを入力します。 電子メールには URL が記載されていて、受信者はこの URL にアクセスしてアセットをダウンロードすることができます。

1. 選択 **[!UICONTROL 書き出し]**.

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
* PDF（変換されたページを生成）
* PostScript®

書き出し対象として様々なアセットタイプを大量に選択すると、次のような動作になります。

* ジョブの送信前に、書き出せないすべてのアセットタイプがリストから削除されます。
* 変換が要求されている場合、変換可能なすべてのタイプは変換され、それ以外のすべては元のまま書き出されます。
