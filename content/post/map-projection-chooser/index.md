---
title: 投影法の選び方
description: 角度・面積・距離のどれを守るかを決めて、地図投影法を選ぶ
slug: "map-projection-chooser"
weight: 4
categories: "data-visualization-map"
address: https://map-projection-chooser.dataviz.jp/
image: "images/cover_map-projection-chooser.png"
---

{{< external-link-card
    url="https://map-projection-chooser.dataviz.jp/"
    title="投影法の選び方"
    image="images/cover_map-projection-chooser.png"
    site="dataviz.jp"
    description="角度・面積・距離のどれを守るかを決めて、地図投影法を選ぶ"
>}}
{{< /external-link-card >}}

## どんなツールか？

地図投影法は、角度・面積・距離を同時に正しくすることはできません。このツールは、いちばん大事にしたい性質から図法を選び、歪みを観察しながら比較するためのガイドです。

## 機能

- 性質からの選択...正角、正積、等距、折衷の4分類から出発する。
- 歪みの観察...Tissot 指示楕円と経緯線で、どこが保たれ、どこが歪むかを見る。
- 図法の比較...2つの投影法を並べて観察できる。
- 書き出し...選んだ図法をデザイン素材用の SVG としてダウンロードできる。D3 の呼び出し方もコピーできる。

## 使い方

- 1. いちばん大事にしたい性質を選ぶ。
- 2. 候補の図法カードから1つを開く。
- 3. 地図をドラッグして中心を動かし、Tissot 楕円で歪みを確認する。
- 4. 必要なら別の図法と並べて比較し、SVG または D3 コードとして書き出す。
