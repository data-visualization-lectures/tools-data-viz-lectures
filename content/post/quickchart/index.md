---
title: QuickChart UI
description: URLだけでチャート画像生成
slug: "quickchart"
weight: 20
categories: "data-visualization"
address: https://quickchart.dataviz.jp/
image: "images/cover-quickchart.png"
---

{{< external-link-card
    url="https://quickchart.dataviz.jp/"
    title="QuickChart UI"
    image="images/cover-quickchart.png"
    site="dataviz.jp"
    description="URLだけでチャート画像生成"
>}}
{{< /external-link-card >}}

## どんなツールか？

QuickChart は、URLのみで、指定したデータとチャート定義（Chart.js 形式）から 静的なチャート画像（PNG 等）を即座に生成できるツールです。

サーバー-サイドやメール、レポート、ドキュメントなど JavaScript 実行環境が無くても画像として埋め込み可能なグラフを作れるのが特徴です。 ￼

本ツールはそのためのURL指定をGUIで手軽に行えるツールです。


## 機能

- チャート画像生成...URL のパラメータやクエリ文字列で指定した設定から、棒グラフ、折れ線、円グラフなどの 静的なチャート画像を生成。 ￼
- URL だけで完結...複雑なライブラリの導入なしに、URL のクエリだけでグラフを作成可能。 ￼
- 画像として利用可能...生成したチャートは PNG 等の画像として出力されるため、ウェブページ、レポート、メールに埋め込みやすい。 ￼



## 使い方

- 1. URL のクエリパラメータに チャート設定を JSON 形式で指定。 ￼
- 2. 生成された 画像 URL をそのまま使う／ダウンロードする。


## データ形式

- 表データ(CSV)