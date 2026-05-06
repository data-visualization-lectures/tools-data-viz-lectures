---
title: ADS-B / AIS 可視化
description: 飛行機や船の移動データを手軽に動画化
slug: "bbts"
weight: 10
categories: "data-visualization-map"
address: https://bbts.dataviz.jp/
image: "images/cover_broadcast-tracking-system.jpg"
---

{{< external-link-card
    url="https://bbts.dataviz.jp/"
    title="ADS-B / AIS 可視化"
    image="images/cover_broadcast-tracking-system.jpg"
    site="dataviz.jp"
    description="飛行機や船の移動データを手軽に動画化"
>}}
{{< /external-link-card >}}


## どんなツールか？

緯度・経度を含むCSVファイルをアップロードするだけで、航跡を地図上にアニメーション表示できるWebツールです。ADS-B（航空機追跡）やAIS（船舶追跡）などの放送型測位データの可視化に対応しています。


## 機能

- CSVアップロード：ドラッグ&ドロップまたはファイル選択でCSVを読み込み
- 航跡の可視化：時系列データをもとに、地図上に移動経路をアニメーション描画
- 複数トラック対応：1つのCSVに複数の機体・船舶が含まれていても自動でグループ化して表示
- カラム名の自動判別：lat/lon、latitude/longitude など、大文字・小文字を問わず自動認識
- サンプルデータ：すぐに試せるサンプルデータを用意

## 使い方

- CSVファイルを用意（緯度・経度・タイムスタンプを含むもの）
- 画面左のサイドバーからファイルをドラッグ&ドロップ、またはクリックして選択
- サンプルデータも用意
- 自動的に航跡が地図上に描画
- GIFアニメ、静止画連番画像、動画ファイルなどで出力可能
- 背景のベース地図のスタイルが選択可能なほか、日時を表示するかどうかなどのカスタマイズが可能


## データ形式

CSVで以下の変数を含めてください。

- 位置（必須）：lat / lon、latitude / longitude、または Position（"lat,lon" 結合形式）
- 時刻（必須）：Timestamp（Unixエポック秒）など
- 識別子：Callsign（航空機）、MMSI / VesselName（船舶）
- オプション：Altitude、Speed、Direction / Course

### 対応する位置データの形式

カラム名の大文字・小文字は区別しません（例：LAT、Lat、lat いずれもOK）。

| カラム名 | 説明 |
|------|-----|
| `lat` / `lon` | 緯度・経度（省略形） |
| `latitude` / `longitude` | 緯度・経度（正式名） |
| `Position` | 緯度・経度の結合形式（`"35.68,139.76"`） |



### 対応する時刻データの形式

時刻データは以下の形式を自動判別します。カラム名は timestamp、time、datetime、date などに対応しています。

| 形式 | 例 |
|------|-----|
| ISO 8601 | `2023-05-20T10:30:00Z` |
| 日時文字列 | `2023-05-20 10:30:00` |
| コンパクト形式 | `20230520_103000` |
| Unixタイムスタンプ（秒） | `1684567890` |
| Unixタイムスタンプ（ミリ秒） | `1684567890123` |


1つのCSVに複数の機体・船舶が含まれている場合も、自動でグループ化して表示します。

## 参考情報

- [ADS-Bとは](https://visualizing.jp/ads-b/)
- [AISとは](https://visualizing.jp/ais/)