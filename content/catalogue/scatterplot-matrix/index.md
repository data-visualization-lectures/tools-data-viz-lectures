---
title: "散布図行列"
title_en: "Scatterplot Matrix"
slug: "scatterplot-matrix"
chart_categories:
  - numeric
chart_subcategories:
  - correlation
weight: 280
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

あるデータセット内の変数を総当たりで相関を探すために、変数を同じように行列に並べ、その交差する箇所にそれぞれの変数を用いた散布図を描くことで、より効率よく探索できます。

交差する2つの変数が同一のものの場合、相関を知る必要がないため、そこにはヒストグラムを示します。交差する2つの変数に順序はないため、同じ2つの変数の組み合わせが2箇所に存在することになります。そのため、同じものを表示するのではなく、1箇所に相関係数を示すことがあります。

