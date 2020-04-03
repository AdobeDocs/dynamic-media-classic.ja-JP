---
title: 公開設定
seo-title: 公開設定
description: 'null'
seo-description: 公開設定画面の設定では、初期設定でアセットをDynamic Media ClassicサーバからWebサイトやアプリケーションに配信する方法を指定します。
uuid: 196f25c8-abf5-4c5d-8f6f-bc70007a0301
contentOwner: admin
content-type: reference
products: SG_EXPERIENCEMANAGER/Dynamic-Media-Scene-7
discoiquuid: cba59093-28b6-4490-b838-d942b72ad1ec
translation-type: tm+mt
source-git-commit: e3c64b90e0af0129571a21b132477c0c86d06405

---


# 公開設定 {#publish-setup}

公開設定画面の設定では、初期設定でアセットをDynamic Media ClassicサーバからWebサイトやアプリケーションに配信する方法を指定します。 設定を指定しない場合、Dynamic Media Classicサーバは、公開設定画面の初期設定に従ってアセットを配信します。 例えば、解像度属性が含まれていない画像を配信するように要求した場合、画像は Image Server 画面に指定されている初期設定のオブジェクト解像度設定で配信されます。

管理者は、Image Server 画面、画像レンダラ画面、ビネット画面の初期設定を変更して、サーバからアセットを配信するための初期設定を指定することができます。

公開設定画面を開くには、設定／アプリケーション設定／公開設定をクリックします。

>[!NOTE]
>
>公開設定画面は、詳しい知識がある Web サイト開発者またはプログラマ向けに用意されています。Dynamic Media Classicは、これらの画面の設定を変更するユーザが、Scene7 Publishing System、HTTPプロトコルの標準と表記、基本的な画像処理技術に精通していることを前提としています。

## Image Server {#image-server}

Image Server 画面では、Image Server から画像を配信するための初期設定を指定します。次の 5 つのカテゴリの設定を指定できます（設定について詳しくは、Image Server 画面を参照してください）。

これらの設定は、Dynamic Media Classicのサポート担当者の支援を受けた場合にのみ変更してください。

**カタログ管理** Scene7 Publishing Systemとカタログとの関係は、次の設定によって決まります。 ほとんどのWebサーバーとは異なり、Dynamic Media Image ServerのURL呼び出しは、適切な画像ファイルではなく、マニフェストまたはカタログファイルに送信されます。 カタログファイル（eCatalog と混同しないでください）には、Image Server に公開されたすべてのコンテンツのリストと、各画像へのパスが含まれています。Digimarc ID がある場合は、「Digimarc ユーザ情報」セクションにユーザ情報を入力します。

**属性を要求** ：これらの設定は、サーバから配信できる画像に制限を設けます。

**デフォルトの要求属性** ：これらの設定は、画像のデフォルトの外観に関係します。

**共通のサムネール属性** ：これらの設定は、サムネール画像の初期設定の外観と配置に関係します。

**カタログフィールドの初期設定** これらの設定は、画像の解像度と初期設定のサムネールタイプに関係します。

**カラーマネジメント属性** ：使用するICCカラープロファイルを指定します。

**互換性属性** この設定により、テキストレイヤーの先頭と末尾の段落が、後方互換性を保つためにバージョン3.6の場合と同じように扱われます。

**ローカライゼーションのサポート** これらの設定を使用すると、複数のロケール属性を管理できます。 また、ロケールマップ文字列を指定することもできます。これにより、ビューアのツールチップで使用する言語を指定できます。

例えば、様々な国で販売している多国籍ブランドである場合は、各国でロケール固有のビューアを使用できるようにすることができます。この機能を実現するには、ロケールマップ文字列を指定します。次に、必要な言語に翻訳したテキスト文字列を追加して、ビューアのプリセットのツールチップテキストを編集します。

>[!NOTE]
> ローカライゼーションサポートオプションを設定するには、Adobe Dynamic Media Classicテクニカルサポートにお問い合わせいただくか、s7support@adobe.comまで電子メールをお送りください。

**「ローカリゼーションサポート」**&#x200B;の設定について詳しくは、[アセットのローカリゼーションを設定する場合の考慮事項](publish-setup.md#considerations_when_setting_up_localization_of_assets)を参照してください。

### アセットのローカリゼーションを設定する場合の考慮事項 {#considerations-when-setting-up-localization-of-assets}

>[!NOTE]
>
>Scene7 Publishing Systemでロケールマップフィールドなどのローカライゼーションサポートオプションを設定する場合は、Adobe Dynamic Media Classicテクニカルサポートにお問い合わせください。 または、s7support@adobe.com まで電子メールをお送りください。

