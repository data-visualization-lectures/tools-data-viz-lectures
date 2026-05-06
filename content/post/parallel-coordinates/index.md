---
title: Parallel Coordinates
description: 多次元データの比較・探索に特化したインタラクティブなチャート
slug: "parallel-coordinates"
weight: 10
categories: "data-visualization"
address: https://parallel-coordinates.dataviz.jp/
image: "images/cover_parallel-coordinates.png"
---

{{< external-link-card
    url="https://parallel-coordinates.dataviz.jp/"
    title="Parallel Coordinates"
    image="images/cover_parallel-coordinates.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

## どんなツールか？

多次元データの比較・探索に特化したインタラクティブなチャートです。CSVファイルをアップロードするだけで、数値項目が平行な軸として並び、各行がそれらを横断する折れ線として描画されます。軸ごとのブラッシングで条件に合うデータだけを絞り込み、パターンや外れ値を直感的に発見できます。


## 機能

- ブラッシング: 各軸を縦方向にドラッグして範囲を指定し、条件に合うデータだけをフィルタリング
- 軸の並べ替え: 列名を横にドラッグして軸の順序を自由に変更。関連する指標を隣り合わせに配置して比較
- スケール切り替え: Original（元の値）、Min-Max（0-1正規化）、Z-Score（標準化）の3モードで表示を切り替え
- テーブル連動: 下部のデータテーブルはブラッシング結果に連動。行にホバーするとチャート上の対応ラインがハイライト
- エクスポート: フィルタリング結果をCSV、チャート画像をSVG/PNGで書き出し
- シェア — 現在の表示状態をURLで共有。SNS向けOGP画像も自動生成
- プロジェクト保存: データと設定（スケール、軸順序、ブラシ範囲）をクラウドにサムネイル付きで保存・復元


## 使い方

- 「CSV Upload」でデータを読み込む（または「Sample」でヨーグルト栄養データを試す）
- 軸を縦にドラッグして気になる範囲を絞り込む
- 必要に応じてScaleをMin-MaxやZ-Scoreに切り替え、異なる単位の指標を比較
- 軸名を横にドラッグして、比較したい項目を隣に並べる
- テーブルの行にマウスを合わせると、チャート上で該当ラインがハイライトされる
- 結果をCSV/SVG/PNGでエクスポート、またはプロジェクトとしてクラウドに保存


## データ形式

- ファイル形式: CSV（カンマ区切り、UTF-8）
- 構造: 1行目がヘッダー（列名）、2行目以降がデータ
- 数値列: 自動判定され、チャートの軸として表示される
- 文字列列: テーブルには表示されるが、チャートの軸には含まれない
- 欠損値: 空セルは欠損として扱われる

