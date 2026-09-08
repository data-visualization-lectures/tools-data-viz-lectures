---
title: Race Chart Builder
description: Build animated race charts in five templates to show ranking changes over time
slug: "race-chart-builder"
weight: 2
categories: "data-visualization"
address: https://race-chart-builder.dataviz.jp/
image: "images/cover_race-chart-builder.png"
---

{{< external-link-card
    url="https://race-chart-builder.dataviz.jp/"
    title="Race Chart Builder"
    image="images/cover_race-chart-builder.png"
    site="dataviz.jp"
    description="Build animated race charts in five templates to show ranking changes over time"
>}}
{{< /external-link-card >}}

## What is this tool?

A race-chart builder for animating how rankings and values change over time. Choose one of five templates — bar chart race, bump chart, line chart, scatter plot race, or slope graph — then load a CSV and play it back. Annotations, export, cloud save, and public sharing are included.

## Features

- Chart picker: five templates from a catalog on the home screen
- Sample data: featured works for each chart type autoload first; switch from the sample picker
- Playback: play, pause, speed, and loop as time steps advance
- Annotations: title, source, and source URL on the chart
- Appearance: palette, number format, and labels
- Export: SVG / PNG / CSV
- Share: publish a public page (`share.html?id=`) from a saved project
- Project save: store data and settings in the cloud and restore later

## How to use

1. Pick a chart type (or let a sample open automatically)
2. Upload a CSV or load a sample
3. Play the animation and check rankings, crossings, and overtakes
4. Add a title and source in the annotation tab
5. Export an image or CSV, save as a project, and publish a share page if needed

## Data format

- File format: CSV (comma-separated, UTF-8)
- Bar / bump / line / slope: wide table. `name` (series), optional `category` (color), then time-step columns (years, etc.)
- Scatter plot race: long table. `date`, `name`, `category`, plus numeric columns for position and size
- First row is the header. Time columns run from oldest to newest, left to right
