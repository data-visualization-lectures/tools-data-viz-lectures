---
title: "積み重ね棒グラフ"
title_en: "Stacked Bar Chart"
slug: "stacked-bar-chart-numeric"
chart_categories:
  - numeric
chart_subcategories:
  - comparison
weight: 160
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

1つのディメンション(切り口)に対して複数のメジャーを同時に高さとして示します。メジャーは色かテクスチャで塗り分けます。メジャーの数値を実数であつかいます。

長さによって割合を示すので、円グラフによる角度よりも正確に認識しやすく、数値をより正確に伝達するには、円グラフよりもこちらを利用するとよいでしよう。

メジャーの数値を割合として示すチャートは100%積み上げ棒グラフというよび名で区別します。チャート表示領域いっぱいを100%とし、各メジャーを割合で示します。



