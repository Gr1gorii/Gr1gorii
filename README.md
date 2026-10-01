[English](README.md) | [Italiano](README.it.md)

# Hryhorii Klymenko

**Junior Data / AI · Python & SQL**

I'm focused on data analysis and applied AI: turning raw data into clear findings, dashboards and carefully evaluated prototypes. Open to junior opportunities in data analytics and applied AI.

[LinkedIn](https://www.linkedin.com/in/hryhorii-klymenko/) · [Devpost](https://devpost.com/GKL1) · [X](https://x.com/HKL1ne)

## Selected projects

### 1. [Hotel Booking Analytics](https://github.com/Gr1gorii/hotel-booking-analytics)

**How do booking patterns and cancellations vary across hotels and channels?**

Python · pandas · SQLite · scikit-learn · Streamlit

- Analysis of **119,390 historical bookings**, with reproducible data preparation, SQL summaries and an interactive dashboard
- Time-ordered ML evaluation, feature-availability checks, baseline comparisons and error analysis
- **Finding:** 41.7% of bookings were canceled at the city hotel, compared with 27.8% at the resort. These are observed differences, not causal effects
- The cancellation model stays an **offline experiment**: its small ranking improvement comes with many false alarms

[Repository & local demo](https://github.com/Gr1gorii/hotel-booking-analytics) · [Business findings](https://github.com/Gr1gorii/hotel-booking-analytics/blob/main/reports/management_brief.md) · [Model evaluation](https://github.com/Gr1gorii/hotel-booking-analytics/blob/main/reports/model_results.md)

<a href="https://github.com/Gr1gorii/hotel-booking-analytics">
  <img src="https://raw.githubusercontent.com/Gr1gorii/hotel-booking-analytics/main/docs/images/overview.jpg" alt="Hotel dashboard showing booking totals, cancellation rates and monthly trends" width="760">
</a>

### 2. [Customer Repeat Purchase Analysis](https://github.com/Gr1gorii/customer-repeat-purchase-analysis)

**Which customers buy again, and how does purchase activity change by cohort?**

Python · SQL · DuckDB · pandas

- Pipeline for **541,909 UCI Online Retail source lines**, with documented quality rules and SQL results reconciled against pandas
- Cohort analysis and 30/60/90-day repeat-purchase windows with complete-observation denominators
- **Finding:** 907 of 4,070 eligible customers (**22.3%**) bought on another invoice within 30 days. This is historical purchase activity, not measured business uplift

[Repository & local demo](https://github.com/Gr1gorii/customer-repeat-purchase-analysis) · [Findings](https://github.com/Gr1gorii/customer-repeat-purchase-analysis/blob/main/reports/management_summary.md) · [Repeat-purchase SQL](https://github.com/Gr1gorii/customer-repeat-purchase-analysis/blob/main/sql/02_repeat.sql)

<details>
<summary>Preview the cohort chart</summary>

![Actual customer cohort activity chart; grey cells mark incomplete observation](https://raw.githubusercontent.com/Gr1gorii/customer-repeat-purchase-analysis/main/reports/cohort-activity.png)

</details>

### 3. [Document Search RAG](https://github.com/Gr1gorii/document-search-rag)

**Can a local assistant answer questions about documentation and make its sources easy to inspect?**

Python · FastAPI · BM25 · Ollama

- Search and local RAG over **12 FastAPI documentation pages**, with source excerpts, citation links and abstention
- Search-only fallback when the local model is unavailable; no paid API required
- Published checks for retrieval, citations, abstention and latency, including failure cases. Keyword matches and valid citation IDs **do not establish factual accuracy**

[Repository & local demo](https://github.com/Gr1gorii/document-search-rag) · [Evaluation & limitations](https://github.com/Gr1gorii/document-search-rag/blob/main/reports/QUALITY.md)

<details>
<summary>Preview an answer and its source</summary>

![Actual local RAG answer with the cited FastAPI source excerpt expanded](https://raw.githubusercontent.com/Gr1gorii/document-search-rag/main/reports/ui-answer.png)

</details>

## Tools used in these projects

**Data:** Python, SQL, pandas, DuckDB, SQLite  
**ML & AI:** scikit-learn, model evaluation, BM25 retrieval, Ollama  
**Delivery:** Streamlit, FastAPI, Git, pytest, reproducible local workflows

## More projects

[TON Tracker](https://github.com/Gr1gorii/ton-tracker) · [HeatRelay](https://github.com/Gr1gorii/HeatRelay) · [All repositories](https://github.com/Gr1gorii?tab=repositories)

## Project scope

These are portfolio and learning projects. Source references, runnable code, checks and limitations are available in the repositories.
