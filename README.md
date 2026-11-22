# Data Analytics Portfolio

I’m Ahmad Ahmouda, an Applied Mathematics master’s student at Kaunas
University of Technology with a background in aviation engineering.
I use SQL and Python to combine datasets, test hypotheses, and explain
what the results mean for a decision.

[LinkedIn](https://www.linkedin.com/in/ahmad-ahmouda/)

## Featured projects

### What drives bad marketplace reviews? · DuckDB SQL + Python

I joined nine Olist e-commerce tables into a dataset of **95,824 delivered,
reviewed orders**, with one row per order. I used SQL to resolve duplicate
reviews and aggregate items and payments, then used Python to compare
review rates and fit a logistic regression.

**54.1% of late orders received a 1- or 2-star review, compared with 9.2%
of on-time orders.** Among orders that arrived on time, the bad-review
rate was **46.9% for multi-seller orders versus 8.7% for single-seller
orders**. That gives marketplace teams a specific group of orders to
investigate beyond late deliveries.

[Read the report](olist-bad-reviews/olist_bad_reviews.pdf) ·
[Open the SQL and Python notebook](olist-bad-reviews/olist_bad_reviews_analysis.ipynb)

### What is associated with depression scores in international students? · PostgreSQL

I cleaned and analyzed **263 survey records** from a university in Japan.
I used PostgreSQL to compare student groups, calculate correlations, and
examine differences across quartiles.

Among international students, **social connectedness had a correlation
of −0.546 with PHQ-9 scores**. Average scores were **12.00 in the
least-connected quartile and 4.57 in the most-connected quartile**.
These are associations from a single survey.

[Read the report](student-mental-health-sql/students_mental_health.pdf) ·
[Open the SQL notebook](student-mental-health-sql/students_mental_health_sql.ipynb)

## More projects

| Project | What I worked on |
|---|---|
| [Automotive recommender](automotive-recommender/) | Compared popularity and personalized recommenders using ranking metrics and catalog coverage. |
| [Credit risk modeling](credit-risk-modeling/) | Compared default prediction models and used dynamic programming to construct FICO score bands. |
| [Natural gas pricing](natural-gas-pricing/) | Estimated prices between observed dates and modeled the cash flows of a storage contract. |
| [Employee attrition explainability](employee-attrition-explainability/) | Examined how classification thresholds affect errors and used LIME and SHAP to explain individual predictions. |
| [Building energy regression](building-energy-regression/) | Checked a regression pipeline on simulated hourly energy use and corrected its RMSE calculation. |
| [Human activity classification](human-activity-classification/) | Compared tree-based models for classifying activity from sensor features. |
| [Landsat-style classification](landsat-classification/) | Compared logistic regression and linear discriminant analysis on simulated satellite features. |
| [Vehicle tracking](vehicle-tracking-kalman-filter/) | Evaluated Kalman filters under different noise assumptions and during a simulated sensor outage. |
