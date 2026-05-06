---
title: ADS-B / AIS Visualization
description: "Easily create videos from aircraft and ship movement data"
slug: "bbts"
weight: 10
categories: "data-visualization-map"
address: https://bbts.dataviz.jp/
image: "images/cover_broadcast-tracking-system.jpg"
---

{{< external-link-card
    url="https://bbts.dataviz.jp/"
    title="ADS-B / AIS Visualization"
    image="images/cover_broadcast-tracking-system.jpg"
    site="dataviz.jp"
    description="Easily create videos from aircraft and ship movement data"
>}}
{{< /external-link-card >}}


## What is this tool?

A web tool that visualizes tracks on a map with animation simply by uploading a CSV file containing latitude and longitude data. It supports visualization of broadcast-type positioning data such as ADS-B (aircraft tracking) and AIS (ship tracking).


## Features

- CSV Upload: Load CSV files via drag & drop or file selection
- Track Visualization: Animate movement paths on a map based on time-series data
- Multiple Track Support: Automatically groups and displays multiple aircraft or vessels from a single CSV
- Auto Column Detection: Automatically recognizes column names like lat/lon, latitude/longitude regardless of case
- Sample Data: Ready-to-use sample data available for quick testing

## How to use

- Prepare a CSV file (containing latitude, longitude, and timestamp)
- Drag & drop or click to select a file from the sidebar on the left
- Sample data is also available
- Tracks are automatically drawn on the map
- Export as GIF animation, sequential still images, or video files
- Customize base map style, date/time display, and other options


## Data formats

Include the following variables in your CSV:

- Position (required): lat / lon, latitude / longitude, or Position ("lat,lon" combined format)
- Time (required): Timestamp (Unix epoch seconds), etc.
- Identifier: Callsign (aircraft), MMSI / VesselName (vessel)
- Optional: Altitude, Speed, Direction / Course

### Supported position data formats

Column names are case-insensitive (e.g., LAT, Lat, lat are all accepted).

| Column Name | Description |
|------|-----|
| `lat` / `lon` | Latitude / Longitude (abbreviated) |
| `latitude` / `longitude` | Latitude / Longitude (full name) |
| `Position` | Combined lat/lon format (`"35.68,139.76"`) |



### Supported time data formats

Time data is automatically detected in the following formats. Supported column names include timestamp, time, datetime, date, etc.

| Format | Example |
|------|-----|
| ISO 8601 | `2023-05-20T10:30:00Z` |
| Date-time string | `2023-05-20 10:30:00` |
| Compact format | `20230520_103000` |
| Unix timestamp (seconds) | `1684567890` |
| Unix timestamp (milliseconds) | `1684567890123` |


When a single CSV contains multiple aircraft or vessels, they are automatically grouped and displayed.

## Reference

- [What is ADS-B?](https://visualizing.jp/ads-b/)
- [What is AIS?](https://visualizing.jp/ais/)
