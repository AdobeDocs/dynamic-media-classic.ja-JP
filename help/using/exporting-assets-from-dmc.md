---
title: Adobe Dynamic Media Classicからのアセットの書き出し
description: Adobe Dynamic Media Classicからアセットを書き出す方法を説明します。
contentOwner: Rick Brough
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Classic
geptopics: SG_SCENESEVENONDEMAND_PK/categories/managing_assets
feature: Dynamic Media Classic,Asset Management
role: User
exl-id: 5e3b0002-5ae2-4437-862f-caa098b04362
topic: Content Management
level: Intermediate
source-git-commit: bc3b696bfde0ed55894cdcbf3533299ae7697e98
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 38%

---

# Adobe Dynamic Media Classicからのアセットの書き出し{#exporting-assets-from-dmc}

Adobe Dynamic Media Classicで編集したアセットをローカルネットワークドライブに保存できます。 書き出されたアセットは、ダウンロード用または電子メールでの送信用に ZIP ファイルにまとめられます。

書き出しジョブの場合、圧縮 ZIP ファイルの最大ファイルサイズは 1 GB です。また、書き出しジョブごとに最大 500 個の合計アセットを使用できます。

Adobe Dynamic Media Classicは、ジョブ画面にジョブの書き出しを記録します。

**Adobe Dynamic Media Classicからアセットを書き出すには：**

1. 書き出すアセットを選択し、に移動します。 **[!UICONTROL ファイル]** > **[!UICONTROL Export]**.
1. 選択したアセットを書き出しウィンドウで、**[!UICONTROL 「イメージ」オプション]**&#x200B;をクリックしてから、次のオプションを指定します（ユーザが指定できるオプションは管理者が決定します）。

   * **[!UICONTROL プリセット]**：オプションで、画像プリセットを選択して、書き出し時にアセットを書式設定します。 「画像プリセット」を選択した場合、アセットは画像プリセットで定義されている形式を採用するため、その他の形式オプションを選択できなくなります。

   * **[!UICONTROL 変換]**：アセットファイルまたは元の画像を変換します。

   * **[!UICONTROL サイズ]**：標準サイズを選択できます。 または、以下から選択できます。 **[!UICONTROL その他]** から **[!UICONTROL サイズ]** ドロップダウン リストから目的の単位を選択し、幅と高さを指定します。

     関連トピック [メディアポータルユーザーが使用できる書き出しオプションを指定](specifying-export-options-available-media.md#specifying_export_options_available_to_media_portal_users).

   * **[!UICONTROL 形式]**：画像形式を選択します。

   * **[!UICONTROL カラー]**:RGB、CMYK またはグレーを選択します。

   * **[!UICONTROL 解決策]**:72 ppi、150 ppi または 300 ppi を選択します。

   * **[!UICONTROL ジョブ名]**：書き出しにジョブ名を割り当てることができます。

   * **[!UICONTROL E メールの送信先]**：オプション。 アセットを電子メールで送信する場合は、電子メールアドレスを入力します。 電子メールには URL が記載されていて、受信者はこの URL にアクセスしてアセットをダウンロードすることができます。

1. を選択 **[!UICONTROL Export]**.

次の 3 つの基本的な書き出し操作がサポートされています。

* 元のファイル（アセットの元のファイルを書き出す）
* プリセットを使用して変換（アセットの形式を設定するには画像プリセットを使用）
* プリセットなしの変換（書き出しダイアログを使用して画像修飾子を指定）

次のアセットタイプは書き出せません。その他はすべて書き出しを生成します。

* 画像セット
* レンダリングセット
* スピンセット
* メディアセット
* マルチビットレート設定
* eCatalog

また、テンプレートを「元のファイル」として書き出すことはできません。

変換を使用して次のアセットタイプを書き出すことができます。

* 画像
* テンプレート
* 調整した画像
* PDF（変換後のページを生成）
* PostScript®

書き出し対象として様々なアセットタイプを大量に選択すると、次のような動作になります。

* 書き出すことができないすべてのアセットタイプは、ジョブ送信前にリストから削除されます
* 変換が要求されると、変換可能なすべてのタイプが変換され、その他のすべてのタイプは元の形式で書き出されます
