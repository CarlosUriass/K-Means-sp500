# The Tribes of Wall Street: Clustering the S&P 500 with Machine Learning

A practical data science project that transforms the complexity of 500 stocks into a strategic visual map of risk and return profiles using Python and clustering techniques.

---

## Project Overview

Analyzing the S&P 500 can be overwhelming due to its sheer size and diversity. Traditionally, stocks are grouped by sectors, but this often fails to capture their true behavioral similarities in terms of risk and return.

This project uses machine learning to group stocks based on their **financial DNA** — a set of carefully selected metrics that capture performance, risk, and risk-adjusted quality — to uncover distinct “investment tribes” within the market.

---

## Key Features

- **Data Collection & Processing:** Extracts 15 years of historical price data for each stock.
- **Financial DNA Metrics:** Calculates 8 key metrics for each stock:
  - Total Return
  - Compound Annual Growth Rate (CAGR)
  - Volatility
  - Maximum Drawdown
  - Downside Deviation
  - Sharpe Ratio
  - Sortino Ratio
  - Calmar Ratio
- **Dimensionality Reduction:** Uses PCA to visualize relationships between metrics.
- **Clustering:** Applies K-Means clustering to segment stocks into groups with similar financial behavior.
- **Analysis & Visualization:** Profiles each cluster’s characteristics and visualizes them with radar charts and scatterplots.

---

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/CarlosUriass/K-Means-sp500
   cd K-Means-sp500
   ```

2. Create a virtual environment and install dependencies:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

---

## Usage

Run the Jupyter notebook to execute the full pipeline:

```bash
jupyter main.ipynb
```

The notebook will:

- Download the stocks data from yahoo finance API
- Calculate financial metrics for each stock.
- Detect and remove outliers.
- Perform PCA for dimensionality reduction.
- Find the optimal number of clusters using K-Means and statistical scores.
- Segment stocks into clusters.
- Visualize and analyze cluster profiles.

---

## Results

The project segments the S\&P 500 into 4 distinct investment tribes, each with unique risk-return profiles. This allows investors to build diversified portfolios with a deeper understanding of stock behavior beyond traditional sector classifications.

---

## Limitations & Future Work

- Relies on historical price data — future market conditions may differ.
- Cluster composition depends on selected financial metrics; adding fundamental data (P/E, ROE, etc.) could enrich insights.
- Future enhancements could include sector analysis within clusters and tracking cluster transitions over economic cycles.

---

## License

This project is licensed under the MIT License.

---

## Contact

For questions or feedback, contact [Carlos Urias](mailto:hicarlosurias@gmail.com).

---

**Transforming data into strategic investment insights with Machine Learning.**
