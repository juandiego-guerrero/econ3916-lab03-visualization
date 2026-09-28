# econ3916-lab03-visualization
Lab 03 Submission
# Honest vs. Misleading Visualizations

## Objective
An applied study of how design choices in data visualization, including axis scaling, deflation, framing, and summary statistics, can distort or clarify economic evidence, paired with quantitative tools for measuring and correcting that distortion.

## Methodology
- **Summary statistics vs. structure:** Reconstructed Anscombe's Quartet, four datasets with near-identical means, variances, correlations, and fitted regression lines, and visualized each to show where summary statistics fail to capture underlying relationships.
- **Quantifying distortion:** Computed Tufte's Lie Factor (the ratio of the effect size shown in a graphic to the effect size in the data) for a truncated-axis revenue chart, then rebuilt the chart with a zero baseline and proportional encoding.
- **Framing real wage data:** Retrieved FRED series AHETPI (Average Hourly Earnings of Production and Nonsupervisory Employees, Total Private), deflated it to constant 2020 dollars, and produced four versions of the same series that varied the design choices (time window, baseline, and nominal vs. real framing) to show how each supports a different narrative.
- **Structured exploratory data analysis:** Applied a four-step EDA framework (structure, distributions, relationships, anomalies) to World Bank GDP data covering [N] countries over [N] years.
- **Interactive diagnostics:** Built an interactive chart toggler that switches between honest and misleading renderings while reporting the Lie Factor live.

## Key Findings
- Identical summary statistics can hide very different data-generating patterns (linear, nonlinear, outlier-driven, and leverage-driven). Visual inspection is a necessary complement to numerical summaries.
- The truncated-axis revenue chart had a Lie Factor of 3.2, meaning it exaggerated the underlying change by more than threefold. A zero-baseline redesign brought the visual effect back in line with the data.
- The same real earnings series could credibly support four different conclusions depending on presentation. Deflating to constant dollars and making framing choices explicit are essential to honest wage analysis.
- The structured EDA process surfaced data-quality issues and distributional features in the GDP panel before any modeling, which reinforced EDA as a safeguard against misleading downstream inference.
- Making distortion measurable (the live Lie Factor) turns visualization integrity from a stylistic judgment into a checkable standard.
