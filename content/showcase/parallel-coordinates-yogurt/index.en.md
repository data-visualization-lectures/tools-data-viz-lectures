---
title: Finding the Ideal Yogurt with Parallel Coordinates
description:
slug: "parallel-coordinates-yogurt"
weight: 1
categories: "showcase"
image: "images/cover_yogurt.png"
---


Let's find the "ideal yogurt" — high in protein, low in sugar.

With a <a href="/en/parallel-coordinates/">Parallel Coordinates chart</a>, you can easily filter data by applying multiple conditions simultaneously.

![Finished chart](images/yogurt_02.png)

Here we show how to create this using our tools.

{{< external-link-card
    url="https://parallel-coordinates.dataviz.jp//?project_id=6c3cf78f-9eec-4d37-9c79-24a92342f699"
    title="Finding the Ideal Yogurt with Parallel Coordinates"
    image="images/cover_yogurt.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

Paid subscribers can open the link above as an editable project file to learn the process and examine the data structure.


## Collecting the Data

First, we gathered nutritional information for yogurts sold at convenience stores, collecting data from each manufacturer's website.

## Visualizing with Parallel Coordinates

After loading nutritional data for 70 yogurt products and switching to Min-Max scale, metrics with different units are normalized to the same 0–1 axis.

![](images/yogurt_01.png)

## Filtering Across Multiple Axes

By brushing the upper range on the protein axis and the lower range on the carbohydrate axis, only products meeting the "high protein, low sugar" criteria remain as blue lines.

![](images/yogurt_02.png)

The standout result is PARTHENO Plain, a rich Greek yogurt — 10.9g of protein with just 4.6g of carbohydrates.

## Reordering Axes

Try dragging axes to rearrange them, and hover over table rows to highlight the corresponding lines. Experience how the "feel" of the data changes with different arrangements.
