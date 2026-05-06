---
title: Gephi Lite
description: ネットワークグラフを手軽に作成
slug: "gephi-lite"
weight: 10
categories: "data-visualization"
address: https://gephi-lite.dataviz.jp/
image: "images/cover_gephi-lite.jpg"
---

{{< external-link-card
    url="https://gephi-lite.dataviz.jp/"
    title="Gephi Lite"
    image="images/cover_gephi-lite.jpg"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}


## どんなツールか？

Gephi Lite は、ネットワークグラフ（関係性の可視化）をブラウザ上で手軽に行えるWebアプリケーションです。ノード（点）とエッジ（線）で構成されるデータを読み込み、レイアウト計算・色分け・フィルタリングなどを直感的に操作できます。


## 機能

- **グラフの可視化**: ノードとエッジの関係をインタラクティブに表示。ズーム・パン・ノード選択が可能
- **レイアウト計算**: ForceAtlas2、Force Directed、Circular、CirclePack など複数のレイアウトアルゴリズムを搭載
- **外観設定**: ノードやエッジの色・サイズ・ラベルを、属性値に基づいて自動的に割り当て
- **フィルタリング**: 属性値や範囲指定でノード・エッジを絞り込み表示
- **メトリクス計算**: 次数、PageRank、媒介中心性、Louvain コミュニティ検出などのネットワーク分析指標を算出
- **データテーブル**: ノード・エッジの属性を一覧表示・編集
- **エクスポート**: グラフ画像（PNG）やグラフデータ（GEXF）として書き出し
- **日本語／英語 自動切替**: ブラウザの言語設定に応じてUIを自動で出し分け


## 使い方

1. ページにアクセスすると、サンプルグラフまたは空のワークスペースが表示されます
2. 画面上部の「データファイルを開く」ボタン、またはファイルのドラッグ＆ドロップでデータを読み込みます
3. 左サイドメニューから「レイアウト」を選び、アルゴリズムを実行してノードを自動配置します
4. 「外観」メニューで、属性に応じた色やサイズを設定し、グラフを見やすく調整します
5. 「フィルター」や「メトリクス」で分析を深めます
6. 完成したグラフは画像（PNG）やデータファイル（GEXF）としてエクスポートできます

## データ形式

以下のファイル形式に対応しています。

| 形式 | 拡張子 | 説明 |
|------|--------|------|
| **CSV** | `.csv` | エッジリスト形式。1行目にヘッダー（Source, Target 等）、2行目以降に各エッジのデータを記述。最もシンプルな形式 |
| **GEXF** | `.gexf` | Gephi 標準のXML形式。ノード・エッジの属性や視覚情報を豊富に保持 |
| **GraphML** | `.graphml` | XMLベースの標準的なグラフ記述形式 |
| **Graphology JSON** | `.json` | Graphology ライブラリのJSON形式 |

**CSVファイルの書式例：**

```csv
Source,Target,Weight
Alice,Bob,1.0
Bob,Charlie,2.0
Alice,Charlie,1.5
```

- 1行目はヘッダー（必須）
- `Source`（または `From`, `Src`）列と `Target`（または `To`, `Dst`）列を自動検出します
- その他の列（Weight など）はエッジの属性として取り込まれます
- ノードは Source / Target の値から自動生成されます
- 文字コードは **UTF-8** および **Shift_JIS** に対応しています



