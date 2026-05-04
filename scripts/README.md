# Scripts

This folder contains the main notebook used in the public GitHub version of the project.

## Main Notebook

- [01_nvidia_risk_analysis.ipynb](01_nvidia_risk_analysis.ipynb)

The notebook focuses on the simulation part of the risk analysis. It does not rebuild the full course project from scratch.

## What the Notebook Covers

The notebook includes:

- an earlier two-path scenario comparison
- an updated three-path scenario comparison
- Monte Carlo simulation logic
- histogram and CDF visualization
- summary statistics for simulated six-quarter sales outcomes

The later three-path comparison is the main public-facing simulation result for the repository. It compares:

- Regulatory Compliance
- Manufacturing Delays
- Trade Restrictions

## What the Notebook Does Not Cover

The notebook does not recreate every part of the original project. Several important project components are preserved through reports, archived files, and selected figures instead.

The notebook does not fully rebuild:

- the original risk register
- the chance-impact scoring workbook
- the heat map creation process
- the influence diagram design process
- the scenario tree design process
- the final report or briefing slides

Those materials are available elsewhere in the repository.

## Assumption and Simulation Notes

The simulation values and probabilities are manually defined project assumptions. The result should be interpreted as a scenario-based comparison, not as a validated forecast of NVIDIA revenue.

The notebook uses:

- 10,000 simulation runs
- a six-quarter horizon
- manually defined scenario values
- NumPy random sampling

The notebook does not set a fixed random seed, so reruns may produce slightly different summary values.

## Environment Notes

The notebook uses the packages listed in the repository-level [requirements.txt](../requirements.txt):

- numpy
- pandas
- matplotlib
- jupyter

To review or rerun the notebook locally:

```bash
pip install -r ../requirements.txt
jupyter notebook 01_nvidia_risk_analysis.ipynb
```

Run the commands from inside the `scripts/` folder, or adjust the path if running from the repository root.

## Related Files

- [Project walkthrough](../walkthrough/project-walkthrough.md)
- [Data and assumption notes](../data/README.md)
- [Outputs notes](../outputs/README.md)
- [Final report](../reports/aly6130-final-report.pdf)
- [Final slides](../slides/aly6130-module-6-briefing.pdf)
- [Influence diagram](../outputs/figures/latest-influence-diagram.png)
- [Scenario tree](../outputs/figures/updated-scenario-tree.png)
- [Monte Carlo and CDF figure](../outputs/figures/updated-cumulative-distribution-function.png)
