---
title: 棒グラフ・クロスフィルター
description: 
slug: "bar-chart-filter"
weight: 1
categories: "data-visualization"
address: https://bar-chart-filter.dataviz.jp/
image: "images/cover_bar-chart-filter.png"
---

{{< external-link-card
    url="https://bar-chart-filter.dataviz.jp/"
    title="棒グラフ・クロスフィルター"
    image="images/cover_bar-chart-filter.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

## どんなツールか？

Bar Chart Filter は、CSVやTSVデータをアップロードするだけで、インタラクティブなクロスフィルター付き棒グラフダッシュボードを作成できるツールです。複数の棒グラフが連動し、一方のグラフをクリックすると他のグラフやデータテーブルが即座に絞り込まれます。データの傾向や構成比を直感的に探索でき、結果はURLで共有したり、画像としてエクスポートできます。

![シェアしたHTMLの例](images/bar-chart-filter_01.png)

{{< external-link-card
    url="https://bar-chart-filter.dataviz.jp/share.html?id=b399cffd-a05c-4ea8-9e66-278ffac8e5cc"
    title="令和6年度 墨田区住民意識調査"
    image="images/bar-chart-filter_01.png"
    site="dataviz.jp"
    description="ショーケース"
>}}
{{< /external-link-card >}}


## 機能

- **クロスフィルター**: 棒グラフのクリックで他のグラフとテーブルが連動フィルタリング
- **カラム選択**: データの中からテキスト型の変数を自動検出し、最大6つまで棒グラフとして表示
- **データテーブル**: フィルタ結果を一覧表示。ページング対応
- **行リンク**: URLカラムを指定すると、テーブル行クリックで外部ページに遷移
- **スタイル調整**: バーの色、行の高さ、テーブル表示件数をカスタマイズ
- **注釈**: タイトルとデータソースを設定可能
- **エクスポート**: SVG / PNG / CSV / JSON 形式でダウンロード
- **共有**: URLを発行して誰でも閲覧可能。iframe による埋め込みにも対応
- **プロジェクト保存・読込**: 作業状態を保存し、後から再開可能

## 使い方

1. CSV / TSV / JSON ファイルをドラッグ＆ドロップ、またはクリックしてアップロード
2. テキスト型の変数が自動検出され、棒グラフ候補としてスタイルタブに表示されます
3. 表示したい変数のチップをクリックして選択（最大6つ）
4. 棒グラフの各バーをクリックすると、他のグラフとデータテーブルが絞り込まれます
5. 注釈タブでタイトルやデータソースを入力
6. 共有タブからSVG/PNG/CSV/JSONのエクスポート、またはShare ボタンで共有URLを発行

## データ形式

CSV / TSV / JSON（配列形式）に対応しています。

- **CSV**: カンマ区切り。1行目がヘッダー
- **TSV**: タブ区切り。1行目がヘッダー
- **JSON**: オブジェクトの配列 `[{"col1":"val1", ...}, ...]` または `{"data": [...]}` 形式

特定のカラム名は不要です。どのようなカラム構成のデータでも読み込めます。テキスト値を含むカラムが棒グラフの候補として自動的にリストされます。
