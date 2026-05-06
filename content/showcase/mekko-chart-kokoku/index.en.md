---
title: Exploring Two Variables at Once with a Mekko Chart
description:
slug: "mekko-chart-kokoku"
weight: 1
categories: "showcase"
image: "images/kokoku_fin.png"
---

Every year, Dentsu publishes "Advertising Expenditures in Japan." We visualized the advertising expenditure by industry across four traditional media (excluding the internet).

![Completed chart](images/kokoku_fin.png)

Normally, using bar charts or pie charts would require creating as many charts as there are industries (21) or media types (4). With a Mekko chart, however, you can represent both dimensions as vertical and horizontal proportions within a single chart.

Here we introduce how to create one using the tools provided by this service.

{{< external-link-card
    url="https://rawgraphs.dataviz.jp/?project_id=cff8e9c7-e4bf-4d82-b3f5-e7a6fbe55212"
    title="Advertising Expenditure by Industry and Mass Media (2025)"
    image="images/kokoku_fin.png"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}

Paid users can open the link above as an editable project file to learn how it was made and examine the data structure.

The data is sourced from Dentsu's PDF report.

- [2025 Advertising Expenditures in Japan - Dentsu](https://www.dentsu.co.jp/news/release/2026/0305-011003.html)


## Extracting Table Data from a PDF

The published materials are available as a PDF. As-is, this data cannot be processed by a computer. Manual data entry would be tedious.

![Cover page](<images/2025年 日本の広告費_p01.png>)
![Relevant page](<images/2025年 日本の広告費_p14.png>)

In cases like this, Tabula makes it easy to extract table data from PDFs.

{{< external-link-card
    url="https://tabula-pdf.dataprep.jp/"
    title="Tabula PDF"
    image="images/cover_tabula-pdf.jpg"
    site="dataprep.jp"
    description="Extract table data from PDFs"
>}}
{{< /external-link-card >}}

![Select the data range to extract](images/kokoku_01.png)

![Visually confirm the optimal algorithm and export as CSV](images/kokoku_02.png)

## Cleansing the Data

To transform the data into a tidy format that computers can process, OpenRefine is very useful. It allows you to cleanse data with visual confirmation.

![CSV file loaded into OpenRefine](images/kokoku_03.png)

We removed unnecessary columns, as well as unnecessary spaces and commas.

![Removed unnecessary columns, spaces, and commas](images/kokoku_05.png)

The data is still in a cross-tabulation (matrix) format, so we need to perform the reverse of a pivot table in Excel. OpenRefine lets you do this visually as well.

![Transpose columns to rows (unpivot)](images/kokoku_06.png)

![Specify column names after transformation](images/kokoku_07.png)

![Data in tidy format](images/kokoku_08.png)

Data cleansing is now complete.
Choose your favorite visualization tool.
In this case, we'll use RawGraphs, which makes it easy to create Mekko charts.

## Visualizing Data with RawGraphs

RawGraphs is a single-page tool where each step appears as you scroll down.

![Load the data](images/kokoku_09.png)

![Select the chart type](images/kokoku_10.png)

![Map data columns to visual and spatial variables](images/kokoku_11.png)

![Fine-tune the layout](images/kokoku_12.png)


## Completed

Export as PNG to include in slides or publish on the web.

![Completed chart](images/kokoku_fin.png)

Export as SVG to edit in design tools such as PowerPoint, Adobe Illustrator, or Figma.
Some axis labels were too close together, so we adjusted them.

### Editing in PowerPoint

![Editing in PowerPoint](images/kokoku_fin_pt.png)

### Editing in Adobe Illustrator

![Editing in Adobe Illustrator](images/kokoku_fin_ai.png)
