# Data Note

## Overview

This project is different from a typical analytics project with a shared CSV or SQL dataset.

The main inputs for this project were:

- public company filings
- public business and news sources
- manually structured risk scores
- manually prepared working Excel files
- manually defined scenario assumptions
- simulated six-quarter revenue outputs

## What Data Is Actually Used Here

This repository does **not** include a large raw tabular dataset.

The project mainly used:

1. **Public source material for business context**
2. **Small project working files for risk scoring**
3. **Scenario assumptions used inside the notebook**

## Public Source Used for Company Baseline

The most important public source in this project was NVIDIA’s annual report / Form 10-K.

### NVIDIA 2024 Annual Report (Form 10-K)
Direct source:
https://s201.q4cdn.com/141608511/files/doc_financials/2024/ar/NVIDIA-2024-Annual-Report.pdf

I used this source as the main baseline for company background and revenue context.

## Why I Did Not Upload the NVIDIA Annual Report to This Repo

I did not include the NVIDIA annual report PDF directly in this repository because:

- it is a large external source file
- it is not my own project output
- the report is already publicly available from NVIDIA
- linking to the original source keeps the repo cleaner and easier to review

So for GitHub, I decided to keep the source link here instead of re-uploading the full PDF.

## Project Working Files

This project also used small manually structured working files created during the course process.

Those original files are kept in the `archive/` folder:

- [`../archive/nvidia-risk-calculation-sheet-original.xlsx`](../archive/nvidia-risk-calculation-sheet-original.xlsx)
- [`../archive/nvidia-risk-register-original.xlsx`](../archive/nvidia-risk-register-original.xlsx)

These are not raw downloaded datasets. They are project working files used to organize:

- risk names
- chance scores
- impact scores
- final risk scores
- mitigation notes
- risk owner notes

## Notebook Input Style

The notebook in this repo does **not** read a CSV or database file.

Instead, it uses manually defined values such as:

- final risk scores for the heat map
- final scenario values for Monte Carlo analysis
- labels for risk paths and categories

## Main Public Sources Mentioned in the Project

Examples of public sources used in the project include:

- NVIDIA 2024 Annual Report (Form 10-K)
- NVIDIA SWOT analysis
- NASA Risk Management Handbook
- public business and news articles referenced in the final report

## Public Repository Note

No private company data, internal business data, or personal data is included in this repository.