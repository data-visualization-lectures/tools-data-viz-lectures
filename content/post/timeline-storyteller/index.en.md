---
title: Timeline Storyteller
description: Turn timeline data into a story told scene by scene, changing how the timeline is presented along the way
slug: "timeline-storyteller"
weight: 1
categories: "data-visualization"
address: https://timeline-storyteller.dataviz.jp/
image: "images/cover_timeline-storyteller.png"
---

{{< external-link-card
    url="https://timeline-storyteller.dataviz.jp/"
    title="Timeline Storyteller"
    image="images/cover_timeline-storyteller.png"
    site="dataviz.jp"
    description="Draw timelines by combining representation, scale, and layout, then tell a story"
>}}
{{< /external-link-card >}}

## What is this tool?

Timeline Storyteller loads timeline data, lets you choose how to present it, annotate it, and record scenes that tell a story. The shape of a timeline comes from three choices: representation, scale, and layout. The same data can become a straight timeline, a circular one, or a set of timelines lined up by person. Record scenes as you change the presentation and annotations, and you get a story you can play back in order.

It is based on Timeline Storyteller (© Microsoft Corporation), released by Microsoft Research under the MIT License.

## Features

- Representation: Linear, radial, spiral, curve, calendar, and grid
- Scale: Chronological, relative, logarithmic, sequential, and collapsed
- Layout: "Unified" for a single timeline, "Faceted" for one timeline per group, and "Segmented" for splitting by units such as centuries or days
- Annotation: Place event labels, free-text captions, and images on the canvas
- Filtering: Emphasize matching events or hide the others, by category, facet, or segment
- Story: Record the current canvas as a scene and play scenes back in order
- Export: PNG, SVG, an animated GIF that steps through the scenes, and a story file you can keep editing
- Project saving: Save and restore the data and recorded scenes to the cloud
- Available in Japanese and English

## How to use

- Pick a timeline from "Sample Data" in the header, or load your own file from "Open" in the left panel
- Choose a representation, scale, and layout in the top panel. Options that cannot be combined are dimmed
- Click an event to add its label, then add captions or images
- Press the red circle button at the bottom to record the current view as a scene. Change the presentation and record again
- Press the frame button to enter playback mode and step through the scenes with the arrows
- Save images or a GIF from "Export" in the left panel. Use "Save Project" in the header to keep your work in the cloud

## Data format

- File format: CSV / JSON
- One row (one item) is one event
- `start_date` (required): Start date, written as `YYYY`, `YYYY-MM`, `YYYY-MM-DD`, or `YYYY-MM-DD HH:MM`. Write BC years as negative numbers, such as `-27`
- `end_date` (optional): End date. Leave it out for an event at a single point in time
- `content_text` (optional): Description of the event, shown as its label
- `category` (optional): Group of the event, used for color
- `facet` (optional): A second grouping, used to split the timeline into several

A CSV example:

```
start_date,end_date,content_text,facet,category
1868-10-23,1912-07-30,Meiji,Era,Era
1923-09-01,,Great Kanto Earthquake,Event,Disaster
```
