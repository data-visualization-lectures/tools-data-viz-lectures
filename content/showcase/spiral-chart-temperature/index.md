---
title: スパイラル・チャートで見る日本の気温変動
description:
slug: "spiral-chart-temperature"
weight: 1
categories: "showcase"
image: "images/spiral-chart-temperature.png"
---

1898年から現在までの日本の年平均気温の偏差を、スパイラル・チャートで可視化しました。

<a href="/rawgraphs/">RawGraphs</a>のスパイラル・チャートを使えば、長期間の時系列データを渦巻き状に配置し、時間経過に伴う変化の傾向を一目で捉えることができます。

![完成図](images/spiral-chart-temperature.png)

ここでは本サービスのツールを用いた作成の仕方を紹介します。

{{< external-link-card
    url="https://rawgraphs.dataviz.jp/?project_id=633f49cd-5368-4f5b-8752-a9a30cc00110"
    title="スパイラル・チャートで見る日本の気温変動"
    image="images/spiral-chart-temperature.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}



## データの取得

気象庁が公開している「日本の年平均気温偏差」のデータを使用しています。

- <a href="https://www.data.jma.go.jp/cpdinfo/temp/list/an_jpn.html" target="_blank">日本の年平均気温偏差 — 気象庁</a>

このデータは1898年から2025年までの各年について、1991〜2020年の30年平均値を基準とした気温偏差（℃）を記録したものです。近年は+1℃を超える正の偏差が続いており、長期的な気温上昇の傾向が読み取れます。

## RawGraphsでの可視化

RawGraphs にCSVデータを読み込み、チャートの種類から「スパイラル・チャート」を選択します。

時間軸に年を、値に気温偏差を割り当てると、中心から外側に向かって年代が進むスパイラル状のチャートが描画されます。外周に近づくほど近年のデータとなり、色や位置の変化から気温上昇の傾向が視覚的に浮かび上がります。

## スパイラル・チャートの利点

棒グラフや折れ線グラフでも同じデータを表現できますが、100年以上の長期データでは横に長くなりすぎてしまいます。スパイラルチャートはコンパクトな面積に長い時系列を収められるため、全体の傾向を俯瞰しやすいのが特長です。

渦巻きの内側（過去）と外側（現在）を比較することで、気温偏差が年々大きくなっていく様子を直感的に把握できます。
