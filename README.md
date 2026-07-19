# tools.data-viz-lectures.com サイト

データ可視化・データ加工ツール群を横断する、中立の総合案内サイトです。
Hugoで構築し、`tools.data-viz-lectures.com` へデプロイします。

このサイトにはサービス別の個別ツール紹介ページやツール本体を置きません。

- データ可視化ツールの個別紹介: `www.dataviz.jp`
- データ加工ツールの個別紹介: `www.dataprep.jp`
- データ可視化ツール本体: `*.dataviz.jp`
- データ加工ツール本体: `*.dataprep.jp`

たとえば Cartogram と Choropleth の個別紹介は `https://www.dataviz.jp/cartogram/` と `https://www.dataviz.jp/choropleth/`、ツール本体は `https://cartogram.dataviz.jp/` と `https://choropleth.dataviz.jp/` です。`/cartogram/` と `/choropleth/` はこのサイトでは公開しません。

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
