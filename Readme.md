# Stock Market Performance Analysis

Comparing the performance and volatility of five large-cap stocks across
three sectors: tech (AAPL, MSFT, NVDA), financials (JPM), and consumer
staples (KO).

## Data
Daily prices for Oct 2025 to Oct 2026, stored in `data/`. Returns are
calculated from adjusted close prices, which account for dividends and splits.

## Methods
- Daily returns and cumulative returns
- Annualized volatility (daily standard deviation x √252)
- Return per unit of risk (total return / volatility)

Tools: Python, pandas, matplotlib, Jupyter

## Key Findings
| Stock | Total return | Annual volatility | Return per unit of risk |
|---|---|---|---|
| KO | 32.9% | 18.8% | 1.75 |
| AAPL | 29.8% | 24.7% | 1.21 |
| NVDA | 23.0% | 37.7% | 0.61 |
| JPM | 7.1% | 22.6% | 0.31 |
| MSFT | 0.6% | 32.8% | 0.02 |

- KO delivered the best return with the lowest volatility, making it the
  strongest risk-adjusted performer.
- NVDA was the most volatile stock, and the extra risk was not rewarded
  over this period.
- MSFT was nearly flat for the year despite high volatility.
- This covers only one year of data, so these are observations about the
  period, not predictions.

## Full Analysis
See [stock_analysis.ipynb](stock_analysis.ipynb) for the code, charts, and
tables.

## How to Run
pip install -r requirements.txt, then open the notebook in Jupyter.
