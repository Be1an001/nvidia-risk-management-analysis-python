# Outputs

This folder contains selected visuals from the public portfolio version of the NVIDIA risk management project.

The figures summarize the main project flow:

- risk scoring and prioritization
- risk register structure
- heat map visualization
- geopolitical risk scenario logic
- Monte Carlo and CDF comparison

These are curated project visuals. They should not be read as a claim that every figure is regenerated directly from the notebook.

## Figure List

### Risk calculation sheet

- [figures/nvidia-risk-calculation-sheet.png](figures/nvidia-risk-calculation-sheet.png)

This figure shows the chance-impact scoring setup and the manually scored risk values.

### Risk register

- [figures/nvidia-risk-register.png](figures/nvidia-risk-register.png)

This figure shows the six-risk register with risk causes, consequences, scores, priorities, mitigation notes, owners, and status.

### Risk heat map

- [figures/nvidia-risks-heat-map-1-9-scale.png](figures/nvidia-risks-heat-map-1-9-scale.png)

This figure visualizes risk priority using chance and impact scores. It supports the focus on supply chain disruptions and geopolitical tensions.

### Influence diagram

- [figures/latest-influence-diagram.png](figures/latest-influence-diagram.png)

This figure shows how geopolitical tension connects to trade restrictions, manufacturing delays, supply chain disruptions, and sales impact.

### Scenario tree

- [figures/updated-scenario-tree.png](figures/updated-scenario-tree.png)

This figure shows the scenario paths and manually defined sales assumptions used in the later project stage.

### Monte Carlo and CDF comparison

- [figures/updated-cumulative-distribution-function.png](figures/updated-cumulative-distribution-function.png)

This figure compares simulated six-quarter outcomes for the three scenario paths. It should be interpreted as a decision-support comparison under project assumptions, not as a validated revenue forecast.

## Notes

- The visuals are meant to help readers understand the project before reading the full report.
- Some visuals are exported project artifacts rather than notebook-generated outputs.
- The Monte Carlo and CDF visual is the main quantitative output figure.
- Dense spreadsheet screenshots are included as evidence, but the heat map, scenario tree, and CDF figure are usually easier to review quickly.

## Related Files

- [Project README](../README.md)
- [Project walkthrough](../walkthrough/project-walkthrough.md)
- [Main notebook](../scripts/01_nvidia_risk_analysis.ipynb)
- [Final report](../reports/aly6130-final-report.pdf)
- [Final slides](../slides/aly6130-module-6-briefing.pdf)
