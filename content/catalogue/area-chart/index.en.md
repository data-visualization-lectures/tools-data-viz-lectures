---
title: "Area chart"
title_en: "Area chart"
slug: "area-chart"
chart_categories:
  - time
chart_subcategories:
  - linear-cartesian
weight: 430
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
{{< external-link-card
    url="https://data-illustrator.dataviz.jp/"
    title="Data Illustrator"
    image="/images/cover_data-illustrator.jpg"
    site="dataviz.jp"
    description="Create diverse charts with ease"
>}}
{{< /external-link-card >}}

An area chart has nearly the same structure as a line chart, with the difference being that the area enclosed between the line and the axis is filled with color. When displaying multiple items in a single chart, be aware that overlapping areas may obscure the data. In such cases, consider using semi-transparent fills, re-aggregating the data so that layers stack without overlapping along the Z-axis, or using a stream graph instead.
