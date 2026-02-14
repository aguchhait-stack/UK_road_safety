# 🚦 UK Road Safety Analysis: Provisional 2025
**Lead Researcher:** Arijit Guchhait  
**Focus:** Data Quality, Provenance, and Inferential Statistics (Hypothesis Testing)

## 📋 Project Overview
This project analyzes the **Road Safety Open Data (Provisional 2025)** provided by the UK Department for Transport (DfT). The goal is to identify patterns in road collisions and validate findings using statistical significance tests.

---

## 🔍 Data Provenance & Reliability
Based on my Week 3 quality assessment, the data has been verified for authority and ethics:

| Criterion | Details |
| :--- | :--- |
| **Origin & Authority** | Published by the UK Department for Transport using official **STATS19** police reports. |
| **License** | [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/). |
| **Sensitivity** | Fully anonymized; contains no Personal Identifiable Information (PII). |
| **Timeliness** | **Provisional 2025 status**; dataset is subject to change until the final release in Sept 2026. |

---

## ⚠️ Data Quality & Risk Mitigation
Before performing analysis, I addressed the following critical risks identified in the data:

* **Handling Nulls:** Identified missing values (7 missing values across 3 rows) and converted the `Date` variable from string to date format.
* **Accuracy Risk:** Variables containing `-1` or `unknown` values were handled as missing data to prevent misleading conclusions.
* **Bias Note:** The dataset only includes **injury-only** collisions, excluding damage-only accidents. I have adjusted my research scope to account for this reporting bias.

---

## 📈 Advanced Statistical Implementation
*In development (Applying MA7441 & DataCamp skills)*

Beyond basic visualization, this "Advanced" version of the project includes:
1. **Hypothesis Testing:** Using Chi-Square tests to determine if weather conditions significantly impact accident severity.
2. **Distribution Analysis:** Fitting the collision frequency to a Poisson Distribution to model the probability of rare road events.

---

## 🛠 Tools Used
* **Python/R:** Data cleaning and statistical modeling.
* **SQL:** Querying large-scale collision subsets.
* **Tableau:** Interactive dashboarding for geospatial accident mapping.