Scene7 Publishing System（SPS）を使用する一般的な方法は、e コマース Web サイトの製品画像を管理することです。国際的なビジネスでは、同じ製品のアセットの表示が国によって異なるという課題に直面します。通常、この相違はメディア全体のごくわずかな部分に関するものです。このような相違に対処するため、国ごとにすべてのアセットをコピーして異なる部分だけを上書きするのは大変な作業で、マスターアセットは 1 つという概念に矛盾します。このようなアセットの相違によって、オーディオトラックが異なる国別のビデオから、製品に使用される電源コードの違いという微妙ながらも重要な違いまで対応できます。Dynamic Media Classicでは、基本的なルックアップメカニズムを使用します。 Image Server が検索するアセットのサフィックスの順序を定義します（必要なロケールから始めます）。

**アセットのローカライズ**

IS（画像サービング）要求のロケールは、次の IS/IR（画像レンダリング）コマンドで識別されます。

`locale=`

このコマンドはロケール ID（locId）文字列を受け入れ、大文字小文字は区別しません。ロケール ID は通常、英文字と「_」を含む 2 ～ 6 文字の文字列です。

IS supports arbitrary printable ASCII strings.The `locale=` command has a global scope, meaning that it is applied to the entire request, including all nested IS and IR requests, referenced templates, and image layers. 要求ごとに複数のロケールを設定すること、例えばレイヤーごとに異なるロケールを設定することはできません。ただし、ネストされた要求での明示的なオーバーライドは可能だと考えられます。

If `locale=` is not specified, `attribute::DefaultLocale` is passed to the translation engines. Limited input validation is applied to the `locale=` value. Empty `locale=` values are permitted. Because `locale=` has a global scope, `attribute::DefaultLocale` is provided by the main catalog for the entire request.

Some of the benefits of using `locale=` and `attribute::DefaultLocale` include the following:

* 複数のロケールでコンテンツを共有できる。
* 汎用 ID を使用して、ロケール固有のコンテンツにアクセスできる。
* 命名規則やロケール固有のコンテンツの管理に柔軟性を持たせることができる（ロケールのプリフィックスとサフィックスの使い分けや、個別のカタログでロケール固有のコンテンツを使用するなど）。
* ロケール固有のバージョンに直接アクセスできる。
* 画像セットなどオブジェクトを集めたものに汎用参照を含め、ロケール固有のコンテンツを参照することができる。
* ローカリゼーションが必要となる、カタログで管理されるすべてのコンテンツ（画像、画像セット、ビネット、素材、ビューアの設定レコードなど）がサポートされる。
* IPS データベースや IS マニフェストのメカニズムの変更を最小限に抑えられる。
* RFC IS-63 を実装すると、ビデオやスキンなどの静的コンテンツのサポートが追加される。
* 初期設定のロケールを設定できる。

**アプリケーションのシナリオ**

| アプリケーション | シナリオ |
|--- |--- |
| ビューアのローカリゼーション | 静的コンテンツのカタログが実装されたら、ローカリゼーションは完全に locale= パラメータで制御されます。このパラメータは IS に対して行われたすべての要求に付加されます。設定レコードやスキン、スプラッシュ画面などに、ロケール固有のバリアントを含めたり含めなかったりすることができます。ローカライズされるコンテンツとその ID をビューアで識別する必要はなく、IS から適切なコンテンツが提供されます。 |
| 画像とビデオ | 多国籍企業では、多くの場合、汎用コンテンツとロケール固有のコンテンツを組み合わせて使用します。このメカニズムでは、画像やビデオの参照を汎用にし、ロケール固有のコンテンツがある場合は IS から提供することができます。 |
| 画像セットとメディアセット | 汎用の画像セットからビューアで処理されるロケール固有の画像セットへの変換によって、eCatalogが完全に異なる場合など、一部のロケールで画像セット全体が異なる場合があります。一般的に、汎用セット内の個々のIDはローカライズされたコンテンツを参照します。 例えば、電気製品のほとんどの画像をすべての言語で同一にし、コントロールパネルの画像だけ変えることができます。IS で ID が自動的に変換されるので、ロケール固有の画像セットを生成する必要はありません。 |

**アセットのローカリゼーションの実装**

Scene7 Publishing と画像サービングには、画像と静的コンテンツのローカリゼーションができるインターフェイスがあります。

ローカリゼーションを行わない場合、Image Server の URL は次のようになります。

`https://server/is/image/company/image`

With localization, an Image Server URL adds the `locale=` parameter to the path, as in the following:

