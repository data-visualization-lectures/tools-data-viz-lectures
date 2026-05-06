---
title: Coloring Administrative District Maps with Data
description:
slug: "choropleth-fukushima"
weight: 1
categories: "showcase"
image: "images/cover_choropleth-fukushima.png"
---

Coloring administrative district maps — commonly known as blank maps — with data is called a "choropleth map." Although sometimes referred to as a "classified area map," <a href="https://visualizing.jp/classification-and-coloplethmap/" target="_blank">that term actually describes a data processing technique, not a visualization type</a>.

Using our "Japan Choropleth Map" and "Prefecture Choropleth Map" tools, you can easily create high-quality choropleth maps.

![Finished map](images/cover_choropleth-fukushima.png)

Here we introduce how to create one using our tools.

{{< external-link-card
    url="https://choropleth-prefectures.dataviz.jp/?project_id=dbbe184f-2022-403b-a84f-525991e61725"
    title="Fukushima Prefecture: Population Change Rate 2011–2024"
    image="images/cover_choropleth-fukushima.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

Paid subscribers can open the link above as an editable project file to learn the process and examine the data structure.


### Visualizing with Sample Data

![Blank map of Fukushima Prefecture](images/cf_1_1.png)

Here is what it looks like when you visualize pre-loaded population data on a Fukushima Prefecture map. By turning on the "Divide by area (/km²)" checkbox, the data becomes population density.

![Population density of people under 15 in Fukushima Prefecture](images/cf_1_2.png)

Incidentally, using a technique called a cartogram — which distorts area to reflect data (also available as a tool) — produces a warped map like this:

![Cartogram of population density of people under 15 in Fukushima Prefecture](images/cf_1_3.png)


### Visualizing with Your Own Data

You can of course prepare and visualize your own data.

In that case, download the sample data and keep only the place names to see what geographic names you need to prepare data for.

![Downloaded sample file](images/cf_1_4.png)

![Keep only the municipality name column](images/cf_1_5.png)

### Population Comparison Data Between 2011 and 2024

Download the "<a href="https://www.pref.fukushima.lg.jp/uploaded/attachment/702454.xlsx" target="_blank">Fukushima Prefecture Current Population Survey Annual Report: Reference Materials</a>" published by Fukushima Prefecture. This dataset compares population between 2011 and 2024.

![Opening the downloaded data](images/cf_2_1.png)

Keep only the sheet and table you need.

![](images/cf_2_2.png)

Once you have this, load it into OpenRefine for cleansing.

![](images/cf_2_3.png)

Remove unnecessary spaces and commas.
The minus sign is represented as "△", so replace it with the minus symbol "-".

![](images/cf_2_4.png)

Also load the file with only municipality names from the sample data into OpenRefine as a separate project.

![](images/cf_3_1.png)

Use the "Add column based on this column" operation to perform a VLOOKUP-like join — merging two tables horizontally.

![](images/cf_3_2.png)

Join using an OpenRefine-specific script:

```
cell.cross('PROJECT_NAME','KEY_COLUMN_NAME').cells['COLUMN_NAME_TO_GET'].value[0]
```

- PROJECT_NAME — the project name of your original data
- KEY_COLUMN_NAME — the name of the column to use as the key
- COLUMN_NAME_TO_GET — the name of the column you want to join

![](images/cf_3_3.png)

You can see that the join was successful for all municipalities except Futaba, Namie, Okuma, and Tomioka, where no data exists.

![](images/cf_3_4.png)

Municipalities with higher population change rates are displayed in darker colors.

![](images/cf_3_5.png)
