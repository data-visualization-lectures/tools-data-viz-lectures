---
title: Vega Editor
description: "Write visualization specs in JSON to render interactive graphs and charts in real time"
slug: "vega-editor"
weight: 10
categories: "data-visualization"
address: https://vega-editor.dataviz.jp/
image: "images/cover_vega-editor.jpg"
---

{{< external-link-card
    url="https://vega-editor.dataviz.jp/"
    title="Vega Editor"
    image="images/cover_vega-editor.jpg"
    site="dataviz.jp"
    description="JSON 形式で可視化仕様を書くことで、インタラクティブなグラフやチャートをリアルタイムにレンダリング"
>}}
{{< /external-link-card >}}


## What is this tool?

Vega Editor is a web-based IDE (editor) for writing, editing, and previewing Vega and Vega-Lite visualization specifications. By writing visualization specifications in JSON format, you can render interactive graphs and charts in real time. Vega and Vega-Lite are declarative visualization grammars that generate charts by defining data and display rules in JSON.


## Features

- Text editor / code view...Provides an editor for entering and editing Vega/Vega-Lite JSON.
- Real-time preview...Instantly displays the edited specification as a visualization in the browser.
- Samples and templates...Load example specs for learning and experimentation (a feature of the official version).
- Vega / Vega-Lite mode switching...Edit and preview in both specification formats (a standard feature of the official tool).
- Sharing / Export...Save and share specifications via GitHub Gist and other backend integrations (an official version feature).



## How to use

- 1. Write specifications in JSON format...Enter Vega or Vega-Lite specifications into the editor.
- 2. View the preview...The specification is rendered in real time so you can review the results.
- 3. Save and share as needed...Save specifications to Gist or similar services for sharing with others (when backend integration is available).

## Data formats

- JSON (Vega / Vega-Lite specification)...Describes the visualization definition (data references, transforms, encodings, marks, etc.) in JSON.
- Tabular data as data sources...Vega/Vega-Lite can load external data either by embedding it directly within the JSON or by referencing CSV/TSV file URLs (as part of the specification standard).
