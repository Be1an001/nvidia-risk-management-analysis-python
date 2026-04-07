# Scripts

## Main Notebook

- [`01_nvidia_risk_analysis.ipynb`](01_nvidia_risk_analysis.ipynb)

This notebook is the main code file in the public GitHub version of this project.

It is meant to show the parts of the project that are most useful for public review:

- an earlier scenario comparison stage
- updated Monte Carlo simulation
- updated CDF-style comparison
- the later three-path scenario comparison used in the final public-facing result

## Why I Used a Notebook Here

For GitHub, I kept the code in notebook form because it is easier to review step by step.

This also fits the project better than a long script file, since the public version is meant to be more readable for recruiters, interviewers, and GitHub visitors.

## Scope of the Notebook

The notebook is focused on the main analysis logic behind the public version of the project.

It mainly reproduces the simulation portion of the project.

The risk register, scoring setup, and heat map are preserved through the archive working files and selected visuals, rather than rebuilt step by step in notebook code.

It also keeps an earlier comparison stage and a later updated three-path scenario stage in the same file. The later updated stage is the main public-facing result used in the final repo story.

It does not try to recreate every document or every manually designed diagram from the original course submission.

The influence diagram and scenario tree are kept as exported visuals in:

- [`../outputs/figures/latest-influence-diagram.png`](../outputs/figures/latest-influence-diagram.png)
- [`../outputs/figures/updated-scenario-tree.png`](../outputs/figures/updated-scenario-tree.png)

## Reproducibility Note

The simulation values and probabilities in the notebook are manually defined project assumptions.

The notebook does not set a fixed random seed, so reruns may vary slightly.

## Related Files

- [Project walkthrough](../walkthrough/project-walkthrough.md)
- [Final report](../reports/aly6130-final-report.pdf)
- [Final slides](../slides/aly6130-module-6-briefing.pdf)
- [Data note](../data/README.md)

## Environment Note

Main packages used in the notebook:

- numpy
- pandas
- matplotlib
- notebook / jupyter
