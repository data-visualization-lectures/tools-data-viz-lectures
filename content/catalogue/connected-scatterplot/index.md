---
title: "連結散布図"
title_en: "Connected Scatterplot"
slug: "connected-scatterplot"
chart_categories:
  - time
chart_subcategories:
  - linear-cartesian
weight: 450
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

普通の散布図のように二軸に変数を割り当てます(図16‐7)。 そして描画された点を時系列の順で接続します。両軸には日時スケールが使用されません。2つの変数間の時間差をループの形として効果的に表現できたり、形状の特徴的な部分にアノテーションをつけやすいという利点がありますが、新奇性と解読の難しさのトレードオフとなります。

