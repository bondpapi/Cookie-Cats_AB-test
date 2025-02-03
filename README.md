# Cookie Cats A/B Test

## Overview

This repository contains the analysis of the Cookie Cats A/B test, which investigates the impact of moving the in-game gate from level 30 to level 40 on player retention and engagement.

## Dataset

The dataset contains these key columns:



- `userid`: Unique player identifier.

- `version`: The A/B test group (gate_30 or gate_40).

- `sum_gamerounds`: Total game rounds played within the first 14 days.

- `retention_1`: Whether the player returned one day after installation.

- `retention_7`: Whether the player returned seven days after installation.

## Methodology

1. **Exploratory Data Analysis (EDA)**
    - Data cleaning and summary statistics.

    - Visualizations of player engagement and retention rates.

2. **Sample Ratio Mismatch (SRM) Test**
    - Conducted a chi-square test to verify sample balance.

3. **Statistical Analysis**
    - Used a t-test to compare game rounds played.

    - Used a Z-test to compare Day 1 and Day 7 retention.

4. **Confidence Interval Computation**
    - Calculated both analytical and bootstrap confidence intervals for Day 7 retention.

5. **Decision & Recommendations**
    - Based on retention impact, we determined whether moving the gate was beneficial.

## Results & Findings

- **No significant impact** on *Day 1 retention.*

- **Significant difference** in *Day 7 retention*, suggesting an effect on long-term engagement.

- Further investigation into player behavior beyond 7 days is recommended.