`https://server/is/image/company/image?locale=de_DE`

On receipt of the http call by the Image Server, the `locale=` parameter is parsed through the localeMap field found in **Setup** > **Application Setup** > **Publish Setup** > **Image Server** > **Localization Support** group.

ロケールマップフィールドには、パイプ記号（|）で区切られたエントリのリストが含まれています。

各エントリには、コンマ区切りの値のリストが含まれています。The first value is the search value that is passed by the `locale=` parameter. その他の値はサフィックス値または置換値で、既存の画像に一致するまで順次検索されます。

サフィックス値または置換値が適用されるかどうかは、**設定**／**アプリケーション設定**／**公開設定**／**Image Server**／**ローカリゼーションサポート**&#x200B;グループのグローバルロケール設定によって決まります。

>[!NOTE]
>
>グローバルロケール設定は現在、Scene7 Publishing System のインターフェイス内でなく、API を使用して設定する場合のみ可能です。

**サフィックスの例**

| URL | localeMap ID | 結果 |
|--- |--- |--- |
| `https://server/is/image/company/image?locale=de_DE` | `de_DE,_DE,|fr_FR,_FR,` | GlobalLocale の定義はありません。ロケールパラメータ de_DE が、localeMap の最初のエントリに一致します。最初の対応する値 _DE がサフィックスとして追加され、image_DE というアセットの検索が Image Server で行われます。サーバで見つかった場合は、その画像が返されます。見つからなかった場合は、2 番目の値 &quot;&quot; がサフィックスとして使用され、その結果画像そのものが返されます。 |

**置換の例**

| URL | GlobalLocale ID と localeMap ID | 結果 |
|--- |--- |--- |
| `https://server/is/image/company/image-main-01?locale=de_DE` | `GlobalLocale=mainlocaleMap -` <br><br/> `de_DE,de,main|fr_FR,fr,main` | この置換の例では、GlobalLocale に main が設定されています。ロケールパラメータ de_DE が、localeMap の最初のエントリに一致します。GlobalLocale のサブ文字列が検索され、localeMap の最初の対応する値 de に置き換えられて image-de-01 になります。この画像が Image Server で見つかった場合は、その画像が返されます。見つからなかった場合は、2 番目の値に置き換えられて image-main-01 で検索されます。 |

URL でロケールが定義されていない場合、Image Server は DefaultLocale（定義されている場合）を取り込み、URL に適用します。

If an unknown or empty locale parameter is supplied with `locale=`, then the localeMap is scanned for the empty value “starting with,”. localeMap で、ロケールが不明の場合に適用する初期設定のロケールを含めるよう設定しておくことが重要です。

**defaultImage について**

Image Server は、要求されたロケールの選択肢を 1 つずつ検索します。一致するものがなかった場合、ロケールの選択肢が defaultImage に適用され、一致するバージョンが返されます。この結果、各ロケールにローカリゼーションなしの画像の選択肢が含まれるか、ローカライズされた defaultImage のバージョンが Scene7 Publishing System で使用可能になります。

**localeMap の検索のシナリオ**

次のロケールをサポートするとします。

`en, en_us, en_uk, de, de_at, de_de, fr`

You map these locales to the suffixes `_E`, `_G`, and `_F`, for English, German, and French, respectively. すべての例で、汎用の入力画像 ID は `myImg` です。

localeMap の検索の標準的な動作&#x200B;**

ロケール ID は対応するサフィックスにマップされます。カタログ内でロケール固有の ID が見つからない場合は、汎用 ID が使用されます。locSuffix の値が空の場合は汎用 ID にマップされることに注意してください。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,`

| locale= | 検索する出力 ID |
|--- |--- |
| en,en_us, en_uk | myImg_E,myImg |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| その他 | - |

ロケールが不明な場合の localeMap の検索&#x200B;**

不明なロケールを、特定の ID または汎用 ID にマップできます。この例では、不明なロケールを英語の ID に、英語の ID が存在しない場合は汎用 ID にマップできます。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,_E,`

| locale= | 検索する出力 ID |
|--- |--- |
| de,de_de,de_at | myImg_D,myImg |
| fr | myImg_F,myImg |
| その他 | myImg_E,myImg |

