# Spread Locator: A Statistical Distribution Analysis Model

## 🎯 Project Overview
This repository contains an end-to-end statistical distribution analysis of e-commerce customer transaction behaviors. By leveraging parametric fitting, goodness-of-fit evaluations, and statistical transformations, this project models daily transaction volumes and purchase amounts to support data-driven business decisions.

## 📁 Repository Structure
- `notebooks/statistical_distribution_analysis.ipynb`: Executable Jupyter Notebook containing all Python steps and visualizations.
- `docs/Spread_Locator_Statistical_Distribution_Analysis_Report.pdf`: Comprehensive theoretical guide and analytical findings.
- `data/spread_locator_dataset.csv`: Dataset containing transaction amounts, customer IDs, and regions.

## 🔬 Key Statistical Findings
- **Data Skewness:** Transaction amounts exhibit strong positive skewness (+3.76) and high kurtosis (25.95), invalidating direct Gaussian assumptions.
- **Optimal Distribution:** The **Log-Normal distribution** demonstrated an outstanding fit ($p = 0.8999$ on the Kolmogorov-Smirnov test), accurately capturing multiplicative purchasing behaviors.
- **Variance Stabilization:** A Box-Cox transformation with $\lambda = -0.1808$ normalized the data (Shapiro-Wilk $p = 0.6419$).
- **Success Rate:** The Bernoulli success probability is $p = 0.4455$, indicating significant payment drop-off at checkout.
- **Daily Volume:** Daily order arrivals follow a Poisson distribution with $\lambda \approx 7.10$ orders/day.

## 🚀 Quickstart
```bash
git clone [https://github.com/](https://github.com/)<your-username>/spread-locator-distribution-model.git
cd spread-locator-distribution-model
pip install -r requirements.txt
jupyter notebook notebooks/statistical_distribution_analysis.ipynb