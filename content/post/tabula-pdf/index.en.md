---
title: Tabula PDF
description: "Extract table data from PDFs"
slug: "tabula-pdf"
weight: 1
categories: "data-wrangling"
address: https://tabula-pdf.dataprep.jp/
image: "images/cover_tabula-pdf.jpg"
---

{{< external-link-card
    url="https://tabula-pdf.dataprep.jp/"
    title="Tabula PDF"
    image="images/cover_tabula-pdf.jpg"
    site="dataprep.jp"
    description="PDFから表データを取り出す"
>}}
{{< /external-link-card >}}

## What is this tool?

Tabula PDF is a tool for extracting tables from PDFs and converting them into reusable formats.
It is useful when you want to use tables from PDFs published as government documents, survey reports, handouts, and similar materials as data.

You can specify the area of the table to extract on the page, and export it as CSV / JSON / Excel format.
It helps you create a starting point for data processing in situations where "you have the PDF but not the original data."

## Features

- Table extraction from PDF (page-by-page and multi-page support)
- Manual selection of table regions (drag) with extraction preview
- Switching extraction modes (rule-based / whitespace-based)
- Batch output of multiple tables
- Download in CSV / JSON / Excel formats

## How to use

- 1. Upload a PDF file
- 2. Open the target page and select the table area to extract
- 3. Choose the extraction mode and review the preview
- 4. If everything looks correct, export as CSV / JSON / Excel

## Data formats

- Input: PDF
- Output: CSV, JSON, Excel

## Notes

- This tool is intended for use with PDFs that contain text data.
- For PDFs consisting primarily of scanned images, running OCR beforehand will improve extraction accuracy.
