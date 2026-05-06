---
title: Cytoscape
description: Cytoscapeのウェブ版
slug: "cytoscape"
weight: 3
categories: "data-visualization"
address: https://cytoscape.dataviz.jp/
image: "images/cover_cytoscape.jpg"
---

{{< external-link-card
    url="https://cytoscape.dataviz.jp/"
    title="Cytoscape"
    image="images/cover_cytoscape.jpg"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}


## どんなツールか？

デスクトップアプリとして人気のあるCytoscapeのブラウザ実装版です。

ネットワーク（グラフ）データをブラウザ上でインタラクティブに可視化するツールです。ノード（点）とエッジ（線）で構成される関係性データを読み込み、レイアウトの変更、属性によるスタイリングなどを直感的に操作できます。

Cytoscapeはネットワーク（グラフ）データを可視化・解析するオープンソースのプラットフォームです。もともとは生物学（分子間相互作用ネットワーク）の可視化・解析用に開発されましたが、ソーシャルネットワーク分析や複雑ネットワークの可視化全般にも利用されます。



## 機能

- **データの読み込み** — GEXF、GraphML、CSV形式のファイルをアップロードして可視化
- **サンプルデータセット** — Les Misérables、Game of Thrones、Marvel Universeなど9種類のサンプルデータをワンクリックで読み込み
- **レイアウト切替** — Grid、Circle、Concentric、Breadthfirst、Cose（物理シミュレーション）、Randomの6種類
- **ノードのスタイリング** — 属性に応じた色（定性的カラースキーム）、サイズ、ラベルの動的変更
- **エッジのスタイリング** — 属性に応じた色（定量的カラースキーム）、太さ、ラベルの動的変更
- **SVGエクスポート** — 現在のグラフをSVG形式でダウンロード
- **プロジェクトの保存・読込** — サーバーにプロジェクトを保存し、後から復元可能


## 使い方

1. 「データファイルの読込」ボタンからファイルを選択、または「サンプルデータの読込」から選択
2. コントロールパネルでレイアウトやイージングを変更してグラフの配置を調整
3. 「ノード」行のドロップダウンでノードの色・サイズ・ラベルに使う属性を選択
4. 「エッジ」行のドロップダウンでエッジの色・太さ・ラベルに使う属性を選択
5. 必要に応じて「エクスポート」でSVG画像として保存

## データ形式

### GEXF / GraphML
グラフ専用のXML形式です。ノードとエッジの属性（カテゴリ、重み、座標など）を豊富に記述できます。GephiやNetworkXなど多くのツールからエクスポート可能です。

### CSV（エッジリスト形式）
スプレッドシートやExcelから手軽に作成できる形式です。

- **ヘッダー行が必須**です
- `source` と `target` 列（または `from` と `to`）でエッジの両端を指定します（大文字小文字は区別しません）
- それ以外の列はエッジの属性として読み込まれます
- ノードはエッジの情報から自動的に生成されます

```csv
source,target,weight,type
Alice,Bob,1.0,friends
Bob,Carol,2.5,colleagues
Alice,Dave,0.8,family


