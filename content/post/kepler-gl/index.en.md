---
title: kepler.gl
description: "Visualization and exploration tool for large-scale geospatial data"
slug: "kepler-gl"
weight: 1
categories: "data-visualization-map"
address: https://kepler-gl.dataviz.jp/
image: "images/cover_kepler-gl.jpg"
---

{{< external-link-card
    url="https://kepler-gl.dataviz.jp/"
    title="大規模地理空間データの可視化・探索ツール"
    image="images/cover_kepler-gl.jpg"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

## What is this tool?

A browser-based tool for visualizing and exploring large-scale geospatial data. It leverages WebGL to produce high-performance map visualizations that enable intuitive analysis of location data. Originally developed by Uber as an open-source GIS tool, it allows data exploration without any programming.


## Features

- Diverse layer types: Supports multiple layers including points, lines, polygons, heatmaps, hexbin aggregation, arcs, and more.
- Interactive operations: Explore data through filtering, zooming, panning, and time-axis animations.
- High-performance rendering: Uses WebGL to smoothly render millions of data points at high speed.
- Style settings and customization: Adjust color coding, scale settings, 3D representation (height/extrude), and many other display options.
- Export: Save and share completed maps as PNG images or interactive HTML, as well as CSV file output.
- Save and load created projects

## How to use

- 1. Add data: Drag and drop CSV or GeoJSON files to load them.
- 2. Configure layers: Select a type (point/polygon, etc.) from the layer panel and assign columns such as latitude and longitude.
- 3. Customize: Adjust colors, sizes, filters, and scales to optimize the visualization.
- 4. Save and share: Save settings and maps (locally/export) for reuse.



## Data formats

- CSV
- Json
- GeoJSON
- Arrow
- Parquet
