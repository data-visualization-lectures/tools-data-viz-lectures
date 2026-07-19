# tools.data-viz-lectures.com サイト

データ可視化・データ加工ツール群を横断して紹介する、中立の総合案内サイトです。
Hugoで構築し、`tools.data-viz-lectures.com` へデプロイします。

このサイトの各ツールページは紹介ページであり、ツール本体の配信先ではありません。

- データ可視化ツール本体: `*.dataviz.jp`
- データ加工ツール本体: `*.dataprep.jp`
- サービス別の公開サイト: `www.dataviz.jp` / `www.dataprep.jp`

たとえば `/cartogram/` と `/choropleth/` は紹介ページです。実際のツール起動先は、それぞれ `https://cartogram.dataviz.jp/` と `https://choropleth.dataviz.jp/` です。

## ローカルテスト

http://localhost:1313/?auth_debug




## 外部リンク用のカスタムスタイル

```
{{< external-link-card
    url="https://example.com/post"
    title="Example Post"
    image="https://example.com/ogp.jpg"
>}}
{{< /external-link-card >}}
```
