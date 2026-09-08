---
title: Race Chart Builder
description: 順位の入れ替わりをアニメーションで見せるレースチャートを、5つの型から選んで作成
slug: "race-chart-builder"
weight: 2
categories: "data-visualization"
address: https://race-chart-builder.dataviz.jp/
image: "images/cover_race-chart-builder.png"
---

{{< external-link-card
    url="https://race-chart-builder.dataviz.jp/"
    title="Race Chart Builder"
    image="images/cover_race-chart-builder.png"
    site="dataviz.jp"
    description="順位の入れ替わりをアニメーションで見せるレースチャートを、5つの型から選んで作成"
>}}
{{< /external-link-card >}}

## どんなツールか？

時系列データの順位や値の変化を、アニメーションで見せるレースチャート作成ツールです。バー・チャート・レース、バンプチャート、ラインチャート、散布図レース、スロープグラフの5つから型を選び、CSVを読み込んで再生できます。レポート向けの注釈、書き出し、プロジェクト保存、公開シェアに対応しています。

## 機能

- チャート選択: バー、バンプ、折れ線、散布図、スロープの5種。トップのカタログから選ぶ
- サンプル読込: チャート種別に合った featured 作品を優先して自動読込。サンプルピッカーからも切り替え可能
- 再生コントロール: 再生・一時停止、速度、ループ。年（時点）が進むたびに順位や値が動く
- 注釈: タイトル、出典、出典URLをチャートに載せられる
- 見た目: 配色、数値の桁、ラベルの出方を設定
- エクスポート: SVG / PNG / CSV
- シェア: 保存済みプロジェクトから公開ページ（`share.html?id=`）を発行
- プロジェクト保存: データと設定をクラウドに保存・復元

## 使い方

1. チャート種別を選ぶ（またはサンプルが自動で開く）
2. CSVをアップロードするか、サンプルから読み込む
3. 再生して順位や交差、追い抜きが見えるか確認する
4. 注釈タブでタイトルと出典を入れる
5. 画像やCSVで書き出すか、プロジェクトとして保存し、必要なら公開シェアする

## データ形式

- ファイル形式: CSV（カンマ区切り、UTF-8）
- バー / バンプ / 折れ線 / スロープ: wide 形式。`name`（系列名）、任意の `category`（色分け）、以降の列が時点（年など）
- 散布図レース: long 形式。`date`、`name`、`category`、位置と大きさの数値列（例: `gdp_per_capita`、`life_expectancy`、`population`）
- 1行目がヘッダー。時点列は左から古い順
