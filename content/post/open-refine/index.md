---
title: OpenRefine
description: 表データのクレンジング・変換ツール
slug: "open-refine"
weight: 1
categories: "data-wrangling"
address: https://open-refine.dataviz.jp/
image: "images/cover_open-refine.jpg"
---

{{< external-link-card
    url="https://open-refine.dataviz.jp/"
    title="OpenRefine"
    image="images/cover_open-refine.jpg"
    site="dataviz.jp"
    description="表データのクレンジング・ツール"
>}}
{{< /external-link-card >}}

## どんなツールか？

OpenRefine は、表データのクリーニング（重複削除・表記ゆれ修正・整形）と変換をブラウザ上で行えるツールです。
大量データを一括で処理でき、手作業での修正を大きく減らせます。

クレンジング作業中の状態をサーバ側で保存することが出来るほか、クレンジング手順自体を記録して同様のファイルに適用することも出来ます。


## 機能

- フィルタ・ファセット による絞り込みと値の確認
- 列の分割・結合、値の置換、空白や記号の正規化
- 重複検出やクラスタリングによる表記ゆれ修正
- 式（GREL）を使った一括変換
- 外部データとの照合（Reconciliation）

## 使い方

- 1. CSV / TSV / Excel / JSON などのデータを読み込む
- 2. Facet やフィルタで問題のある値を見つける
- 3. 変換・置換・クラスタリングでデータを整える
- 4. 必要な形式でエクスポートする

## データ形式

- 入力：CSV、TSV、Excel(xls/xlsx)、Googleシート、JSON、XML、OpenDocument など
- 出力：CSV、TSV、Excel、JSON など

## 公式解説サイト

{{< external-link-card
    url="https://open-refine-doc.dataviz.jp/"
    title="OpenRefineの公式解説サイト"
    image="images/cover_openrefine-doc.png"
    site="dataviz.jp"
    description="OpenRefine解説"
>}}
{{< /external-link-card >}}