---
title: Gephi Lite
description: "Create network graphs with ease"
slug: "gephi-lite"
weight: 10
categories: "data-visualization"
address: https://gephi-lite.dataviz.jp/
image: "images/cover_gephi-lite.jpg"
---

{{< external-link-card
    url="https://gephi-lite.dataviz.jp/"
    title="Gephi Lite"
    image="images/cover_gephi-lite.jpg"
    site="dataviz.jp"
    description=""
>}}
{{< /external-link-card >}}


## What is this tool?

Gephi Lite is a web application that allows you to easily create network graphs (relationship visualizations) in your browser. You can load data composed of nodes (points) and edges (lines), and intuitively perform layout calculations, color coding, filtering, and more.


## Features

- **Graph Visualization**: Interactively display relationships between nodes and edges. Zoom, pan, and node selection are supported
- **Layout Calculation**: Multiple layout algorithms including ForceAtlas2, Force Directed, Circular, and CirclePack
- **Appearance Settings**: Automatically assign colors, sizes, and labels to nodes and edges based on attribute values
- **Filtering**: Narrow down the display of nodes and edges by attribute values or range specifications
- **Metrics Calculation**: Compute network analysis metrics such as degree, PageRank, betweenness centrality, and Louvain community detection
- **Data Table**: View and edit node and edge attributes in a list format
- **Export**: Export as graph images (PNG) or graph data (GEXF)
- **Japanese/English Auto-Switch**: The UI automatically switches based on your browser's language settings


## How to use

1. When you access the page, a sample graph or an empty workspace will be displayed
2. Load data using the "Open Data File" button at the top of the screen, or by dragging and dropping a file
3. Select "Layout" from the left side menu and run an algorithm to automatically arrange the nodes
4. In the "Appearance" menu, set colors and sizes based on attributes to make the graph easier to read
5. Deepen your analysis using "Filters" and "Metrics"
6. The completed graph can be exported as an image (PNG) or data file (GEXF)

## Data formats

The following file formats are supported.

| Format | Extension | Description |
|--------|-----------|-------------|
| **CSV** | `.csv` | Edge list format. The first row contains headers (Source, Target, etc.), and subsequent rows contain the data for each edge. The simplest format |
| **GEXF** | `.gexf` | Gephi's standard XML format. Retains rich node/edge attributes and visual information |
| **GraphML** | `.graphml` | A standard XML-based graph description format |
| **Graphology JSON** | `.json` | JSON format for the Graphology library |

**CSV file format example:**

```csv
Source,Target,Weight
Alice,Bob,1.0
Bob,Charlie,2.0
Alice,Charlie,1.5
```

- The first row is the header (required)
- The `Source` (or `From`, `Src`) and `Target` (or `To`, `Dst`) columns are automatically detected
- Other columns (such as Weight) are imported as edge attributes
- Nodes are automatically generated from the Source / Target values
- Character encoding supports both **UTF-8** and **Shift_JIS**


