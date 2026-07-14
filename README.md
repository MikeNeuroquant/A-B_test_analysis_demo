# Marketing A/B Test — Conversion Analysis

A/B test analysis on the Kaggle marketing dataset (`faviovaz/marketing-ab-testing`). Users are split between an `ad` treatment and a `psa` control; the analysis quantifies the lift in conversion rate and checks how exposure volume and timing affect it.

## Project structure

```
marketing-ab-test/
├── README.md
├── insights.md
├── requirements.txt
└── notebooks/
    └── ab_test_analysis.ipynb
```

The dataset is pulled at runtime via `kagglehub`, so no local copy is needed.

## Requirements

- Python 3.10+
- R 4.x with packages: `emmeans`, `car`, `dplyr` (used inside the notebook via `rpy2`)
- Kaggle account credentials configured for `kagglehub`

Install Python dependencies:

```bash
pip install -r requirements.txt
```

R packages (from an R session):

```r
install.packages(c("emmeans", "car", "dplyr"))
```
