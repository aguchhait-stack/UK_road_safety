# 🚗 2025 UK Road Safety: A Data-Driven Analysis
**Author:** Arijit Guchhait  
**Status:** MSc Data Science Project | University of Leicester  

---

## 📌 Project Overview
This project investigates the underlying patterns of road collisions in the UK using provisional 2025 data. This analysis identifies the "danger signals"—specific combinations of time, location, and speed—that determine the severity of a crash.

### **The "Why" Behind the Research**
While many reports focus on rain or snow, this study reveals a "Good Weather Trap," where 91% of incidents occur in fine conditions, suggesting that **human behavior and timing** are the primary drivers of risk.

---

## 🚀 Key Insights
* **The 74% Reality:** Nearly 74% of collisions are "Slight." This drives our model's **73.77% accuracy** rate.
* **The Friday Surge:** Collision frequency peaks on Fridays as the work week ends.
* **Daily Danger Windows:** The most volatile window for collisions occurs between **15:00 and 17:00**.
* **Speed vs. Lethality:** While 30 mph zones have the highest volume, **60-70 mph zones** drive the highest severity.

---

## 🛠️ Technical Workflow
* **Language:** R (Quarto)
* **Modeling:** Random Forest (`randomForest`, `caret`)
* **Fairness Check:** Performed a stability audit using random sampling to ensure **Demographic Parity**.

---

## 📁 Repository Structure
* **`data/`**: Raw and processed CSV datasets.
* **`outputs/`**: Contains the final rendered reports (**Collision.pdf** and **Collision.html**).
* **`Project.qmd`**: The main Quarto source file containing all analysis and code.
* **`README.md`**: Project documentation and overview.
* **`LICENSE`**: MIT License.

---

## ⚖️ Future Work
Because "Slight" accidents dominate the data, future versions will implement **SMOTE (Over-sampling)** and **Class Weighting** to help the algorithm better predict rare, high-stakes "Fatal" events.

---

### **License & Data Attribution**
This project uses data provided by the **Department for Transport (DfT)** under the **Open Government Licence v3.0**.

* **License:** [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/)
* **Collection Method:** Downloaded via `read_csv()` from the official DfT portal.
* **Version / Release Date:** 25 September 2025.
* **Access URL:** [Official Dataset](https://data.dft.gov.uk/road-accidents-safety-data/dft-road-casualty-statistics-collision-provisional-2025.csv)
* **Update Frequency:** Bi-annual (Provisional in November; Final in September 2026).
* **Known Limitations:** Data is provisional; negative values (-1) represent missing or unknown data.

### **Predictive Power: Modeling Collision Severity**
The statistical model developed in this study achieved a **~74% accuracy rate**, indicating a remarkably strong relationship between behavioral inputs and the resulting **Collision Severity**.

**Key Predictive Variables:**
* **The Chronological Pulse:** Hour of the day and Day of the week.
* **The Velocity Variable:** Speed limits in specific zones.
* **The Severity Outcome:** How these factors intersect to determine whether a collision is classified as **Slight, Serious, or Fatal**.

By focusing on **Collision Severity**, this analysis moves beyond simple counting and toward understanding the factors that lead to the most life-altering outcomes on UK roads.

---
