# NVIDIA Risk Management Analysis

This repository is the public portfolio version of my individual final project for **ALY6130: Risk Management for Analytics**.

The project analyzes NVIDIA as a business risk case. The goal was to identify major risks, prioritize them with a simple scoring framework, and use scenario-based simulation to support mitigation and monitoring decisions.

This is best understood as a risk analytics and decision-support case study. It is not a machine learning project, a production forecasting system, a dashboard app, or a real NVIDIA consulting engagement.

## Project Type and Tools

- Project type: risk analytics / decision-support case study
- Status: coursework project cleaned for portfolio review
- Main tools: Python, Jupyter notebook, NumPy, pandas, matplotlib, Excel
- Main artifacts: final report, briefing slides, archived risk workbooks, selected figures, and one notebook

## Business Problem

NVIDIA has strong growth in GPUs and AI, but the company also faces risks that could affect operations and revenue. This case study focuses on risks related to semiconductor supply chains, U.S.-China and Taiwan geopolitical tension, export restrictions, competition, lower-cost AI models, and market valuation volatility.

The main question was:

**How can NVIDIA prioritize its most important business risks and connect the top risks to practical mitigation and monitoring actions?**

## Project Objective

The objective was to move from a broad list of business risks to a clearer decision-support view:

- identify major NVIDIA risk themes
- build a six-risk register
- score risks using chance and impact
- visualize priorities with a heat map
- model geopolitical risk paths with an influence diagram and scenario tree
- compare manually defined scenario outcomes with Monte Carlo simulation
- connect the findings to KRIs, treatment plans, and communication steps

## Data and Assumptions

This project does not use a large raw operational dataset. It is based on public company and industry sources, manually structured risk scores, archived Excel workbooks, and manually defined scenario assumptions.

The notebook does not read a CSV file or database table. Instead, it defines scenario values directly in code and simulates six-quarter sales outcomes under the project assumptions.

Important notes:

- The NVIDIA 2024 annual report was used as a company baseline source.
- Risk scores were manually structured in the archived workbooks.
- Scenario probabilities and sales values were manually defined for this course project.
- The simulation does not set a fixed random seed, so reruns can vary slightly.
- The results should be read as decision support, not as a validated NVIDIA revenue forecast.

See [data/README.md](data/README.md) for more detail.

## My Role / Contribution

This was an individual course-based project. My work included reviewing public sources, building the risk register, scoring and prioritizing risks, creating supporting visuals, organizing scenario logic, using Python for the Monte Carlo comparison, and preparing the final report and briefing materials.

## Methodology

The project followed a risk management workflow:

1. Identify major risks from public company and industry context.
2. Build a six-risk register with causes, impacts, mitigation notes, owners, and status.
3. Score each risk using chance and impact.
4. Use a heat map to identify the highest-priority risks.
5. Focus the later scenario analysis on geopolitical tension and supply chain exposure.
6. Build an influence diagram and scenario tree for decision paths.
7. Run a Monte Carlo simulation for six-quarter scenario outcomes.
8. Use histograms, CDF comparison, and summary statistics to compare relative downside exposure.
9. Translate the analysis into KRIs, mitigation ideas, contingency actions, and communication planning.

## Key Findings

- The final risk register contains six major risks: supply chain disruptions, export restrictions, strong competition, geopolitical tensions, cost-effective AI models, and market valuation volatility.
- The final scoring identifies geopolitical tensions and supply chain disruptions as the two highest-priority risks.
- The heat map helps show why those two risks deserve the most attention in the project.
- The scenario model compares regulatory compliance, manufacturing delays, and trade restrictions.
- Under the project assumptions, trade restrictions show the clearest downside risk in the Monte Carlo and CDF comparison.
- The practical response focuses on supplier diversification, non-Taiwan capacity, export-policy monitoring, and KRI-based escalation.

These findings should be interpreted carefully because the scenario inputs are manually defined assumptions, not validated operating forecasts.

## Visual Highlights

The selected figures below summarize the main project story. They are curated project visuals; not every figure is regenerated directly from the notebook.

### Risk register

The risk register organizes the six risks, scores, priorities, mitigation ideas, owners, and status.

![Risk register](outputs/figures/nvidia-risk-register.png)

### Risk heat map

The heat map summarizes manually scored risk priorities using chance and impact scores.

![Risk heat map](outputs/figures/nvidia-risks-heat-map-1-9-scale.png)

### Scenario tree

The scenario tree shows how the project translated geopolitical tension into decision paths and scenario assumptions.

![Scenario tree](outputs/figures/updated-scenario-tree.png)

