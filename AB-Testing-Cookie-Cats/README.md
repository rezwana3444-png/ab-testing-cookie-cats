# A/B Testing: Cookie Cats Mobile Game Gate Placement

## Overview
An A/B testing analysis examining whether moving a progression gate from level 30 to 
level 40 in the mobile game Cookie Cats affects player retention, using data from 
90,189 real players.

## Business Question
Does moving the gate from level 30 to level 40 help or hurt player retention?

## Method
- **Chi-Square test** to compare retention rates (categorical outcome) between the 
  control (gate_30) and test (gate_40) groups
- Tested both 1-day and 7-day retention to check for short vs long-term effects

## Key Findings
- **1-Day Retention:** No statistically significant difference (p = 0.0755)
- **7-Day Retention:** Statistically significant difference (p = 0.0016) — gate_30 
  retains slightly more players (19.0%) than gate_40 (18.2%)

## Recommendation
Keep the gate at level 30. The move to level 40 shows a small but statistically 
significant negative effect on long-term retention, with no meaningful benefit to 
offset it.

## Tools Used
Python (pandas, scipy, seaborn, matplotlib) — Chi-Square hypothesis testing

## Files
- `AB_Testing_Cookie_Cats.ipynb` — full analysis notebook with narrative, tests, and visualizations
