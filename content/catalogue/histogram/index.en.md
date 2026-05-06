---
title: "Histogram"
title_en: "Histogram"
slug: "histogram"
chart_categories:
  - numeric
chart_subcategories:
  - distribution-summary
weight: 10
---

Tools that can create this chart...

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
    description="Write visualization specs in JSON to render interactive graphs and charts in real time"
>}}
{{< /external-link-card >}}

A data variable is sorted in ascending order to show its distribution. A data width called a "bin" is specified, and the count of data points within each bin is displayed. The bin width and the resulting counts determine the appearance of the histogram.

If there are too few bins, the appearance becomes too coarse and fine differences go unnoticed. Conversely, if there are too many bins, the appearance becomes too detailed, making it difficult to grasp overall trends. The process of adjusting the bin width itself helps in understanding the characteristics of the data.