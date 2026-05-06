---
title: GTFSネットワークデータ変換
description: "Convert GTFS transit data to network data"
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



## What is this tool?

Converts GTFS data, a common format for transit information, into network data.

## Features

Uses stop information (stops.txt) and stop time information (stop_times.txt) to generate network data in CSV format.

### 1. stops.txt (used as node information)
| Variable | Description | Required | Usage |
| :--- | :--- | :--- | :--- |
| `stop_id` | Stop ID | **Yes** | Used as node ID (source/target). |
| `stop_name` | Stop name | **Yes** | Node name attribute. Also assigned as origin/destination names for links. |
| `stop_lat` | Latitude | **Yes** | Node coordinates. |
| `stop_lon` | Longitude | **Yes** | Node coordinates. |

### 2. stop_times.txt (used for link aggregation)
| Variable | Description | Required | Usage |
| :--- | :--- | :--- | :--- |
| `trip_id` | Trip ID | **Yes** | Used for grouping to identify movements (A to B) within the same trip. |
| `stop_id` | Stop ID | **Yes** | Identifies the source and target of each link. |
| `stop_sequence`| Stop sequence | **Yes** | Determines travel order within a trip (used for sorting). |
| `arrival_time` | Arrival time | **Yes** | Calculates link travel time (next stop arrival - current stop departure). |
| `departure_time`| Departure time | **Yes** | Calculates link travel time. |

### Output data attributes (aggregated/calculated values)
| CSV Header | Description | Calculation Method |
| :--- | :--- | :--- |
| `frequency` | Number of trips | Count of `trip_id`s traversing the same segment (source to target). |
| `avg_duration_sec` | Average travel time (seconds) | Average travel time for the same segment. |


## How to use

- 1. Upload GTFS files...Load the target files via drag-and-drop or file selection.
- 2. Specify the current format...Select whether it is 1 file or 2 files.
- 3. Press the convert button...
- 4. After conversion, the file is automatically downloaded.


## Data formats

- Input formats
    - GTFS: Stop information (stops.txt)
    - GTFS: Stop time information (stop_times.txt)
- Output formats
    - CSV (single-file format): Nodes and links combined in a single file
    - CSV (two-file format): Nodes and links in separate files
