# Project Walkthrough

This walkthrough explains the flow of the NVIDIA risk management case study from business framing to scenario-based simulation and response planning.

## Project Overview

This project was my individual final project for **ALY6130: Risk Management for Analytics**. I used NVIDIA as the case company and built a structured risk analytics workflow around one main question:

**How can NVIDIA identify, prioritize, and respond to major business risks in a practical way?**

The GitHub version keeps the final report, briefing slides, selected figures, one notebook, and archived working files that support the project story.

Main files:

- [Final report](../reports/aly6130-final-report.pdf)
- [Final briefing slides](../slides/aly6130-module-6-briefing.pdf)
- [Notebook](../scripts/01_nvidia_risk_analysis.ipynb)
- [Data note](../data/README.md)
- [Outputs note](../outputs/README.md)

## Business Problem

NVIDIA is a useful risk analytics case because its growth depends on AI demand, GPU leadership, and semiconductor supply chains. At the same time, the company faces risks that could affect production, sales, or investor confidence.

The project considered six major risk themes:

- supply chain disruptions
- export restrictions
- strong competition
- geopolitical tensions
- emergence of cost-effective AI models
- market valuation volatility

The analysis focused most on supply chain disruptions and geopolitical tensions because they were identified as the highest-priority risks in the final scoring.

## Data and Assumptions

This project is not built around a raw transaction dataset. The main inputs were:

- public company filings and business sources
- manually built risk scores
- archived Excel workbooks
- manually defined scenario assumptions
- simulated six-quarter sales outputs

The working files are preserved in the archive folder:

- [Risk calculation sheet](../archive/nvidia-risk-calculation-sheet-original.xlsx)
- [Risk register](../archive/nvidia-risk-register-original.xlsx)
- [Treatment and response plan](../archive/nvidia-risk-treatment-and-response-plan-original.docx)

The notebook defines scenario values directly in code. These assumptions are useful for decision-support comparison, but they should not be treated as a validated revenue forecast.

## Workflow

The project followed this workflow:

1. Identify major NVIDIA business risks.
2. Build a six-risk register.
3. Score risks by chance and impact.
4. Use a heat map to narrow the focus.
5. Build an influence diagram and scenario tree.
6. Simulate six-quarter scenario outcomes with Monte Carlo analysis.
7. Compare scenario distributions with histograms and CDF curves.
8. Translate the results into mitigation, KRI, contingency, and communication planning.

## Risk Register and Scoring

The final project used six risks:

1. Supply Chain Disruptions
2. Export Restrictions
3. Strong Competition
4. Geopolitical Tensions
5. Emergence of Cost-Effective AI Models
6. Market Valuation Volatility

The final scoring identified two high-priority risks:

- Geopolitical Tensions
- Supply Chain Disruptions

The risk register and scoring details are mainly preserved through the archived workbooks and selected figures.

![Risk calculation sheet](../outputs/figures/nvidia-risk-calculation-sheet.png)

![Risk register](../outputs/figures/nvidia-risk-register.png)

## Heat Map

The heat map visualizes the chance and impact scores for the six risks. It helps show why the project narrowed attention to supply chain and geopolitical exposure.

![Heat map](../outputs/figures/nvidia-risks-heat-map-1-9-scale.png)

## Influence Diagram and Scenario Tree

After the scoring step, the later analysis focused on geopolitical tension as the main scenario case. The influence diagram connects geopolitical instability to trade restrictions, manufacturing delays, supply chain disruptions, and sales impact.

![Influence diagram](../outputs/figures/latest-influence-diagram.png)

The scenario tree translates that logic into three scenario paths:

- Regulatory Compliance
- Manufacturing Delays
- Trade Restrictions

![Scenario tree](../outputs/figures/updated-scenario-tree.png)

## Notebook and Simulation Logic

The notebook is:

- [01_nvidia_risk_analysis.ipynb](../scripts/01_nvidia_risk_analysis.ipynb)

The notebook focuses on the simulation portion of the project. It includes an earlier comparison stage and a later three-path comparison. The later three-path comparison is the main public-facing simulation result.

The simulation uses:

- 10,000 runs
- six-quarter total sales outcomes
- manually defined scenario values
- scenario weights of 0.25, 0.50, and 0.25 for the calm, moderate, and intense cases

The notebook does not set a fixed random seed, so reruns can produce slightly different results.

## Monte Carlo and CDF Result

The final simulation compares:

- Regulatory Compliance
- Manufacturing Delays
- Trade Restrictions

The result is best read as a relative scenario comparison. The CDF output suggests that trade restrictions have the clearest downside risk under the project assumptions. Regulatory compliance appears narrower and more stable, while manufacturing delays show more spread.

This does not mean the project predicts NVIDIA's actual future revenue. It shows how the project assumptions behave in a simple simulation.

![Monte Carlo and CDF](../outputs/figures/updated-cumulative-distribution-function.png)

## Business Interpretation

The main project interpretation is that risk scoring can help narrow a broad list of business risks into a smaller set of priorities. For this case, supply chain disruptions and geopolitical tensions became the most important risks to monitor.

The scenario analysis then connects those risks to practical planning ideas:

- diversify suppliers
- invest in more stable manufacturing locations
- monitor export policy changes
- define KRI thresholds for escalation
- keep medium-priority risks under review

## Limitations

- This is a course-based case study, not a real NVIDIA engagement.
- The project does not use private NVIDIA data or raw operational data.
- Scenario probabilities and sales values are manually defined.
- The Monte Carlo results support decision-support comparison, not validated forecasting.
- The notebook does not set a fixed random seed.
- The repository does not contain a dashboard app, SQL pipeline, machine learning model, GenAI component, MLOps workflow, or production deployment.
- Some archived materials preserve earlier project versions, so the final story should be read across the README, final report, notebook, and selected figures.
- Some supporting artifacts come from different course stages, so exact scores or scenario values should be checked against the final report, archived workbooks, and notebook before reuse.

## Related Materials

- [README](../README.md)
- [Data note](../data/README.md)
- [Script note](../scripts/README.md)
- [Outputs note](../outputs/README.md)
- [Final report](../reports/aly6130-final-report.pdf)
- [Final slides](../slides/aly6130-module-6-briefing.pdf)
- [Notebook](../scripts/01_nvidia_risk_analysis.ipynb)
- [Archive folder](../archive)
