---
title: Draw-to-Answer Line Chart
description: An interactive quiz tool where you predict time-series trends by drawing on a line chart
slug: "drawing-line-chart"
weight: 1
categories: "data-visualization"
address: https://drawing-line-chart.dataviz.jp/
image: "images/cover_drawing-line-chart.png"
---

{{< external-link-card
    url="https://drawing-line-chart.dataviz.jp/"
    title="Draw-to-Answer Line Chart"
    image="images/cover_drawing-line-chart.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}


## What is this tool?

"Draw-to-Answer Line Chart" is an interactive quiz builder based on time-series data. Quiz creators upload their data, and respondents predict upcoming trends by drawing directly on the chart. After submitting, the prediction is compared against the actual data and a score is displayed.

![](images/drawing-line-chart_01.png)

## Features

- **CSV upload**: Create quizzes from your own time-series data
- **Sample data**: Try it instantly with built-in datasets — U.S. unemployment rate, Japan's population, inbound tourists to Japan, and USD/JPY exchange rate
- **Date range selection**: Select a portion of the data to define the quiz scope
- **Period annotations**: Overlay contextual labels on the chart, such as political transitions or economic events
- **Hand-drawn style**: Choose between a standard style and a hand-drawn sketch style
- **Publish & share**: Share your quiz via URL or on social media
- **Project save & load**: Save work-in-progress quizzes and resume editing later

## How to use

1. **Upload data** — Drag & drop a CSV file or select a sample dataset
2. **Set the date range** — Specify the start and end of the data range
3. **Configure the quiz** — Enter a title (question), the prediction start point, units, and style
4. **Add annotations (optional)** — Set period labels to display as background context
5. **Preview** — Check the chart in real time on the right panel
6. **Publish** — Generate a URL and share it with respondents

## Data format

CSV files with a header row are supported.

| Column | Content | Example |
|---|---|---|
| X-axis (time series) | Year or year-month | `2000`, `2020/04` |
| Y-axis (numeric) | Any numeric value | `4.9`, `12615`, `105.21` |

```csv
date,value
2000,4.0
2001,4.7
2002,5.8
```

- X-axis supports YYYY (year) or YYYY/MM (year-month) formats
- For multi-column CSVs, you can select the X-axis and Y-axis columns after uploading
- JSON format is also supported ([{"x": 2000, "y": 4.0}, ...])
