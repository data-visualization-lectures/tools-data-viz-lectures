---
title: "棒グラフ"
title_en: "Bar Chart"
slug: "bar-chart"
chart_categories:
  - numeric
chart_subcategories:
  - comparison
weight: 150
---

このチャートを作ることができるのは...

{{< external-link-card
    url="https://rawgraphs.dataviz.jp/"
    title="RAWGraphs2"
    image="/images/cover_rawgraphs-db.jpg"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}
{{< external-link-card
    url="https://vega-editor.dataviz.jp/"
    title="Vega Editor"
    image="/images/cover_vega-editor.jpg"
    site="dataviz.jp"
    description="JSON 形式で可視化仕様を書くことで、インタラクティブなグラフやチャートをリアルタイムにレンダリング"
>}}
{{< /external-link-card >}}
{{< external-link-card
    url="https://data-illustrator.dataviz.jp/"
    title="Data Illustrator"
    image="/images/cover_data-illustrator.jpg"
    site="dataviz.jp"
    description="多様なチャートを手軽に作成"
>}}
{{< /external-link-card >}}

1つのディメンション(切り口)に対して、1つのメジャーの大きさを長さで示します。たとえば都道府県ごと(デイメンション)の人口(メジャー)を知りたい場合などが該当します。多くの人が読み方を知っており、数値を長さで伝える伝達の正確さから、多くの場面で利用できるでしょう。

長さで示しつつ、面積で伝えていることでもあるので、四角のかわりに三角を用いることは避けましょう。長さと面積は比例せず、データ値をどちらで読み取ればよいのか不明であり、誤認を招くおそれがあるからです。

棒が垂直(上下方向)に伸びる縦棒グラフと、棒が水平(左右方向)に伸びる横棒グラフに、本質的な違いはありません。慣習的には説明変数を横軸、目的変数を縦軸に置くことが多いため縦棒グラフが使われがちですが、この慣習はそこまで気にする必要はありません。

縦棒グラフが望ましい場合は以下です。

- 折れ線グラフと同一スペースに棒グラフを表示させたい場合
- チャートを表示するスペースがどちらかというと横に長く、かつディメンション数が多い場合

横棒グラフが望ましい場合は以下です。

- ディメンションのラベルの文字数が長いものが多い場合
- アノテーションを記載したい場合
- チャートを表示するスペースがどちらかというと縦に長く、かつディメンション数が多い場合