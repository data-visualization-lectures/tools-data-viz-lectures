---
title: Vega Editor
description: JSON 形式で可視化仕様を書くことで、インタラクティブなグラフやチャートをリアルタイムにレンダリング
slug: "vega-editor"
weight: 10
categories: "data-visualization"
address: https://vega-editor.dataviz.jp/
image: "images/cover_vega-editor.jpg"
---

{{< external-link-card
    url="https://vega-editor.dataviz.jp/"
    title="Vega Editor"
    image="images/cover_vega-editor.jpg"
    site="dataviz.jp"
    description="JSON 形式で可視化仕様を書くことで、インタラクティブなグラフやチャートをリアルタイムにレンダリング"
>}}
{{< /external-link-card >}}


## どんなツールか？

Vega Editor は、Vega および Vega-Lite ビジュアライゼーション仕様 を記述・編集・プレビューできる Web ベースの IDE（エディタ）です。JSON 形式で可視化仕様を書くことで、インタラクティブなグラフやチャートをリアルタイムにレンダリングできます。Vega と Vega-Lite は宣言的な可視化文法であり、データと表示ルールを JSON で定義してグラフを生成します。 ￼


## 機能

- テキストエディタ／コードビュー...Vega/Vega-Lite の JSON を入力・編集するエディタを提供。 ￼
- リアルタイムプレビュー...編集した仕様を即座に可視化としてブラウザ上で表示。 ￼
- サンプル・テンプレ...例示スペックを読み込み、学習・試行錯誤が可能（公式版の特徴としてあり）。 ￼
- Vega / Vega-Lite モード切替...両方の仕様を選んで編集・プレビューできる（公式ツールの標準機能）。 ￼
- 共有／エクスポート...仕様を GitHub Gist などに保存・共有できるバックエンド連携が存在（Vega 公式版機能）。 ￼



## 使い方

- 1. JSON 形式で仕様を書く...Vega または Vega-Lite の仕様をエディタに入力。 ￼
- 2. プレビューを見る...書いた仕様がリアルタイムでレンダリングされ、結果を確認可能。 ￼
- 3. 必要に応じて保存・共有...仕様を Gist 等に保存して他者と共有（バックエンド連携時）。 ￼

## データ形式

- JSON（Vega / Vega-Lite 仕様）...可視化の定義（データ参照、変換、エンコーディング、マーク等）を JSON で記述します。 ￼
- データソースとしての表形式...Vega/Vega-Lite では JSON 内に直接埋め込むか、CSV/TSV ファイルへの URL 参照などで外部データを読み込み可能です（仕様一般）。 ￼
