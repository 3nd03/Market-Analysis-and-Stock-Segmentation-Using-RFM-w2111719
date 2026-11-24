Market Analysis and Stock Segmentation Using RFM - 6BUIS017W, Oscar Denche, w2111719 - Coursework 1

## Overview
This project segments S&P 500 shares from 2021 to 2024 in two ways: by risk and return (mean weekly return and weekly beta) and by trading activity using an adapted RFM model (Recency, Frequency, Monetary). The two feature sets are clustered with Ward agglomerative clustering and K-means.

## How to run
Open the notebook in Colab and select Runtime > Run all:
https://colab.research.google.com/github/3nd03/Market-Analysis-and-Stock-Segmentation-Using-RFM-w2111719/blob/main/Market_Analysis_and_Stock_Segmentation_Using_RFM.ipynb

The first cell clones this repository and loads the saved data snapshots, so no new download is needed.

## Data snapshots (retrieved 2026-11-21)
- `data/sp500_2026-11-21.csv`: ticker list
- `data/sp500_prices_2026-11-21.csv.gz`: daily prices and volume
- `data/sp500_exclusions_2026-11-21.csv`: excluded tickers and reasons
- `data/features_2026-11-21.csv`: one row per share (mean return, beta, R, F, M)
- `data/clusters_2026-11-21.csv`: cluster assignments for each solution

## Figures
`figures/` contains the dendrograms, elbow plot, cluster plots and sector composition chart.

## Requirements
See `requirements.txt` (pandas 2.2.3, yfinance 0.2.66, scikit-learn 1.6.1).

## Reproducibility
Yahoo Finance data can be revised, so results are produced from the saved snapshots rather than a new download. K-means uses random_state = 158. The RFM observation date is 2024-12-31.
