---
title: GTFSネットワークデータ変換
description: 交通データGTFSをネットワーク・データに変換します
slug: "gtfs-to-network"
weight: 1
categories: "data-wrangling-map"
address: https://gtfs-to-network.dataprep.jp/
image: "images/gtfs-to-network.png"
---

{{< external-link-card
    url="https://gtfs-to-network.dataprep.jp/"
    title="GTFSネットワークデータ変換"
    image="images/gtfs-to-network.png"
    site="dataprep.jp"
    description="交通データGTFSをネットワーク・データに変換します"
>}}
{{< /external-link-card >}}



## どんなツールか？

交通情報の共通フォーマットである GTFS データを、ネットワーク用のデータに変換します。

## 機能

停留所情報（stops.txt）と通過時刻情報（stop_times.txt）を用いて、CSV形式のネットワーク・データ化します。

### 1. stops.txt (ノード情報として使用)
| 変数名 | 日本語名 | 必須 | 使用用途 |
| :--- | :--- | :--- | :--- |
| `stop_id` | 停留所ID | **Yes** | ノードのID (source/target) として使用。 |
| `stop_name` | 停留所名称 | **Yes** | ノードの名称属性。リンクの始点・終点名としても付与。 |
| `stop_lat` | 緯度 | **Yes** | ノードの座標。 |
| `stop_lon` | 経度 | **Yes** | ノードの座標。 |

### 2. stop_times.txt (リンク集計に使用)
| 変数名 | 日本語名 | 必須 | 使用用途 |
| :--- | :--- | :--- | :--- |
| `trip_id` | 便ID | **Yes** | 同じ便内の移動（A→B）を特定するためにグルーピングに使用。 |
| `stop_id` | 停留所ID | **Yes** | リンクの始点(source)・終点(target)の特定。 |
| `stop_sequence`| 停車順序 | **Yes** | 便内での移動順序の確定（ソートに使用）。 |
| `arrival_time` | 到着時刻 | **Yes** | リンク所要時間（次停留所の到着 - 現停留所の出発）の計算。 |
| `departure_time`| 出発時刻 | **Yes** | リンク所要時間の計算。 |

### 出力データに含まれる属性 (集計・計算値)
| CSVヘッダー | 説明 | 計算方法 |
| :--- | :--- | :--- |
| `frequency` | 便数 | 同一区間 (source→target) を走行する `trip_id` のカウント数。 |
| `avg_duration_sec` | 平均所要時間(秒) | 同一区間の所要時間の平均値。 |


## 使い方

- 1. GTFS ファイルをアップロード...対象の複数ファイルをドラッグ＆ドロップまたはファイル選択で読み込み。 ￼
- 2. 現在の形式を指定...1ファイルか 2ファイルかを選択。 ￼
- 3. 変換開始ボタンを押す...￼
- 4. 変換後、自動でダウンロードされます。


## データ形式

- 入力形式
    - GTFS：停留所情報（stops.txt）
    - GTFS：通過時刻情報（stop_times.txt）
- 出力形式
    - CSV（1列形式）：ノードとリンクを同一ファイル化したもの
    - CSV（2列形式）：ノードとリンクを別ファイル化したもの
