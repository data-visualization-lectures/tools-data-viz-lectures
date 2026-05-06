---
title: Color Brewer
description: カラースキーム選びを地図上でシミュレーション
slug: "colorbrewer"
weight: 2
categories: "data-visualization-color"
address: https://colorbrewer.dataviz.jp/
image: "images/cover_colorbrewer.jpg"
---

{{< external-link-card
    url="https://colorbrewer.dataviz.jp/"
    title="Color Brewer"
    image="images/cover_colorbrewer.jpg"
    site="dataviz.jp"
    description="カラースキーム選びを地図上でシミュレーション"
>}}
{{< /external-link-card >}}


## どんなツールか？

ColorBrewer は、データ可視化や地図で使用するための 最適な配色（カラーパレット）を選ぶためのオンラインツールです。色の視認性やカテゴリー・数値データの性質に応じた配色を提案することを目的としています。

## 機能

- カラースキームの選択支援...データの性質に応じて 定量データ（sequential）、分岐データ（diverging）、定性的データ（qualitative） などのカラースキームを提示。 ￼
- 表示用途の考慮...カラーブラインド（色覚バリアフリー）、印刷、コピー耐性など用途に応じたオプションでフィルタリング可能。 ￼
- 階級分類数の指定...色数（3〜12 など）を調整しながら最適な配色を選べる。 
- カラー情報出力形式...選択したパレットを HEX/RGB/CMYK の形式や CSS/JavaScript 配列などで出力できる。
- 作成プロジェクトの保存と読込。

## 使い方

- 1. データの性質を選択...定量（順序あり）、分岐（中心値を境に両極を示す）、カテゴリー（順序なし）などから選ぶ。 ￼
- 2. 色数（クラス数）を指定...表示したいデータクラス数（例：3, 4, …）を選択。 ￼
- 3. 配色を確認・調整...選択したパレットが地図やグラフ上でどのように見えるか確認する。 ￼
- 4. 出力...必要に応じて CSS、JavaScript、Adobe Swatch などでエクスポート。 ￼






![](images/screen_01.png)

![](images/screen_02.png)



