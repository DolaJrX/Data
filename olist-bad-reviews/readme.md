# What Makes Customers Leave Bad Reviews?

**Customer review analysis | SQL (DuckDB) + Python**

Why do some marketplace orders receive 1- or 2-star reviews? I used the Olist Brazilian E-Commerce dataset to examine delivery delays, order structure, sellers, and other factors associated with poor ratings.

## Dataset and approach

- **Source:** Olist Brazilian E-Commerce dataset, Brazil (2016–2018).
- **Sample:** 95,824 delivered, reviewed orders from nine source tables.
- **SQL:** Checked data quality, resolved duplicate reviews, aggregated item and payment records, and joined the tables into one row per order using CTEs and window functions.
- **Python:** Compared review rates, examined patterns by delivery timing and sellers, ran a chi-square test, and fitted a logistic regression model.

A bad review means **1 or 2 stars**. An order is late when it arrives after its estimated delivery date.

## Key findings

- **Late deliveries:** 54.1% of late orders received bad reviews, compared with 9.2% of on-time orders.
- **Multi-seller orders:** Even among on-time orders, the bad-review rate was 46.9% for orders involving two or more sellers, versus 8.7% for single-seller orders.
- **Seller performance:** 29 higher-risk sellers accounted for 6.5% of all bad reviews while handling 2.5% of orders.
- **Predictive model:** The logistic regression achieved a test-set ROC AUC of **0.725**.

These are **associations, not proven causes**. The data does not include parcel-level delivery times or a full analysis of written review comments.

## Tools and techniques

`DuckDB` · `SQL` · `Python` · `pandas` · `matplotlib` · `SciPy` · `statsmodels` · `scikit-learn`

SQL joins, CTEs, `ROW_NUMBER()`, order-level aggregation, data cleaning, exploratory analysis, statistical testing, and logistic regression.

## Project report and code

**[Read the complete analysis and code (PDF)](olist_bad_reviews_complete.pdf)**

The PDF contains the redesigned report, figures, conclusions, and a technical appendix with the complete SQL and Python code cells. To run the code separately, download the nine Olist CSV files and place them in a local `data/` folder as described in the appendix.
