---
title: "Bar Chart"
title_en: "Bar Chart"
slug: "bar-chart"
chart_categories:
  - numeric
chart_subcategories:
  - comparison
weight: 150
---

You can create this chart with...

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
{{< external-link-card
    url="https://data-illustrator.dataviz.jp/"
    title="Data Illustrator"
    image="/images/cover_data-illustrator.jpg"
    site="dataviz.jp"
    description="Create diverse charts with ease"
>}}
{{< /external-link-card >}}

A bar chart represents the magnitude of one measure against one dimension (category) using the length of bars. For example, this is useful when you want to see the population (measure) for each prefecture (dimension). Since most people know how to read bar charts and they convey numerical values accurately through length, they can be used effectively in many situations.

Because bar charts communicate values through length while also implying area, avoid using triangles instead of rectangles. Length and area do not scale proportionally, making it unclear which encoding the reader should use, which can lead to misinterpretation.

There is no fundamental difference between a vertical bar chart (where bars extend vertically) and a horizontal bar chart (where bars extend horizontally). By convention, the independent variable is often placed on the horizontal axis and the dependent variable on the vertical axis, leading to more frequent use of vertical bar charts. However, this convention does not need to be strictly followed.

Vertical bar charts are preferable when:

- You want to display a bar chart alongside a line chart in the same space
- The display space is wider than it is tall and there are many dimension categories

Horizontal bar charts are preferable when:

- The dimension labels contain long text strings
- You want to include annotations
- The display space is taller than it is wide and there are many dimension categories
