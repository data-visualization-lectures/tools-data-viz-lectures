---
title: Voyager2
description: データ探索（Exploratory Data Analysis, EDA）を支援するビジュアライゼーションツール
slug: "voyager2"
weight: 10
categories: "data-visualization"
address: https://voyager2.dataviz.jp/
image: "images/cover_voyager2.jpg"
---

{{< external-link-card
    url="https://voyager2.dataviz.jp/"
    title="Voyager2"
    image="images/cover_voyager2.jpg"
    site="dataviz.jp"
    description="データ探索（Exploratory Data Analysis, EDA）を支援するビジュアライゼーションツール"
>}}
{{< /external-link-card >}}

## どんなツールか？

Voyager 2 は、データ探索（Exploratory Data Analysis, EDA）を支援するビジュアライゼーションツールです。ブラウザ上でデータを読み込み、視覚化をインタラクティブに探索・生成できます。元のプロジェクトは Vega エコシステム上で開発された Voyager のフォーク／派生であり、手動チャート指定と自動推薦を組み合わせた探索支援を特徴とします。

## 機能

- データ探索インターフェース...データを読み込んでフィールド一覧、チャートエンコーディング、フィルタリングなどのパネルで操作可能。 ￼
- 視覚化の推薦機能...現在の可視化（focus view）に関連するチャート（related views）や、複数のチャート候補を wildcards で自動生成して一覧表示。 ￼
- 部分指定による複数チャート生成...Wildcard（ワイルドカード）を使い、複数の視覚化仕様を同時に生成・比較できる。 ￼
- インタラクティブ操作...ドラッグ＆ドロップ等で encoding チャネルにフィールドを割り当て、リアルタイムで可視化を更新。 ￼


## 使い方

- 1. データを読み込む...CSV 等の表形式データをロードし、フィールド一覧を確認。 ￼
- 2. 可視化を指定する...エンコーディングチャネル（例：x 軸、y 軸、色など）にフィールドをドラッグして視覚化を作成。 
- 3. 探索支援を使う...Wildcards を使って複数ビューを同時生成したり、関連ビューを推薦してデータを広く探索。 ￼
- 4. 結果を調整／比較...推薦された視覚化や生成されたチャートを比較しながら、分析を深める。 ￼


## データ形式


- 表データ(CSV、TSV)
- JSON


