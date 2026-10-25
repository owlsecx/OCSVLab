# 🦉 OCSVLab

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-Security-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OCSVLab** — part of the OwlSec Toolkit.

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OCSVLab lets you explore and clean CSV and TSV files without a spreadsheet. It auto-detects the delimiter and column types, then lets you select columns, filter rows with simple expressions, sort, deduplicate and group data. It also produces column statistics and a data-quality report, and converts files to JSON or Markdown.

---

## ✨ Features

- Auto-detects delimiter (comma, tab, semicolon, pipe) and column types (integer, numeric, bool, date, string)
- Preview, column selection and row filtering with expressions (==, !=, ~, >, >=, AND/OR)
- Sort by any column and remove duplicate rows
- Column statistics (min/max/mean/median/stdev/percentiles) and top values for categorical columns
- Group-by aggregates: count, sum, avg, min, max, distinct
- Data-quality report (ragged rows, empty/duplicate columns, nulls, mixed types) and export to JSON / Markdown / CSV

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OCSVLab                                    # interactive menu
./OCSVLab --file data.csv --schema
./OCSVLab --file data.csv --filter "status == failed AND port > 1024"
./OCSVLab --file data.csv --group country --agg count --on ip
./OCSVLab --file data.csv --quality
```

Run `./OCSVLab --help` for the full list of options.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
