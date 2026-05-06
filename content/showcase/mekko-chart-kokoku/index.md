---
title: 二つの変数を総当たりにみるメッコ・チャート
description: 
slug: "mekko-chart-kokoku"
weight: 1
categories: "showcase"
image: "images/kokoku_fin.png"
---

毎年電通さんが公表している「日本の広告費」。業種ごとのインターネットを覗く四媒体別広告費を可視化しました。

![完成図](images/kokoku_fin.png)

通常、棒グラフか円グラフを使うと、業種数（21つ）か媒体数（4つ）だけチャートを作成する必要がありますが、メッコ・チャートであれば、縦横の比率としてこれらを一つのチャートで表現することができます。

ここでは本サービスのツールを用いた作成の仕方を紹介します。

{{< external-link-card
    url="https://rawgraphs.dataviz.jp/?project_id=cff8e9c7-e4bf-4d82-b3f5-e7a6fbe55212"
    title="業種別 マスコミ四媒体別広告費（2025年）"
    image="images/kokoku_fin.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

有料ユーザーであれば、上記リンクから編集可能なプロジェクト・ファイルとして開くことができ、作り方を学んだり、データのあり方を確認することができます。

データについては、電通さんのPDFを参照させていただいております。

- [2025年 日本の広告費 - News（ニュース） - 電通ウェブサイト](https://www.dentsu.co.jp/news/release/2026/0305-011003.html)


## PDFから表データを取り出す

公開資料がPDFで公開されています。このままではコンピュータで扱うことはできません。手作業でデータ化するのも面倒です。

![表紙ページ](<images/2025年 日本の広告費_p01.png>)
![該当ページ](<images/2025年 日本の広告費_p14.png>)

こんなときは Tabula を使うと簡単に、PDFから表データを取り出すことができます。

{{< external-link-card
    url="https://tabula-pdf.dataprep.jp/"
    title="Tabula PDF"
    image="images/cover_tabula-pdf.jpg"
    site="dataprep.jp"
    description="PDFから表データを取り出す"
>}}
{{< /external-link-card >}}

![取り出すデータ範囲を選択](images/kokoku_01.png)

![二種類のアルゴリズムから最適な方を目で確認してCSV出力します](images/kokoku_02.png)

## データをクレンジングする

コンピュータで扱える整頓データにするためには OpenRefine が便利です。ビジュアルに確認しながらデータをクレンジングできます。

![さきほどのCSVファイルを読み込んだところ](images/kokoku_03.png)

不要な列を削除しました。そして不要な空白やコンマも削除しました。

![不要な列、空白、コンマを削除](images/kokoku_05.png)

そのままではクロス集計（マトリックス形式）された状態ですので、エクセルでいうピボットテーブルの逆を行います。OpenRefineならそれもビジュアルに行えます。

![行列転置→列を行に転置（縦持ち化）](images/kokoku_06.png)

![加工したあとの列名を指定](images/kokoku_07.png)

![コンピュータで扱える整頓データされたところ](images/kokoku_08.png)

これでデータのクレンジングは終了です。
好きな可視化ツールを使いましょう。
今回はメッコ・チャートが簡単に作れる RawGraphs を用います。

## RawGraphsでデータ可視化する

RawGraphs は一画面で完結するツールで、工程を終えると、下へスクロールすることで、次の工程が現れます。

![データの読み込み](images/kokoku_09.png)

![使用するチャートの選択](images/kokoku_10.png)

![表データとチャートのビジュアル変数、スペース変数との組み合わせを指定](images/kokoku_11.png)

![レイアウトを微調整する](images/kokoku_12.png)


## 完成

PNGで出力すれば、スライドに掲載するなり、ウェブに掲載するなりできますね。

![完成したチャート](images/kokoku_fin.png)

SVGで出力すれば、パワーポイントやAdobe Illustrator、Figmaなどのデザインツールで編集できます。
軸ラベルの一部が近すぎるので調整してみました。

### パワーポイントでの編集

![パワーポイントでの編集](images/kokoku_fin_pt.png)

### Adobe Illustratorでの編集

![Adobe Illustratorでの編集](images/kokoku_fin_ai.png)