[English](README.md) | [Italiano](README.it.md)

# Hryhorii Klymenko

**Data Analyst / Junior Data Scientist · Retail, e-commerce & hospitality analytics**

MSc in Computer Science. I build analyses that end in a business decision: what to stock, whom to contact, what a customer is worth and whether a discount is real. Python and SQL, with time-based validation and confidence intervals rather than single-number claims.

Open to junior data roles in Italy and remote (EU). Fully authorised to work in Italy; no visa or relocation assistance required.

[LinkedIn](https://www.linkedin.com/in/hryhorii-klymenko/) · [Devpost](https://devpost.com/GKL1) · [X](https://x.com/HKL1ne)

## Currently building

### [Are Black Friday discounts real? Italy 2026](https://github.com/Gr1gorii/price-tracker)

Under the EU Omnibus directive, an announced discount must be calculated from the lowest price of the previous 30 days. I track **~1,800 products in 5 Italian online shops twice a day** to test whether Black Friday discounts (27 Nov 2026) follow that rule.

- Scheduled collector: robots.txt-aware, rate-limited, Parquet + DuckDB storage, twice-daily runs
- Compliance checker: true 30-day low, claimed vs honest discount, flags for inflated reference prices and price increases just before a discount
- **Results: early December 2026**

Python · httpx · DuckDB · pandas · GitHub Actions · pytest

## Selected projects

### 1. [Retail Demand Planner](https://github.com/Gr1gorii/retail-demand-planner)

**Which forecast gives a grocery store the cheapest weekly replenishment?**

- Daily forecasts for **1,437 food items** (Walmart M5) across four chronological windows: LightGBM vs seasonal naive and a 28-day moving average
- Forecasts turned into a weekly order policy with a two-day lead time and safety stock calibrated on validation data only
- **Result:** LightGBM has the lowest simulated inventory cost, **20.8% below seasonal naive**, and is the cheapest in all four windows and all nine cost scenarios

Python · LightGBM · pandas · Streamlit (EN/IT)

<a href="https://github.com/Gr1gorii/retail-demand-planner">
  <img src="https://raw.githubusercontent.com/Gr1gorii/retail-demand-planner/main/assets/en/overview.png" alt="Simulated inventory cost by forecasting method and savings by window" width="760">
</a>

### 2. [Email Campaign Uplift](https://github.com/Gr1gorii/discount-uplift)

**Is it more profitable to email only the customers the campaign actually persuades?**

- Randomized Hillstrom email experiment, **42,613 customers**: email lifts conversion by **0.68 pp** (95% CI 0.50–0.86)
- Uplift model, incremental profit by targeting policy, bootstrap intervals and sensitivity to contact cost and coupon size
- **Result:** targeting the top 30% is not significantly more profitable than mailing everyone (−$66 per 10,000 customers, 95% CI −$989 to $804), so I recommend a new randomized pilot before rollout

Python · scikit-learn · bootstrap · Streamlit (EN/IT)

<details>
<summary>Preview: profit by targeting policy</summary>

![Incremental profit and bootstrap intervals by targeting policy](https://raw.githubusercontent.com/Gr1gorii/discount-uplift/main/reports/policy_profit.png)

</details>

### 3. [Customer Lifetime Value & Segmentation](https://github.com/Gr1gorii/ecommerce-clv-segmentation)

**What is each customer worth over the next year, and what should we do with each segment?**

- BG/NBD + Gamma-Gamma model on UK transactions from Online Retail II, backtested on three time windows against two baselines
- The model beats both baselines on top-10% and top-20% revenue capture in all three windows; I use it to rank customers, not to forecast exact revenue
- **Result:** CAC reference ranges and an action for each segment, including a costed reactivation test for 104 high-value dormant customers

Python · lifetimes · pandas · Streamlit (EN/IT)

<details>
<summary>Preview: portfolio dashboard</summary>

![Streamlit dashboard with segment contribution and customer value distribution](https://raw.githubusercontent.com/Gr1gorii/ecommerce-clv-segmentation/main/reports/figures/en/dashboard.jpg)

</details>

### 4. [Hotel Booking Analytics](https://github.com/Gr1gorii/hotel-booking-analytics)

**Where do hotel cancellations come from, and can late ones be predicted?**

- **119,390 bookings** analysed with SQL views, an interactive dashboard and a management brief
- **Finding:** 41.7% of bookings canceled at the city hotel vs 27.8% at the resort; the cancellation rate is 57.0% for bookings made more than 180 days ahead vs 9.6% at 0–7 days
- Late-cancellation model with time-based validation and a feature-leakage audit; kept offline because its small gain comes with many false alarms

Python · SQL (SQLite) · scikit-learn · Streamlit

<details>
<summary>Preview: booking dashboard</summary>

![Hotel dashboard with booking totals, cancellation rates and monthly trends](https://raw.githubusercontent.com/Gr1gorii/hotel-booking-analytics/main/docs/images/overview.jpg)

</details>

### 5. [Document Search RAG](https://github.com/Gr1gorii/document-search-rag)

**Can a small local model answer documentation questions with sources you can check?**

- Local RAG (BM25 + Ollama) over 12 FastAPI documentation pages, with citations and abstention when evidence is missing
- Expected page among the top four results for 45/45 answerable questions; abstained on 15/15 out-of-scope questions; failure cases documented

Python · FastAPI · BM25 · Ollama

## Skills

**Analytics:** Python, pandas, SQL (DuckDB, SQLite), Streamlit dashboards  
**Statistics & ML:** A/B tests and uplift, bootstrap intervals, demand forecasting (LightGBM), CLV models, scikit-learn, time-based validation  
**Data engineering:** web data collection, Parquet, scheduled pipelines (GitHub Actions), pytest  
**AI:** local RAG and evaluation of model answers

## More projects

[Customer Repeat Purchase Analysis](https://github.com/Gr1gorii/customer-repeat-purchase-analysis) · [Processing Efficiency Study](https://github.com/Gr1gorii/processing-efficiency-study) · [TON Tracker](https://github.com/Gr1gorii/ton-tracker) · [HeatRelay](https://github.com/Gr1gorii/HeatRelay) · [All repositories](https://github.com/Gr1gorii?tab=repositories)

Portfolio projects on public data. Each repository documents its sources, checks and limitations.

## Project code license

Copyright (c) 2026 Gr1gorii.

The original project code authored by Gr1gorii is licensed under the
GNU General Public License version 3 only (`GPL-3.0-only`).
See [LICENSE](LICENSE) for the full terms.

Third-party code, datasets, and materials retain their respective licenses
and attribution requirements. This license does not replace those terms.
