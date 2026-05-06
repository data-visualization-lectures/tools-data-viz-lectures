---
title: "ヒストグラム"
title_en: "Histogram"
slug: "histogram"
chart_categories:
  - numeric
chart_subcategories:
  - distribution-summary
weight: 10
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

あるデータ変数を小さい順に並べ直し、その分布を示します。 ビンとよばれるデータ幅を指定し、そのビンごとにデータの個数を示します。ビンの幅とその結果としての数が、ヒストグラムの外観を決めます。

ビンの数が少なければ外観が大雑把になり細かい差異に気づけず、逆に数が多すぎると、外観が細か
すぎて傾向を大づかみすることが難しくなります。ビンの幅をさまざまに調整すること自体が、データの特徴を把握することにつながります。