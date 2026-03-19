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
