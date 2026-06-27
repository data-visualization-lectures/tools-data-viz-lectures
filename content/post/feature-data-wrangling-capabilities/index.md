---
title: データ加工ツールで出来ること
description: クレンジング・変換・結合・地理情報処理まで、データ可視化前に必要なデータ加工を幅広くサポートします。
slug: "feature-data-wrangling-capabilities"
weight: 4
categories: "features"
image: "/images/features/feature-data-wrangling-capabilities.png"
---

可視化結果の品質は、**元データの品質**で決まります。「データの道具箱」では、データ可視化前の前処理を効率化するデータ加工ツール群を幅広く取り揃えています。

- [データをクレンジングしたい](#データをクレンジングしたい)
- [データ同士を結合したい](#データ同士を結合したい)
- [JSONの構造を把握したい](#jsonの構造を把握したい)
- [文字化けを解消したい](#文字化けを解消したい)
- [住所から緯度経度を算出したい](#住所から緯度経度を算出したい)
- [PDFから表データを取り出したい](#pdfから表データを取り出したい)
- [地図データを加工したい](#地図データを加工したい)
- [座標やフォーマットを変換したい](#座標やフォーマットを変換したい)


## データをクレンジングしたい

表記ゆれや重複のクレンジングを、**ビジュアルに確認しながら**進められます。

{{< external-link-card
    url="https://open-refine.dataviz.jp/"
    title="OpenRefine"
    image="/images/cover_open-refine.jpg"
    site="dataviz.jp"
    description="表データのクレンジング・変換ツール"
>}}
{{< /external-link-card >}}


## データ同士を結合したい

地図データとテーマデータの**マージ作業**をブラウザ上で完結。JOIN のキー設定もGUIで行えます。

{{< external-link-card
    url="https://geo-data-merger.dataprep.jp/"
    title="(Geo) DataMerger"
    image="/images/cover_geo-data-merger.jpg"
    site="dataprep.jp"
    description="地理データとテーマデータを手軽に結合"
>}}
{{< /external-link-card >}}


## JSONの構造を把握したい

複雑にネストされたJSONの構造を、**ツリー状に展開**して視覚的に把握できます。

{{< external-link-card
    url="https://jsoncrack.dataprep.jp/"
    title="JSON Crack"
    image="/images/cover_jsoncrack.png"
    site="dataprep.jp"
    description="ブラウザ上で JSON データ構造を視覚的に理解する"
>}}
{{< /external-link-card >}}


## 文字化けを解消したい

Shift JIS と UTF-8 の相互変換を、**ブラウザ上で安全に**行えます。行政機関の公開データを扱う際に重宝します。

{{< external-link-card
    url="https://change-character-encoding.dataprep.jp/"
    title="Shift JIS ⇄ UTF-8 文字コード変換ツール"
    image="/images/cover-change-character-encoding.png"
    site="dataprep.jp"
    description="文字コードを、Shift JIS ⇄ UTF-8 間で相互に変換"
>}}
{{< /external-link-card >}}


## 住所から緯度経度を算出したい

住所データを**ジオコーディング**し、地図化に必要な緯度経度を取得できます。

{{< external-link-card
    url="https://address-to-latlon.dataprep.jp/"
    title="住所 → 緯度経度 変換ツール"
    image="/images/cover_address-to-latlon.jpg"
    site="dataprep.jp"
    description="ジオコーディング・ツール"
>}}
{{< /external-link-card >}}


## PDFから表データを取り出したい

PDF内の**表データを範囲指定**して抜き出し、CSVやExcel形式で保存できます。

{{< external-link-card
    url="https://tabula-pdf.dataprep.jp/"
    title="Tabula PDF"
    image="/images/cover_tabula-pdf.jpg"
    site="dataprep.jp"
    description="PDFから表データを取り出す"
>}}
{{< /external-link-card >}}


## 地図データを加工したい

GeoJSON の**軽量化・整形・相互変換**を、目的にあわせて複数のツールから選べます。

{{< external-link-card
    url="https://mapshaper.dataprep.jp/"
    title="Mapshaper"
    image="/images/cover_mapshaper.jpg"
    site="dataprep.jp"
    description="地図データの加工や変換"
>}}
{{< /external-link-card >}}
{{< external-link-card
    url="https://geojson.dataprep.jp/"
    title="GeoJSON.io"
    image="/images/cover_geojson.jpg"
    site="dataprep.jp"
    description="地図タイルをトレースしてGeoJSON作成"
>}}
{{< /external-link-card >}}
{{< external-link-card
    url="https://turf-buffer.dataprep.jp/"
    title="バッファ生成ツール"
    image="/images/cover_turf-buffer.png"
    site="dataprep.jp"
    description="指定した半径指定をブラウザで手軽に"
>}}
{{< /external-link-card >}}


## 座標やフォーマットを変換したい

**座標系の変換、緯度経度の桁数調整、SVG↔GeoJSON 変換**など、フォーマット調整を細かくサポートします。

{{< external-link-card
    url="https://latlon-formatter.dataprep.jp/"
    title="緯度経度フォーマッター"
    image="/images/cover_latlon-formatter.png"
    site="dataprep.jp"
    description="緯度経度データの桁数を簡単に変換"
>}}
{{< /external-link-card >}}
{{< external-link-card
    url="https://transform-coordinates.dataprep.jp/"
    title="座標系 変換ツール"
    image="/images/cover_transform-coordinates.png"
    site="dataprep.jp"
    description="地物ファイルの座標を変換"
>}}
{{< /external-link-card >}}
{{< external-link-card
    url="https://geojson-and-svg.dataprep.jp/"
    title="SVG ⇄ GeoJSON 変換ツール"
    image="/images/cover_geojson-and-svg.jpg"
    site="dataprep.jp"
    description="GeoJSON と SVG の相互変換を支援"
>}}
{{< /external-link-card >}}


## 関連ページ

- <a href="/how-to-use-data-wrangling/">データ加工ツールの使い分け</a>
- <a href="/tools/">ツール一覧</a>
