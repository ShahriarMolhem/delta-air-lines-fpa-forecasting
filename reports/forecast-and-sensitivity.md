# Three-Year Driver-Based FP&A Scenario | Delta Air Lines

**Author:** Shahriar Molhem · Undergraduate BBA Finance · University of Georgia  
**Historical base:** FY2025 consolidated GAAP statements. **Modeled:** FY2026–FY2028 *hypothetical student what-if cases*, not Delta internal budget or issuer guidance.

## Model structure and assumptions

Passenger revenue is modeled from capacity in **available seat miles (ASM)** and implied passenger revenue per ASM. Fuel expense combines modeled gallons (capacity plus efficiency changes) and modeled unit expense; labor and a simplified other-expense residual use modeled cost per ASM. Cargo and other revenue have independent growth assumptions.

| Assumed driver | FY2026 | FY2027 | FY2028 |
| --- | ---: | ---: | ---: |
| ASM growth | 3.0% | 3.0% | 2.8% |
| Passenger revenue/ASM growth | 0.5% | 1.0% | 1.0% |
| Cargo revenue growth | 3.0% | 3.0% | 3.0% |
| Other revenue growth | 4.0% | 4.0% | 4.0% |
| Fuel usage efficiency improvement, gal/ASM | 0.5% | 0.5% | 0.5% |
| Implied fuel expense/gallon change | 0.0% | 2.0% | 2.0% |
| Labor unit cost inflation | 3.0% | 3.0% | 3.0% |
| Other nonfuel/nonlabor unit cost inflation | 2.0% | 2.0% | 2.0% |

The source 2025 fuel unit expense is calculated as **reported GAAP fuel cost divided by reported fuel gallons**, rather than using Delta's rounded, published price/gallon.

## Scenario outcomes (USD millions)

| Metric | FY2025 actual | FY2026 hypothetical | FY2027 hypothetical | FY2028 hypothetical |
| --- | ---: | ---: | ---: | ---: |
| Consolidated operating revenue | 63,364 | 65,638 | 68,271 | 70,896 |
| Fuel | 9,819 | 10,063 | 10,519 | 10,975 |
| Salaries and related costs | 17,520 | 18,587 | 19,719 | 20,879 |
| Other nonfuel/nonlabor costs | 30,203 | 31,731 | 33,337 | 34,956 |
| Consolidated operating expenses | 57,542 | 60,381 | 63,575 | 66,810 |
| **Operating income** | **5,822** | **5,257** | **4,696** | **4,086** |
| Operating margin | 9.2% | 8.0% | 6.9% | 5.8% |

Under this **cost-pressure stress case**, revenue grows, but assumed unit-cost increases outweigh modeled passenger yield improvements. These results do *not* state what Delta will actually earn.

## FY2026 what-if sensitivity: operating income (USD millions)

The workbook varies passenger yield by **±4%** and modeled fuel unit expense by **±20%**; all other assumptions remain unchanged.

| Fuel price change ↓ / Passenger yield change → | −4% | −2% | 0% | +2% | +4% |
| --- | ---: | ---: | ---: | ---: | ---: |
| −20% | 5,126 | 6,198 | 7,270 | 8,342 | 9,413 |
| −10% | 4,120 | 5,192 | 6,264 | 7,335 | 8,407 |
| **0%** | **3,114** | **4,185** | **5,257** | **6,329** | **7,401** |
| +10% | 2,107 | 3,179 | 4,251 | 5,323 | 6,394 |
| +20% | 1,101 | 2,173 | 3,245 | 4,316 | 5,388 |

Formula: `scenario EBIT = base EBIT + passenger revenue × yield shock − fuel expense × fuel-unit-cost shock`.

The center cell returns **$5,257m**, matching the unshocked model. A 10% rise in modeled unit fuel expense lowers EBIT by roughly **$1.006bn**, all else constant. A 1% modeled change in passenger yield changes EBIT by about **$536m**.

**Excel companion workbook:** `models/delta_air_lines_fpa_model.xlsx`. The workbook has already been prepared and checked, but the binary **has not yet been uploaded** to this repository. Do not describe this Markdown reconstruction as the Excel file itself.

## Critical limitations

1. FY2021 has pandemic recovery effects and recognized grants; do not extrapolate directly.
2. The simplified residual cost category includes non-airline businesses and does not literally scale with ASM in reality.
3. Fuel price and passenger yield shocks do not model ticket-price demand elasticity, hedging, refinery effects or labor contract dynamics.
4. Other revenue and CASM-Ex reflect different concepts; non-GAAP CASM-Ex is *not* this model's GAAP residual.
5. FY2026 outcomes are presented as scenarios constructed using FY2025 disclosures, not real FY2026 operating results or management guidance.

**Sources:** [Delta 2025 Form 10-K](https://www.sec.gov/Archives/edgar/data/27904/000002790426000013/dal-20251231.htm); [reported historical GAAP inputs](../data/historical-gaap.csv); [operating statistics](../data/operating-statistics.csv).
