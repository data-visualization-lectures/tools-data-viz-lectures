---
title: 行政区割の地図に塗り絵のようにデータで着色する
description: 
slug: "choropleth-fukushima"
weight: 1
categories: "showcase"
image: "images/cover_choropleth-fukushima.png"
---

いわゆる白地図とよばれる行政区割の地図に、塗り絵のようにデータで着色することを「コロプレス・マップ」といいます。階級区分図と呼ばれることもありますが、<a href="https://visualizing.jp/classification-and-coloplethmap/" target="_blank">これはデータ加工の手法なので、可視化名称とは異なります</a>。

本サービスの「日本地図コロプレス」や「都道府県地図コロプレス」を用いれば、かんたんに高品質なコロプレス・マップを作成することができます。

![完成図](images/cover_choropleth-fukushima.png)

ここでは本サービスのツールを用いた作成の仕方を紹介します。

{{< external-link-card
    url="https://choropleth-prefectures.dataviz.jp/?project_id=dbbe184f-2022-403b-a84f-525991e61725"
    title="福島県_人口の増減率_2011-2024"
    image="images/cover_choropleth-fukushima.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

有料ユーザーであれば、上記リンクから編集可能なプロジェクト・ファイルとして開くことができ、作り方を学んだり、データのあり方を確認することができます。


### サンプルデータでの可視化

![白地図状態の福島県](images/cf_1_1.png)

あらかじめ用意してある人口データを福島県の地図で可視化することこのようになります。「面積で割る（/km²）」チェックボックスをONにすることで人口密度のデータになります。

![福島県における15歳未満人口の人口密度](images/cf_1_2.png)

ちなみにカルトグラムとよばれる面積にもデータを反映させる手法（これもツールとして用意してあります）を用いるとこのように地図が歪んだような表現になります。

![福島県における15歳未満人口の人口密度](images/cf_1_3.png)


### オリジナル・データでの可視化

自分でデータを用意して可視化することももちろん可能です。

その場合はサンプルデータをダウンロードし、地名だけ残すと、どんな地名ごとにデータを用意すればいいかわかりやすいです。

![ダウンロードしたサンプルファイル](images/cf_1_4.png)

![必要な市区町村名の列のみを残します](images/cf_1_5.png)

### 2011年と2024年で人口を比較しているデータ

福島県が公開している「<a href="https://www.pref.fukushima.lg.jp/uploaded/attachment/702454.xlsx" target="_blank">福島県現住人口調査年報 資料編</a>」をダウンロードします。このデータには2011年と2024年で人口を比較しているデータです。

![取得したデータを開いたところ](images/cf_2_1.png)

使用するシートのみを残し、かつ使用する表のみを残します。

![](images/cf_2_2.png)

ここまでできたら OpenRefine に読み込んでクレンジングしていきます。

![](images/cf_2_3.png)

不要な空白やコンマを取り除きます。
マイナス表現が「△」になっているので、マイナス記号「-」にしておきます。

![](images/cf_2_4.png)

サンプルデータをダウンロードして市区町村名のみにしたファイルも OpenRefine で別なプロジェクトとして読み込みます。

![](images/cf_3_1.png)

「このカラムに基づいてカラムを追加」という操作で、ExcelでいうVLOOKUPのような操作、二つの表を横方向に結合します。

![](images/cf_3_2.png)

OpenRefine 専用スクリプトで結合します。

```
cell.cross('PROJECT_NAME','KEY_COLUMN_NAME').cells['COLUMN_NAME_TO_GET'].value[0]
```

- PROJECT_NAME...オリジナルデータのプロジェクト名
- KEY_COLUMN_NAME...キーとしたい列の名称
- COLUMN_NAME_TO_GET...結合したい列の名称

![](images/cf_3_3.png)

データが存在しない双葉町、浪江町、大熊町、富岡町以外はうまく結合できていることがわかります。

![](images/cf_3_4.png)

人口の増減率が高い自治体ほど色が濃く表現されています。

![](images/cf_3_5.png)

