<p align="center">
  <img src="google-banner.svg" alt="Google Product Lifecycle & Innovation Analysis Banner" width="100%">
</p>

<h1 align="center">Google Product Lifecycle & Innovation Analysis</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas" alt="Pandas">
  <img src="https://img.shields.io/badge/Matplotlib-Visualization-orange" alt="Matplotlib">
  <img src="https://img.shields.io/badge/Seaborn-Statistical%20Plots-4c72b0" alt="Seaborn">
  <img src="https://img.shields.io/badge/Status-Completed-brightgreen" alt="Status">
  <img src="https://img.shields.io/badge/License-MIT-lightgrey" alt="License">
</p>

<p align="center">
  A quantitative study of product mortality, innovation strategy, and lifecycle trends at Google — powered by Python and Google Trends data.
</p>

---

## Overview

Google has launched — and quietly killed — hundreds of products over the past two decades. This project turns that graveyard into a dataset, applying exploratory data analysis and statistical visualization to uncover what patterns exist in how and when Google products die.

Using the [Killed by Google](https://killedbygoogle.com/) dataset alongside Google Trends, the analysis investigates product longevity by era, category, and macro tech trend alignment.

**Core questions explored:**
- Are modern Google products dying faster than older ones?
- Do certain years show spikes in shutdowns, hinting at strategic pivots?
- Which product categories have the best survival rates?
- Do public interest peaks (via Trends) correlate with launches or shutdowns?

---

## Key Findings

- **Lifespans are shrinking.** Products launched in the 2010s and beyond show shorter average lifespans than those from the early 2000s, suggesting faster iteration cycles or higher tolerance for failure.
- **Shutdown waves exist.** Certain years cluster with disproportionately high shutdowns, pointing to deliberate portfolio restructuring rather than organic attrition.
- **Category matters.** Infrastructure and developer tools outlive consumer-facing social products by a significant margin.
- **AI and cloud have legs.** Unlike previous tech waves, sustained public interest in AI and cloud computing shows no sign of the sharp drop-off seen in older categories.

---

## Tech Stack

| Layer | Libraries |
|---|---|
| Data manipulation | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn`, `joypy` |
| Trend data | `pytrends` |
| Dataset | Killed by Google (via `kagglehub`) |

---

## Project Structure
```
Google-Product-Analysis/
│
├── Google.ipynb       # Main analysis notebook
├── trends.csv         # Google Trends data
├── products.json      # Killed by Google product dataset
└── README.md
```

---

## Analyses

### Lifespan vs. Launch Year
Regression analysis examining whether products from different eras survive for meaningfully different durations, with a fitted trend line over scatter data.

### Density Mapping
Hexbin visualization to surface clustering — identifying whether short-lived products concentrate in specific launch windows or categories.

### Category Survival Distributions
Ridge plots (via Joypy) comparing lifespan distributions side-by-side across product categories, revealing where variance is highest.

### Shutdown Frequency Over Time
Bar chart breakdown of annual product shutdowns, highlighting years with abnormal spikes and their broader strategic context.

### Average Lifespan Trend
Grouped rolling analysis to observe how mean product survival has shifted decade-over-decade.

---

## Getting Started

**Clone the repository**
```bash
git clone https://github.com/Pynthamil/The-Hunger-Games-The-Google-Edition.git
cd The-Hunger-Games-The-Google-Edition
```

**Install dependencies**
```bash
pip install pandas numpy matplotlib seaborn joypy pytrends kagglehub
```

**Run the notebook**

Open `Google.ipynb` and run all cells sequentially. Trend data is fetched live via `pytrends`; an internet connection is required for that section.

---

## Skills Demonstrated

Exploratory Data Analysis · API Data Extraction · Statistical Visualization · Regression Analysis · Time Series Analysis · Data Cleaning & Transformation · Data-Driven Storytelling

---

## Roadmap

- [ ] Kaplan–Meier survival analysis for more rigorous longevity modeling
- [ ] ML-based lifespan prediction (launch era, category, competitive landscape)
- [ ] Interactive dashboard with Streamlit or Plotly
- [ ] Comparative analysis across Apple, Microsoft, and Meta product histories

---

## Author

**Pynthamil Pavendan**  
[github.com/Pynthamil](https://github.com/Pynthamil) · India

---

## License

MIT — see [LICENSE](LICENSE) for details.
