---
title: Tabula PDF
description: PDFから表データを取り出す
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

## どんなツールか？

Tabula PDF は、PDF 内の表を抽出して再利用しやすい形式に変換するツールです。  
行政資料・調査報告書・配布資料など、PDF で公開された表をデータとして使いたい場面で役立ちます。

抽出したい表の範囲をページ上で指定し、CSV / JSON / Excel 形式で書き出せます。  
「PDF はあるが元データが手元にない」という状況で、データ整形の出発点を作れます。

## 機能

- PDF からの表抽出（ページ単位・複数ページ対応）
- 表領域の手動選択（ドラッグ）と抽出プレビュー
- 抽出モードの切り替え（罫線ベース / 余白ベース）
- 複数テーブルの一括出力
- CSV / JSON / Excel 形式でのダウンロード

## 使い方

- 1. PDF ファイルをアップロード
- 2. 対象ページを開き、抽出したい表領域を選択
- 3. 抽出モードを選んでプレビューを確認
- 4. 問題なければ CSV / JSON / Excel のいずれかで出力

## データ形式

- 入力：PDF
- 出力：CSV、JSON、Excel

## 補足

- 文字情報を持つ PDF での利用を想定しています。
- スキャン画像中心の PDF は、事前に OCR を行うと抽出精度が上がります。
