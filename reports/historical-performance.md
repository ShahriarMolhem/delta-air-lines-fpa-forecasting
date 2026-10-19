# Delta Air Lines — Historical Financial Performance (FY2021–FY2025)

**Research:** Independent undergraduate FP&A portfolio case study. All USD values are in **millions**, unless otherwise specified.

## Selected GAAP statement metrics

| Metric (USD m) | FY2021 | FY2022 | FY2023 | FY2024 | FY2025 |
| --- | ---: | ---: | ---: | ---: | ---: |
| Operating revenue | 29,899 | 50,582 | 58,048 | 61,643 | 63,364 |
| Operating expenses | 28,013 | 46,921 | 52,527 | 55,648 | 57,542 |
| Operating income | 1,886 | 3,661 | 5,521 | 5,995 | 5,822 |
| Operating margin | 6.3% | 7.2% | 9.5% | 9.7% | 9.2% |
| Aircraft fuel and related taxes | 5,633 | 11,482 | 11,069 | 10,566 | 9,819 |
| Salaries and related costs | 9,728 | 11,902 | 14,607 | 16,161 | 17,520 |

**FY2025:** Delta reported $63.364bn in operating revenue (+2.8% vs FY2024), yet GAAP operating income was $5.822bn (down $173m or 2.9%). This demonstrates why FP&A must consider both revenue and cost drivers, without claiming historical accounting changes prove causal relationships.

## FY2024–FY2025 GAAP operating-income bridge

The following contributions reconcile the change in operating income **exactly**:

| Driver | Change in EBIT (USD m) |
| --- | ---: |
| FY2024 reported operating income | **5,995** |
| Passenger revenue change | +874 |
| Cargo revenue change | +78 |
| Other revenue change | +769 |
| Salaries and related costs change | −1,359 |
| Aircraft fuel and related taxes change | +747 |
| All remaining operating expense changes, net | −1,282 |
| **FY2025 reported operating income** | **5,822** |

The $1,282m category combines all cost categories *other than salaries and aircraft fuel*. This is an **arithmetic variance bridge** rather than evidence of managerial cause. Other revenue includes refinery and ancillary operations.

## Price/volume decomposition of fuel expense

In FY2024 Delta reported 4,114m gallons consumed and $10,566m of fuel and related taxes; in FY2025, 4,269m gallons and $9,819m. Fuel volume rose, but total expenses fell.

Use **implied expense per gallon** from actual financial-statement total ÷ reported volume, not the rounded disclosed price per gallon:

```text
P24 = 10,566 / 4,114 ($/gallon, implied)
P25 =  9,819 / 4,269 ($/gallon, implied)
Price effect = (P25 − P24) × 4,114
Volume effect = (4,269 − 4,114) × P25
Price effect + Volume effect = −747 (USD millions)
```

This identity is sensitive to the expense/volume definition and is **not a causal fuel-market analysis** or a standalone assessment of refinery economics.

## Special-year limitations

- FY2021 was a pandemic-recovery year. Reported GAAP expenses included **negative $4,512m government grant recognition**, so raw ratios should not be treated as steady-state cost expectations.
- FY2023 included a separately reported pilot agreement and related expense ($864m).
- Published **CASM-Ex** is a non-GAAP operational KPI and is **not** identical to this project's GAAP operating-expense residual.
- The prospective FY2026–FY2028 model will be **student-selected hypothetical assumptions**, not an actual budget or management guidance.

## Reproducibility
- [Source-linked GAAP dataset](../data/historical-gaap.csv)
- [Source-linked aviation operating statistics](../data/operating-statistics.csv)
- [Validation record](../quality/validation.md)
- [SEC FY2025 Form 10-K](https://www.sec.gov/Archives/edgar/data/27904/000002790426000013/dal-20251231.htm) and [FY2023 Form 10-K](https://www.sec.gov/Archives/edgar/data/27904/000002790424000003/dal-20231231.htm)

**Interpretation:** Revenue growth alone did not ensure operating-profit growth in FY2025. An FP&A model should explicitly track capacity, revenue per capacity unit, fuel inputs and labor unit costs, while retaining limitations on operational causality.