You could also have a dedicated locSuffix, such as U, just for unknown locales, and force to the default image if no `_U` exists, as in the following:

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,U`

または、次のように汎用 ID に直接マップできます。

`attribute::LocaleMap=en,_E,|en_us,_E,|en_uk,_E,|fr,_F,|de,_D,|de_at,_D,|de_de,_D,|,`

*多層検索を使用した localMap の検索*

ヨーロッパ、中東、北米などロケールをグループ化し、肌の露出度など地域の基準に対処することが望ましい場合が多くあります。多層検索を使用して、このような効果を実現することができます。

この例では、西欧で使用するコレクションと中東で使用するコレクションをサポートするとします。どちらのコレクションも汎用の画像コレクションに基づいて作成し、いくつかの画像を追加または変更します。Both collections are then further refined for specific locales, such as `m1, m2` for two middle-eastern variants, and `w1, w2,` and `w3` for three Western locales, except that images are shared for `w1` and `w3`. 不明なロケールは汎用のコレクションのみにマッピングされ、ロケール固有の画像にはアクセスされません。マッピングは次のようになります。

`attribute::LocaleMap=w1,-W,|w2,-W2,-W,|w3,-W,|m1,-M1,-M,|m2,-M2,-M,|,`

| locale= | 検索する出力 ID |
|--- |--- |
| w1, w3 | myImg-W, myImg |
| w2 | myImg-W2, myImg-W, myImg |
| m1 | myImg-M1, myImg-M, myImg |
| m2 | myImg-M2, myImg-M, myImg |
| その他 | mylmg |

*特定の ID の検索による localeMap の検索*

一部の画像の命名規則で、汎用の画像 ID がサポートされない場合があります。要求にある汎用 ID を、カタログ内の特定の ID にマップする必要があります。ただし、正確な特定の ID が不明な場合があります。

Using the first example as a basis, images for all languages may have the suffixes `_1`, `_2`, or `_3`. Images that are specific to French locales may have the suffixes `_22` or `_23` suffix. And images that are specific to German locales may have the suffixes `_470` or `_480`.

`attribute::LocaleMap=,_1,_2,_3|fr,_22,_23,_1,_2,_3|de,_470,_480,_1,_2,_3|de_at,_470,_480,_1,_2,_3|de_de,_470,_480,_1,_2,_3`

| locale= | 検索する出力 ID |
|--- |--- |
| fr | myImg_22, myImg_23, myImg_1, myImg_2, myImg_3 |
| de, de_at, de_de | myImg_470, myImg_480, myImg_1, myImg_2,myImg_3 |
| その他 | myImg_1, myImg_2, myImg_3 |

**ローカリゼーションサポートを実装する場合の重要な考慮事項**

* ローカリゼーションの使用は ID に基づく呼び出しに限られ、パスに基づくアセットの呼び出しには使用できません。したがって、ロケールを使用してビデオを呼び出す場合は、ビデオのフルパスではなく会社 ID またはアセット ID として呼び出す必要があります。つまり、rtmp のメソッドはパスに基づくビデオの呼び出しのみに使用できるので、ローカリゼーションでは使用できません。
* localeMap がアクティブな場合は、単一のビデオを含む混在メディアセットを使用できません。使用した場合は、このセットのコンテンツの呼び出しが失敗します。この問題の回避策として、単一のビデオをアダプティブビデオセットに追加することができます。追加したら、このアダプティブビデオセットを混在メディアセットに追加します。
* アダプティブビデオセットのコンテンツの要求など、ローカライズされない要求があります。したがって、アダプティブビデオセットをローカリゼーションで使用する場合は、アダプティブビデオセットを混在メディアセット内に配置してください。Then, call the set into a Mixed Media viewer with the `locale=` parameter.

## 画像レンダラ {#image-renderer}

画像レンダラ画面では、画像レンダリングサーバから画像セットを配信するための初期設定を指定します。次の 5 つのカテゴリの設定を指定できます（設定について詳しくは、Image Server 画面を参照してください）。

**カタログ管理** Scene7 Publishing Systemとカタログファイルとの関係は、これらの設定によって決まります。 Dynamic Media Classic Render ServerのURL呼び出しがカタログに対して行われ、カタログがサーバから画像を配信するための呼び出しが行われます。 これらの設定は、Dynamic Media Classicのサポート担当者の支援を受けた場合にのみ変更してください。

**Session Attributes** ：エラーパラメータ、相対画像URLのURL、およびオブジェクトの重なりを許可するかどうかを指定します。

**[既定のマテリアル属性** ]これらの設定は、画像の既定の解像度とシャープの設定を指定します。

**応答画像属性** ：これらの設定は、画像の初期設定の外観に関係します。

**カラーマネジメント属性** ：これらの設定は、画像の初期設定のカラー設定に関係します。

## ビネット {#vignette}

ビネット画面には、ビネットの初期設定の外観を指定するための設定があります（オプションについて詳しくは、ビネット画面を参照してください）。
