# USDT vs USDC: Supply, Growth and Peg Stability in Numbers

A short data project comparing the two biggest stablecoins, USDT (Tether) and USDC (Circle), from a cross-border payments perspective. Built in Python on Google Colab using free, public data from DefiLlama.

## Why this project

Cross-border payments in traditional banking run on SWIFT and correspondent banks, with limits on settlement time and cost. More and more fintechs now use stablecoins to move money across borders, with USDT and USDC at the centre. This project compares the two on three things: **supply, growth and peg stability.**

![Stablecoin payment flow](charts/stablecoin_payment_flow.png)

## Key findings

| Measure | USDT | USDC |
| --- | --- | --- |
| Total supply | $176.8B | $70.6B |
| Number of chains | 131 | 161 |
| Main chain | Tron | Ethereum |
| Main chain share | 52.1% | 60.8% |
| Growth since Jan 2021 | 8.8x | 18x |
| Average gap from $1 | 0.088% | 0.077% |
| Worst gap from $1 | 1.14% | 3.89% |

- **Supply:** USDT is about 2.5 times bigger. Tron and Ethereum together hold 90.3% of all USDT, while USDC is centred on Ethereum and spread across newer chains.
- **Growth:** USDC has grown faster since 2021, about 18 times against 8.8 times for USDT.
- **Peg stability:** both hold $1 very well day to day, but USDC's worst depeg (March 2023, after the Silicon Valley Bank collapse) was more than three times deeper than USDT's worst.

## Charts

| | |
| --- | --- |
| ![Supply by chain](charts/chart1_supply_by_chain.png) | ![Share by chain](charts/chart2_share_by_chain.png) |
| ![Supply over time](charts/chart3_supply_over_time.png) | ![Peg stability](charts/chart4_peg_stability.png) |

## How to run

1. Open `usdt_vs_usdc_analysis.ipynb` in [Google Colab](https://colab.research.google.com) or Jupyter.
2. Run the cells from top to bottom. No API keys or accounts are needed.
3. The charts are saved as PNG files in the working folder.

To run it locally: `pip install -r requirements.txt`, then open the notebook in Jupyter.

## Data

All data comes from the free [DefiLlama stablecoins API](https://defillama.com/stablecoins): current supply by chain, daily supply history and daily prices, from January 2021 to November 2026.

## Limitations

- Supply on a chain shows where money sits, not how much is sent.
- Daily prices hide intraday drops, so the worst depegs were likely deeper.
- Transfer costs (network fees, on- and off-ramp) are not covered.

## Article

Read the full write-up on Medium: [USDT vs USDC: Supply, Growth and Peg Stability in Numbers](https://medium.com/@timelexx1watch/usdt-vs-usdc-supply-growth-and-peg-stability-in-numbers-5d718fdb193e)

## Author

**Abolarin Oladimeji**: cross-border payments professional in Nigeria, with a diploma in data science.

*This project is analysis, not financial advice.*
