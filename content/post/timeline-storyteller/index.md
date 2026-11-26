---
title: Timeline Storyteller
description: 年表のデータから、見せ方を変えながら場面ごとに語るストーリーをつくる可視化ツール
slug: "timeline-storyteller"
weight: 1
categories: "data-visualization"
address: https://timeline-storyteller.dataviz.jp/
image: "images/cover_timeline-storyteller.png"
---

{{< external-link-card
    url="https://timeline-storyteller.dataviz.jp/"
    title="Timeline Storyteller"
    image="images/cover_timeline-storyteller.png"
    site="dataviz.jp"
    description="年表を表現・スケール・レイアウトの組み合わせで描き、ストーリーに仕立てる"
>}}
{{< /external-link-card >}}

## どんなツールか？

Timeline Storyteller は、年表のデータを読み込み、見せ方を選び、注釈を付けて、場面ごとに語るストーリーに仕立てるツールです。年表の形を「表現」「スケール」「レイアウト」の3つの組み合わせで決めるので、同じデータを直線の年表にも、円形の年表にも、人物ごとに並べた年表にもできます。見せ方や注釈を変えながら場面を記録していくと、順に再生できるストーリーになります。

Microsoft Research が MIT License で公開した Timeline Storyteller（© Microsoft Corporation）をもとにしています。

## 機能

- 表現: 線形、放射状、らせん、曲線、カレンダー、グリッドの6種類
- スケール: 年代順、相対、対数、順序、圧縮の5種類
- レイアウト: 1本にまとめる「統合」、分類ごとに並べる「ファセット」、世紀や日などで分ける「区切り」の3種類
- 注釈: イベントのラベル、自由な文章のキャプション、画像をキャンバスに配置
- 絞り込み: カテゴリ、ファセット、区切りを条件に、該当するイベントを強調、または該当しないイベントを非表示
- ストーリー: いまのキャンバスをシーンとして記録し、順に再生
- 書き出し: PNG、SVG、シーンを順に見せる GIF アニメーション、続きを編集できるストーリーのファイル
- プロジェクト保存: データと記録したシーンをクラウドに保存・復元
- 日本語と英語の表示に対応。軸の日付も日本語で表示

## 使い方

- ヘッダーの「サンプルデータ」から年表を選ぶ。手元のファイルは左のパネルの「開く」から読み込む
- 画面上部のパネルで、表現、スケール、レイアウトを選ぶ。組み合わせられない選択肢は薄く表示される
- イベントをクリックしてラベルを付け、キャプションや画像を加える
- 画面下部の赤い丸のボタンで、いまの画面をシーンとして記録する。見せ方を変えて記録を重ねる
- 四角い枠のボタンで再生モードに入り、矢印でシーンを順に送る
- 左のパネルの「書き出し」から画像や GIF を保存する。作業状態はヘッダーの「プロジェクトの保存」でクラウドに残せる

## データ形式

- ファイル形式: CSV / JSON
- 1行（1件）が1つのイベント
- `start_date`（必須）: 開始日。`YYYY`、`YYYY-MM`、`YYYY-MM-DD`、`YYYY-MM-DD HH:MM` の形式。紀元前は `-27` のように負の数で書く
- `end_date`（任意）: 終了日。省略すると、ある一時点の出来事になる
- `content_text`（任意）: イベントの説明文。ラベルとして表示される
- `category`（任意）: イベントの分類。色分けに使われる
- `facet`（任意）: もう1つの分類。年表を分けて並べるときに使われる

CSV の例です。

```
start_date,end_date,content_text,facet,category
1868-10-23,1912-07-30,明治,元号,元号
1923-09-01,,関東大震災,出来事,災害
```
