---
title: "面グラフ"
title_en: "Area chart"
slug: "area-chart"
chart_categories:
  - time
chart_subcategories:
  - linear-cartesian
weight: 430
---


このチャートを作ることができるのは...

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

折れ線グラフとほぼ同じ作りで、違いは線と軸で囲われた面を色で着色することです。複数のアイテムを1つのチャート内で表示しようとすると、重なりで適切に面が見えない状態になることがあるので注意が必要です。その場合は
着色を半透明の色で行うか、データを集計し直してZ軸で重ならず積み重なるようにするか、代わりにストリームグラフを用いるとよいでしょう。
