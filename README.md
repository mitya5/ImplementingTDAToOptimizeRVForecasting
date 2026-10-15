# Implementing Topological Data Analysis to Optimize Forecasting of Short-Horizon Volatility in High-Frequency Cryptocurrency Markets

**Matt Koffman**, Department of Mathematics, University of Chicago

📄 **[Read the paper (PDF)](ImplementingTDA.pdf)**

*Preprint, October 2026. Written as part of the University of Chicago Mathematics REU.*

## Abstract

This paper builds upon the novel introduction of Topological Data Analysis as a feature in machine learning models used to trade equities. Specifically, we aim to improve upon current industry-standard realized-volatility models within high-frequency cryptocurrency markets. We do this by adding various topological features derived from persistent homology, in an aim to improve forecasting performance during volatile periods. Using one-minute BTC/USDT and ETH/USDT data spanning 2020–2023, we embed rolling windows of returns as point clouds, compute persistence diagrams, and extract twelve topological summary features that augment both a linear (HAR-RV) and a nonlinear (XGBoost) benchmark. We identify and correct for a frequency confound: because topological features are computed on finer-frequency returns than the baseline models observe, part of their apparent benefit is attributable to frequency information rather than topology itself. After controlling for this with a ladder of robust one-minute volatility estimators, we find that the naive six-to-fourteen percent reduction in QLIKE loss shrinks by roughly half, but a statistically decisive residual gain of 3.2 to 5.9 percent survives (Diebold–Mariano statistics between 7.6 and 9.9). This residual gain concentrates in turbulent regimes and nonlinear models, and is carried in part by a scale-invariant topological feature. We therefore provide evidence that persistent homology contributes genuine, non-redundant information for forecasting realized volatility in high-frequency cryptocurrency markets during turbulent periods, provided the frequency confound is properly controlled.

## Key results

| | BTC/USDT | ETH/USDT |
|---|---|---|
| Naive QLIKE reduction from topological features | 6.1–6.9% | 7.2–14.1% |
| QLIKE reduction after robust volatility controls | 3.25–3.30% | 3.9–5.9% |
| Diebold–Mariano statistic (controlled comparison) | 8.9–9.9 | 7.6–7.8 |


## Citation

```bibtex
@misc{koffman2026tda,
  title  = {Implementing Topological Data Analysis to Optimize Forecasting of
            Short-Horizon Volatility in High Frequency Cryptocurrency Markets},
  author = {Koffman, Matt},
  year   = {2026},
  note   = {Preprint},
  url    = {https://github.com/USERNAME/REPO}
}
```

## Acknowledgments

Thanks to my mentor, Sofia Sampaio Lacerda, and to the University of Chicago Mathematics REU, J. Peter May, and its organizers.

## Contact

mkoffman5@uchicago.edu
