---
title: "Scatterplot Matrix"
title_en: "Scatterplot Matrix"
slug: "scatterplot-matrix"
chart_categories:
  - numeric
chart_subcategories:
  - correlation
weight: 280
---


Tools that can create this chart...

{{< external-link-card
    url="https://vega-editor.dataviz.jp/"
    title="Vega Editor"
    image="/images/cover_vega-editor.jpg"
    site="dataviz.jp"
    description="Write visualization specs in JSON to render interactive graphs and charts in real time"
>}}
{{< /external-link-card >}}

To exhaustively explore correlations among variables within a dataset, variables are arranged in a matrix and a scatterplot is drawn at each intersection using the corresponding pair of variables, enabling more efficient exploration.

When the two intersecting variables are the same, there is no need to examine correlation, so a histogram is displayed instead. Since the order of two intersecting variables does not matter, the same pair of variables appears in two locations. Rather than displaying the same scatterplot twice, one of the locations may show the correlation coefficient instead.

