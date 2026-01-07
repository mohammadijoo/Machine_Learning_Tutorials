# EDA Report Draft — Chapter 3 Lesson 10

- Generated: 2026-01-07 18:47 UTC
- Datasets: ../../../Datasets/Regression/NYC_Collisions.csv, ../../../Datasets/Classification/Fast_Food_Restaurants_US.csv

## Executive Summaries

### NYC Collisions (sample)
(See notebook outputs in Sections 4, 5, 15.)

### Fast Food Restaurants (sample)
(See notebook outputs in Sections 6, 16.)

## Key Findings (draft)

# Key Findings (Draft)

## 1. Collisions concentrate in specific hours
- **Observation:** Highest collision volume occurs around hour 16 in this sample.
- **Evidence:** Hour-of-day bar chart; injury-rate heatmap (Section 15).
- **Implication:** Operational interventions can be targeted to peak windows.
- **Recommendation:** Create an injury-weighted peak-hour list and validate intervention impact via pre/post comparison.
- **Confidence:** Medium
- **Owner:** Analytics

## 2. Borough comparisons require missingness-aware reporting
- **Observation:** Geography fields have missingness; borough-level rates vary across groups in the sample.
- **Evidence:** Missingness table (Section 3) + borough injury-rate plot with intervals (Section 15).
- **Implication:** Naive borough ranking may be biased if missingness is systematic.
- **Recommendation:** Include an 'Unknown' group, test missingness mechanisms, and publish borough comparisons with uncertainty bars.
- **Confidence:** Low
- **Owner:** Analytics / Data Engineering

## 3. Location dataset needs canonicalization for reliable analytics
- **Observation:** Raw rows include duplicates and heterogeneous fields (categories/websites).
- **Evidence:** Duplicate key counts; domain distribution; taxonomy mapping coverage (Section 16).
- **Implication:** Unclean entities lead to inflated counts and unstable trends.
- **Recommendation:** Publish a canonical entity table with stable keys, dedupe rules, and versioned taxonomy mapping.
- **Confidence:** Medium
- **Owner:** Data Engineering


## Action plan
| Action | Owner | Expected impact | Validation | Impact (1-5) | Confidence (1-5) | Effort (1-5) | PriorityScore |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Investigate BOROUGH/ZIP missingness patterns; define reporting policy for unknown geography. | Analytics / Data Engineering | Reduce bias risk; improve interpretability of borough-level insights. | Missingness by time and by location proxies; sensitivity with/without unknown group. | 5 | 3 | 2 | 7.5 |
| Create injury severity buckets and track tail metrics (P90/P99) monthly. | Analytics | Better prioritization for high-severity risk windows. | Backtest stability and variance across months; monitor changes after interventions. | 4 | 4 | 2 | 8.0 |
| Deduplicate restaurant entities with spatial clustering + string normalization; publish canonical entity table. | Data Engineering | Prevent inflated counts and incorrect coverage estimates. | Manual audit of sampled clusters; measure false merges and missed duplicates. | 5 | 3 | 4 | 3.75 |
| Standardize restaurant categories using a controlled taxonomy + versioned mapping. | Data Engineering + Domain | Stable category analytics and comparable trends over time. | Coverage, drift monitoring, and periodic mapping review. | 4 | 3 | 3 | 4.0 |

## Assumptions
| Dataset | Assumption | Status | Verification |
| --- | --- | --- | --- |
| NYC Collisions | ACCIDENT_DATE/ACCIDENT_TIME reflect local time consistently. | Unclear | Check anomalies by hour/borough; look for DST artifacts. |
| NYC Collisions | BOROUGH/ZIP missingness is not systematically biased. | Unclear | Missingness by time and by location proxies (LAT/LON). |
| Fast Food | Rows can be resolved into unique physical locations. | Unclear | Spatial clustering + text matching; manual audit of ambiguous clusters. |
| Fast Food | Free-text categories can be mapped to a stable taxonomy. | Likely | Build mapping; measure coverage and drift. |
