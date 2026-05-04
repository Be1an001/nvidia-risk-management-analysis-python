# Data and Assumptions

This repository does not include a large raw dataset, CSV file, SQL database, or private company data. The project is a scenario-based risk analytics case study built from public sources, manually structured risk scores, and manually defined simulation assumptions.

## Main Inputs

The project used three main input types:

- public company and industry sources for business context
- small project working files for risk scoring and risk register structure
- scenario assumptions entered directly in the notebook

The working files are stored in the `archive/` folder:

- [Risk calculation sheet](../archive/nvidia-risk-calculation-sheet-original.xlsx)
- [Risk register](../archive/nvidia-risk-register-original.xlsx)
- [Treatment and response plan](../archive/nvidia-risk-treatment-and-response-plan-original.docx)

These files are project artifacts, not raw downloaded datasets.

## Public Source Baseline

The main company baseline source referenced in the project is NVIDIA's 2024 annual report / Form 10-K.

Source:
https://s201.q4cdn.com/141608511/files/doc_financials/2024/ar/NVIDIA-2024-Annual-Report.pdf

I did not upload the NVIDIA annual report PDF directly into this repository because it is an external public source, not my own project output.

## Risk Scoring Data

The archived workbooks organize the manually scored risk information, including:

- risk names
- risk causes and consequences
- chance scores
- impact scores
- risk scores
- priority labels
- mitigation notes
- risk owner notes

The final risk register contains six risks and identifies geopolitical tensions and supply chain disruptions as the highest-priority risks in the final scoring.

## Notebook Input Style

The notebook does not load a CSV file or query a database. It defines scenario values directly in code and uses those values to run the Monte Carlo comparison.

The notebook assumptions include:

- manually defined scenario paths
- manually defined quarterly sales values
- scenario weights for calm, moderate, and intense cases
- a six-quarter simulation horizon

Because these inputs are manually defined, the output should be read as decision support rather than a validated revenue forecast.

## Reproducibility Caveat

The notebook does not set a fixed random seed. If the notebook is rerun, the exact Monte Carlo summary values may change slightly.

## Privacy and Scope

No private company data, internal NVIDIA data, customer-level data, or personal data is included in this repository.

The repository does not contain:

- raw operational data
- SQL database tables
- a data warehouse model
- a dashboard data source
- machine learning training data
- GenAI or LLM data inputs
