---
title: "Word Crowd"
title_en: "Word Crowd"
slug: "word-crowd"
chart_categories:
  - text
chart_subcategories:
  - text-frequency
weight: 300
---

You can create this chart with...

{{< external-link-card
    url="https://word-cloud.dataviz.jp/"
    title="Word Cloud"
    image="/images/cover_wordcloud.png"
    site="dataviz.jp"
    description="日本語に特化したWord Cloud"
>}}
{{< /external-link-card >}}

Words appearing in a document, paragraph, or text are sized based on their frequency and arranged around the center of the chart drawing area. However, since the original character length of words affects their visual size, this chart is not well suited for reading precise numerical values.

Text color can encode an additional variable, but many word clouds in the wild use meaningless random coloring, which is inappropriate as a visual expression (it becomes noise). If there is no suitable variable to map, there is no need to force colorful styling.

