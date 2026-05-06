---
title: Tilegrams
description: タイル地図を作成できるツール
slug: "tilegrams"
weight: 3
categories: "data-visualization-map"
address: https://tilegrams.dataviz.jp/
image: "images/cover_tilegrams.png"
---

{{< external-link-card
    url="https://tilegrams.dataviz.jp/"
    title="Tilegrams"
    image="images/cover_tilegrams.png"
    site="dataviz.jp"
    description="タイル地図を作成できるツール"
>}}
{{< /external-link-card >}}


## どんなツールか？

地理的な地域を六角形タイルで表現し、データに応じて領域サイズを視覚的に変える「タイルグラム（Tiled Cartogram）」 を生成できる Web ベースの地図作成ツールです。地域の面積を人口や指標の大きさに比例させてタイル数で表現しつつ、元の地形の形もある程度保つように配置します。 ￼

## 機能

- 六角形タイルによるカートグラム生成...地理領域を均一な六角形タイルで表現し、データ値に応じて各地域のタイル数を変えて表示。 ￼
- 既存地図の利用／カスタムデータ対応...アメリカやヨーロッパなどの標準地図テンプレートに加え、独自データを読み込んでタイルグラムを生成可能。 ￼
- インタラクティブ調整...タイルをドラッグして配置調整したり、解像度（1タイルが表す数値）を変更して見た目を最適化する編集機能。 ￼
- エクスポート...作成したタイルグラムを SVG や TopoJSON といった形式で出力し、他ツールでの利用や加工が可能。


## 使い方

- 1. ベース地図を選択...用意された地理領域（例：米国州、フランス地域など）から出発。 ￼
- 2. データを指定・読み込み...CSV 形式等で地域ごとの値（人口や投票数など）をアップロード。 ￼
- 3. 解像度・調整設定...1タイルが表す値（例：1タイル＝100万人）を設定し、場合によってはタイルをドラッグで微調整します。 ￼
- 4. 生成・エクスポート...完成したタイルグラムを PNG / SVG / TopoJSON などでダウンロードし、分析や共有に使用。


## データ形式

CSV（カンマ区切り） 形式で地域識別子（Geo ID など）と値（例：人口、得票数）を含む構造。 



![スクリーンショット](images/screen01.png)

![スクリーンショット](images/screen02.png)

![スクリーンショット](images/screen03.png)