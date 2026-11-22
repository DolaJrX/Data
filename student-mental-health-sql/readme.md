# International Students' Mental Health: A SQL Analysis

**Student survey analysis | PostgreSQL**

Are international students more likely to report depression symptoms? And how do social connectedness, cultural adjustment stress, and length of stay relate to their scores? I explored these questions using a 2018 university student survey from Japan.

## Dataset and approach

- **Source:** 2018 student survey at a university in Japan.
- **Sample:** 263 cleaned records: 197 international students and 66 domestic students.
- **Data preparation:** Excluded 18 invalid or summary rows and removed five exact duplicate records from the original 286 rows.
- **Analysis:** Used PostgreSQL to compare groups, calculate correlations, examine quartiles, and compute test statistics.

Depression symptoms were measured using the **PHQ-9 score**. Social connectedness and acculturative stress were examined using their respective survey scores. These measures are not clinical diagnoses.

## Key findings

- **Social connectedness:** Among international students, the correlation with PHQ-9 was **r = −0.546**. Average PHQ-9 was 12.00 in the least-connected quartile and 4.57 in the most-connected quartile.
- **Acculturative stress:** The correlation with PHQ-9 was **r = 0.411**. International students also reported higher average stress scores than domestic students (75.47 vs 63.14).
- **Depression scores by student group:** International and domestic students had similar average PHQ-9 scores (8.02 vs 8.61); the difference was **not statistically significant**.
- **Length of stay:** Its correlation with PHQ-9 was close to zero (**r = 0.069**), with no statistically significant difference found in the longer-stay comparison.

These findings show **relationships, not cause and effect**. The survey covers one university at one point in time, and some subgroups are small.

## SQL skills demonstrated

PostgreSQL · data cleaning · CTEs · `SELECT DISTINCT` · `FILTER` · `CASE` · `NTILE()` · window functions · `CORR()` · `PERCENTILE_CONT()` · `GROUPING SETS` · `ROLLUP` · statistical summaries.


