---
title: Choosing a map projection
description: "Pick a map projection by deciding which property to preserve: angle, area, or distance"
slug: "map-projection-chooser"
weight: 4
categories: "data-visualization-map"
address: https://map-projection-chooser.dataviz.jp/
image: "images/cover_map-projection-chooser.png"
---

{{< external-link-card
    url="https://map-projection-chooser.dataviz.jp/"
    title="Choosing a map projection"
    image="images/cover_map-projection-chooser.png"
    site="dataviz.jp"
    description="Pick a map projection by deciding which property to preserve"
>}}
{{< /external-link-card >}}

## What is this tool?

No map projection can preserve angle, area, and distance at the same time. This tool helps you choose a projection from the property you care about most, then observe and compare distortion.

## Features

- Start from a property...Choose conformal, equal-area, equidistant, or compromise.
- Observe distortion...Tissot indicatrices and a graticule show what is preserved and what is warped.
- Compare projections...Place two projections side by side.
- Export...Download the chosen projection as design-ready SVG, or copy the D3 call.

## How to use

- 1. Choose the property you want to preserve.
- 2. Open one of the candidate projection cards.
- 3. Drag the map to change the center and inspect distortion with Tissot ellipses.
- 4. Compare another projection if needed, then export SVG or D3 code.