### Monte Carlo and CDF comparison

The CDF comparison shows relative scenario outcomes under the project assumptions, not a validated forecast.

![Monte Carlo and CDF](outputs/figures/updated-cumulative-distribution-function.png)

## How to Review This Project

This repository is best reviewed as a case study, not as a fully automated data pipeline.

A good review order is:

1. Read the [project walkthrough](walkthrough/project-walkthrough.md) for the full project flow.
2. Review the [final report](reports/aly6130-final-report.pdf) for the complete course deliverable.
3. Open the [notebook](scripts/01_nvidia_risk_analysis.ipynb) to inspect the Monte Carlo and CDF logic.
4. Check the archived workbooks for the original risk register and scoring setup.
5. Review the selected visuals in [outputs/figures](outputs/figures).

## Reproducibility Notes

The notebook can be reviewed and rerun with the packages listed in [requirements.txt](requirements.txt), but the project is only partially reproducible because several inputs are manually defined.

```bash
pip install -r requirements.txt
jupyter notebook scripts/01_nvidia_risk_analysis.ipynb
```

Reproducibility caveats:

- The notebook uses manually entered scenario assumptions.
- The simulation does not set a fixed random seed.
- The risk register, scoring setup, influence diagram, and scenario tree are preserved through archived files and selected figures rather than rebuilt entirely in notebook code.
- The exported report, slides, and archive files are part of the project evidence but are not regenerated by a script.

## Repository Structure

```text
nvidia-risk-management-analysis-python/
|-- README.md
|-- requirements.txt
|-- data/
|   `-- README.md
|-- scripts/
|   |-- 01_nvidia_risk_analysis.ipynb
|   `-- README.md
|-- walkthrough/
|   `-- project-walkthrough.md
|-- outputs/
|   |-- README.md
|   `-- figures/
|       |-- nvidia-risk-calculation-sheet.png
|       |-- nvidia-risk-register.png
|       |-- nvidia-risks-heat-map-1-9-scale.png
|       |-- latest-influence-diagram.png
|       |-- updated-scenario-tree.png
|       `-- updated-cumulative-distribution-function.png
|-- reports/
|   `-- aly6130-final-report.pdf
|-- slides/
|   `-- aly6130-module-6-briefing.pdf
`-- archive/
    |-- nvidia-risk-treatment-and-response-plan-original.docx
    |-- aly6130-nvidia-risk-portfolio-v1.pdf
    |-- nvidia-risk-calculation-sheet-original.xlsx
    `-- nvidia-risk-register-original.xlsx
```

## Limitations

- This is a course-based case study, not a real NVIDIA engagement.
- The project does not use private NVIDIA data or raw operational data.
- Scenario probabilities and sales assumptions are manually defined.
- The Monte Carlo output supports relative scenario comparison, not validated financial forecasting.
- The notebook does not set a fixed random seed.
- There is no SQL database, BI dashboard, Streamlit app, machine learning model, GenAI component, MLOps workflow, or production deployment in this repository.
- Some archived materials preserve earlier course work, so the final repository story should be read from the README, walkthrough, final report, notebook, and selected figures together.
- Some supporting artifacts come from different course stages, so exact scores or scenario values should be checked against the final report, archived workbooks, and notebook before reuse.

## Future Improvements

- Add a clearer assumption table for scenario probabilities and sales values.
- Set a fixed random seed in the notebook for easier result comparison.
- Separate the earlier scenario comparison and final three-path comparison more clearly.
- Add sensitivity analysis to show how results change when scenario probabilities change.
- Clean up dense visuals for easier GitHub viewing.
- Add a short source-to-assumption mapping for the risk scores and scenario values.

## Related Files

- [Project walkthrough](walkthrough/project-walkthrough.md)
- [Data and assumption notes](data/README.md)
- [Notebook notes](scripts/README.md)
- [Outputs notes](outputs/README.md)
- [Main notebook](scripts/01_nvidia_risk_analysis.ipynb)
- [Final report](reports/aly6130-final-report.pdf)
- [Final briefing slides](slides/aly6130-module-6-briefing.pdf)
- [Original risk calculation sheet](archive/nvidia-risk-calculation-sheet-original.xlsx)
- [Original risk register](archive/nvidia-risk-register-original.xlsx)
- [Original treatment and response plan](archive/nvidia-risk-treatment-and-response-plan-original.docx)
- [Portfolio PDF v1](archive/aly6130-nvidia-risk-portfolio-v1.pdf)
- [Selected figures](outputs/figures)
- [Requirements file](requirements.txt)
