# Metal Commodity Trading Strategy

## Overview

This project investigates whether **price shocks in industrial metals** can predict equity returns of firms that produce those commodities.

The analysis combines econometric modelling with financial backtesting to evaluate whether commodity price movements contain predictive power for stock returns.

A **long–short trading strategy** is constructed based on the identified predictive relationships.

---

## Research Question

Do shocks in industrial metal prices predict future equity returns of companies producing those metals?

If so, can this information be used to construct a profitable investment strategy?

---

## Methodology

The project follows the following pipeline:

1. **Data Collection**

   * Metal prices and macro variables obtained from FRED
   * Equity data for commodity-producing firms

2. **Shock Identification**

   * Metal price shocks defined using rolling volatility thresholds

3. **Regression Analysis**

   * Predictive regressions testing whether lagged metal returns explain industry returns

4. **Strategy Construction**

   * Long/short portfolios based on positive or negative metal price shocks

5. **Backtesting**

   * Performance evaluated against the S&P 500 benchmark

The analysis is implemented entirely in **Python using Jupyter Notebook**.

---

## Repository Structure

```
metal-commodity-trading-strategy
│
├── notebooks
│   └── metals_strategy.ipynb
│
├── data
│   └── metals_data.zip
│
└── README.md
```

---

## Data

The dataset contains:

* Commodity prices (Copper, Aluminium, Zinc, Nickel, Oil)
* Equity returns of producing firms
* Inflation and term spread control variables

All datasets are provided in:

```
data/metals_data.zip
```

After downloading the repository, unzip the data folder before running the notebook.

---

## How to Run the Project

1. Clone the repository

```
git clone https://github.com/YOUR_USERNAME/metal-commodity-trading-strategy.git
```

2. Navigate into the folder

```
cd metal-commodity-trading-strategy
```

3. Unzip the data

```
data/metals_data.zip
```

4. Open the notebook

```
notebooks/metals_strategy.ipynb
```

Run all cells to reproduce the analysis.

---

## Python Libraries Used

Python
pandas
numpy
matplotlib
statsmodels
Jupyter Notebook

---

## Key Results

The analysis finds that **negative shocks in certain industrial metal prices have statistically significant predictive power for next-month returns of producing firms.**

Using this information, the constructed trading strategy outperforms the S&P 500 benchmark in cumulative returns, although with higher volatility.

---

## Author

Yadhu Soppin
Econometrics & Economics Student
Erasmus University Rotterdam

