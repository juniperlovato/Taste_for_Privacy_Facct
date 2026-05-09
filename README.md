# Taste for Privacy — Replication Code

This repository contains the analysis code for:

> Lovato, J., Hébert-Dufresne, L., Ghasemizade, M., St-Onge, J., Dodds, P. S., Bloomfield, L., Fudolig, M. I., Price, M., & Danforth, C. (2026). **Taste for Privacy: How Context, Identity, and Lived-Experience Shape Information Sharing Preferences.** *The 2026 ACM Conference on Fairness, Accountability, and Transparency (FAccT '26)*, June 25–28, 2026, Montreal, QC, Canada. https://doi.org/10.1145/3805689.3812311

A preprint is available at: https://arxiv.org/abs/2604.22025

---

## Repository Structure

| File | Figures | Description |
|------|---------|-------------|
| `01_privacy_settings_social_media.py` | Figure 1 | Descriptive statistics for social media privacy settings (public/mixed/private), platform usage, and social media use frequency. Includes an ordered logit model predicting privacy settings from comfort sharing data with platforms, and stacked bar charts of Likert-scale responses by privacy setting group. |
| `02_taste_for_privacy_by_institution.py` | Figure 3 | Ranks 17 data-sharing contexts (e.g. government, employer, stranger) by mean discomfort using bootstrap resampling. Produces violin plots and confidence interval plots of institution rankings across the full sample. |
| `03_institutions_and_demographics.py` | Figures 4–7 | Examines how privacy preferences across institutions vary by demographics (gender, ACE score, etc.). Uses bootstrap mean-difference tests and rank-difference comparisons to identify which groups show significantly higher discomfort with specific data-sharing contexts. |
| `04_circle_plots.py` | Figures 2, 8–13 | Circular bar chart ("circles of trust") visualizations showing the distribution of Likert responses across institutions for the full sample and broken out by demographic subgroups (e.g. men, women). |

---

## Data

The scripts expect a CSV file at the path specified in each script's data-loading cell (`pd.read_csv('filepath.csv')`). Update this path to point to your local copy of the dataset before running.

---

## Dependencies

```
numpy
pandas
matplotlib
seaborn
statsmodels
```

Install with:

```bash
pip install numpy pandas matplotlib seaborn statsmodels
```

---

## License

This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).  
© 2026 The Authors. Published by ACM. ISBN 979-8-4007-2596-8/2026/06.
