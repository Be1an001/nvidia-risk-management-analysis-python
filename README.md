# NVIDIA Risk Management Analysis

Portfolio version of my ALY6130 final project on NVIDIA risk management using risk scoring, heat maps, scenario modeling, and Monte Carlo analysis.

## Project Overview

This repository is the public portfolio version of my final project for **ALY6130: Risk Management for Analytics**.

I used NVIDIA as the case company and studied how major business risks can be identified, prioritized, visualized, and translated into action plans. The project started from risk identification and a six-risk register, then moved to heat maps, scenario modeling, and a Monte Carlo summary for six-quarter sales impact.

I cleaned this repo up for GitHub, but I still kept the main report, the final slides, selected figures, one notebook, and a small archive of original project files.

## Business Problem

NVIDIA has strong growth in GPUs and AI, but it also faces major business risks. In this project, the biggest ones were supply chain dependence on TSMC and geopolitical tensions around U.S.-China relations and Taiwan.

The main question was:

**How can NVIDIA prioritize and manage its most important risks in a practical way that protects revenue and operations over the next six quarters?**

## What I Did

This was an **individual course project**.

My work in this project included:

- reviewing public company and industry sources
- building the risk register
- scoring and prioritizing six risks
- creating heat map visuals
- organizing the influence diagram and scenario tree logic
- summarizing the six-quarter risk impact with Monte Carlo analysis
- writing the final report and briefing materials

## Project Scope

This project covers:

- risk identification
- qualitative risk analysis
- risk scoring and prioritization
- risk register design
- heat map visualization
- influence diagram
- scenario tree
- Monte Carlo simulation summary
- KRI and response planning
- continuous risk management communication

## Final Risk Focus

The final version used six risks:

1. Supply Chain Disruptions  
2. Export Restrictions  
3. Strong Competition  
4. Geopolitical Tensions  
5. Emergence of Cost-Effective AI Models  
6. Market Valuation Volatility  

The two highest-priority risks in the final version were:

- **Supply Chain Disruptions**
- **Geopolitical Tensions**

## Final Takeaways

My main takeaways from the final version were:

- Supply chain and geopolitical risks were the most serious risks in the final scoring.
- The risk register and heat map helped narrow the focus to the top two risks.
- The updated scenario model showed three final paths: regulatory compliance, manufacturing delays, and trade restrictions.
- Trade restrictions showed the biggest downside risk in the final Monte Carlo/CDF comparison.
- The final project was not only about analysis. It also included KRI design, mitigation ideas, contingency planning, and communication flow.

## Data Note

This project does **not** use a large raw tabular dataset like a typical analytics project.

Instead, the project used:

- public company filings
- public business and news sources
- manually structured risk scores
- small working Excel files
- manually defined scenario assumptions
- simulated revenue outputs

Please see [data/README.md](data/README.md) for details.

## Repository Guide

- [Project walkthrough](walkthrough/project-walkthrough.md)
- [Final report](reports/aly6130-final-report.pdf)
- [Final briefing slides](slides/aly6130-module-6-briefing.pdf)
- [Notebook](scripts/01_nvidia_risk_analysis.ipynb)
- [Script note](scripts/README.md)
- [Outputs note](outputs/README.md)

## Selected Visuals

### Risk calculation and risk register

![Risk calculation sheet](outputs/figures/nvidia-risk-calculation-sheet.png)

![Risk register](outputs/figures/nvidia-risk-register.png)

### Risk heat map

![Risk heat map](outputs/figures/nvidia-risks-heat-map-1-9-scale.png)

### Influence diagram and scenario tree

![Influence diagram](outputs/figures/latest-influence-diagram.png)

![Scenario tree](outputs/figures/updated-scenario-tree.png)

### Monte Carlo and CDF

![Monte Carlo and CDF](outputs/figures/updated-cumulative-distribution-function.png)

## Repo Structure

```text
nvidia-risk-management-analysis-python/
├─ README.md
├─ .gitignore
├─ requirements.txt
├─ data/
│  └─ README.md
├─ scripts/
│  ├─ 01_nvidia_risk_analysis.ipynb
│  └─ README.md
├─ walkthrough/
│  └─ project-walkthrough.md
├─ outputs/
│  ├─ README.md
│  └─ figures/
│     ├─ nvidia-risk-calculation-sheet.png
│     ├─ nvidia-risk-register.png
│     ├─ nvidia-risks-heat-map-1-9-scale.png
│     ├─ latest-influence-diagram.png
│     ├─ updated-cumulative-distribution-function.png
│     └─ updated-scenario-tree.png
├─ reports/
│  └─ aly6130-final-report.pdf
├─ slides/
│  └─ aly6130-module-6-briefing.pdf
└─ archive/
   ├─ nvidia-risk-treatment-and-response-plan-original.docx
   ├─ aly6130-nvidia-risk-portfolio-v1.pdf
   ├─ nvidia-risk-calculation-sheet-original.xlsx
   └─ nvidia-risk-register-original.xlsx
```

## Archive Note

The `archive/` folder keeps a small set of original working files that support this project:

- original risk treatment and response plan
- an earlier portfolio PDF version
- the original risk calculation sheet
- the original risk register

I kept these files to preserve some project history, but the main GitHub story is still centered on the final report, final briefing, selected figures, and the notebook.

## Resume-Friendly Summary

Scenario-based risk management project on NVIDIA using risk scoring, heat maps, scenario modeling, and Monte Carlo analysis to study supply chain and geopolitical risk impact.