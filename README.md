# 🚌 redBus DataDecode 2025 – Demand Forecasting Challenge

Forecasting demand for bus journeys 15 days in advance using historical booking data, search trends, and enriched holiday features.

![Leaderboard Proof](https://github.com/SannidhyaDas/redBus-DataDecode_rank21_Sol/blob/main/BestSol/LB%20Standings%20.png)

## 🚀 Overview

This repository contains my top-performing solutions for the **RedBus DataDecode Hackathon 2025**, hosted by **Analytics Vidhya** in collaboration with **redBus**. The challenge was to forecast **route-level seat demand** for a specific date of journey (DOJ), **15 days in advance**, using historical booking and search data.

📈 **Final Rank: 21**  
🏆 Recognized for analytical rigor and creative feature engineering.

---

## 🧠 Problem Statement

> Predict total seats booked for each route on a specific date of journey, using data available **15 days in advance**.

👉 Click to visit the detailed problem statement: [RedBus DataDecode Hackathon 2025](https://www.analyticsvidhya.com/datahack/contest/redbus-data-decode-hackathon-2025/)

### 🔍 Key Challenges:
- Impact of holidays, weekends, school calendars, and wedding seasons.
- Regional variability in holiday effects.
- Day-of-week and temporal search trends.
- Noise in user search behavior and booking delays.

---

## 📁 Repository Structure

```bash
redBus-DataDecode_rank21_Sol/
├── BestSol/
│   ├── 15.06.25_v4.ipynb          <- Final best performing solution
│   ├── submission.csv             <- Corresponding submission file
│
├── AnotherSol/
│   ├── 22.06.25_v1.ipynb          <- Alternate solution with holiday enrichment
│   ├── submission_with_holidays.csv
│   ├── holiday_dates.csv          <- Holiday data scraped manually (2023–2025)
│
├── LB Standings .png              <- Proof of leaderboard rank
└── README.md                      <- This file

```
---

## 🏗️ Block Diagram

Visual pipeline of the solution:

**[🖼️ View Block Diagram](your_block_diagram_link_here)**

---

## 🔧 Techniques & Tools Used

- **🧠 ML Models**: LightGBM, XGBoost (with fine-tuned hyperparameters) and Ridge (meta-learner)
- **📅 Temporal Features**: DOJ & DOI-based time deltas, week/day flags
- **📊 Feature Engineering**:
  - Route frequency statistics
  - Search-to-booking ratios
  - Holiday influence (via custom calendar CSV)
  - Long weekend detection
- **🔍 External Data**: Manually curated holiday calendar (India-wide)
- **📦 Tools**: Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib

---

## 📊 Model Performance

| Solution | Description | Notes |
|----------|-------------|-------|
| ✅ **BestSol** | Final best solution with tuned features and minimal leakage | [Notebook](BestSol/15.06.25_v4.ipynb) · [CSV](BestSol/submission.csv) |
| ✅ **AnotherSol** | Used enriched holiday features from custom calendar | [Notebook](AnotherSol/22.06.25_v1.ipynb) · [CSV](AnotherSol/submission_with_holidays.csv) · [Holidays CSV](AnotherSol/holiday_dates.csv) |

Both models were designed with strict 15-day-ahead forecasting logic, avoiding future leakage and optimizing for **RMSE**.

---

## 📈 Evaluation Metric

> **RMSE** (Root Mean Squared Error)  
Used to evaluate model predictions against actual seats booked.

---

## 🏅 Recognition

- **Top 25 Rank (Rank 21)** among 694 teams.
- Uploaded on [GitHub](https://github.com/SannidhyaDas/redBus-DataDecode_rank21_Sol) to share reproducible research.

---

## 🙏 Acknowledgements

- **redBus** and **Analytics Vidhya** for hosting the challenge.
- Public sources for Indian holiday data (e.g., [digitalpathsala.com](https://digitalpathsala.com/indian-festival-calendar-2024/), official state calendars).
- Community on GitHub and AV for discussions and guidance.

---
## 🤝 Connect

If you find this work helpful or have any questions, feel free to reach out:

- 📧 dassannidhya003@gmail.com
- 🌐 [LinkedIn](https://www.linkedin.com/in/sannidhya-das3/)

