---
title: kepler.gl
description: 大規模地理空間データの可視化・探索ツール
slug: "kepler-gl"
weight: 1
categories: "data-visualization-map"
address: https://kepler-gl.dataviz.jp/
image: "images/cover_kepler-gl.jpg"
---

{{< external-link-card
    url="https://kepler-gl.dataviz.jp/"
    title="大規模地理空間データの可視化・探索ツール"
    image="images/cover_kepler-gl.jpg"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

## どんなツールか？

ブラウザ上で動作する大規模地理空間データの可視化・探索ツールです。WebGL を活用して高性能な地図ビジュアライゼーションを生成し、位置情報データを直感的に分析できます。もともと Uber 社が開発したオープンソース GIS ツールで、プログラミング不要でデータを探索できます。 ￼


## 機能

- 多様なレイヤー表現：ポイント、ライン、ポリゴン、ヒートマップ、六角形集約（hexbin）、アークなど複数のレイヤーをサポート。 ￼
- インタラクティブ操作：フィルタリング、ズーム、パン、時間軸アニメーションなどによってデータ探索が可能。 ￼
- 高性能レンダリング：WebGL を用い、数百万件のデータポイントをスムーズに描画できる高速表示。 ￼
- スタイル設定とカスタマイズ：色分け、スケール設定、3D 表現（高さ/エクストルード）など多彩な見せ方を調整。 ￼
- エクスポート：完成した地図をPNG画像や インタラクティブなHTMLに保存・共有や、CSVファイルでの出力。
- 作成プロジェクトの保存と読込

## 使い方

- 1. データを追加：ドラッグ＆ドロップで CSV や GeoJSON ファイルを読み込む。 ￼
- 2. レイヤーを設定：レイヤー追加パネルからタイプ（ポイント/ポリゴン等）を選び、緯度経度などの列を割り当てる。 ￼
- 3. カスタマイズ：色やサイズ、フィルター・スケールを調整して視覚化を最適化。 ￼
- 4. 保存・共有：設定やマップを保存（ローカル/エクスポート）して再利用可能。 ￼



## データ形式

- CSV
- Json
- GeoJSON
- Arrow
- Parquet
