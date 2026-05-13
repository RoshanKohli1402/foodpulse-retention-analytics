# 🍽️ FoodPulse — Customer Retention & Cohort Analytics

> End-to-end analytics project simulating a food delivery platform's customer intelligence system — covering cohort retention analysis, RFM segmentation, and an interactive business dashboard.

---

## 📌 Project Overview

Built to answer the core business question every food delivery company obsesses over:

**"Which customers are we losing, when do we lose them, and what's the revenue impact?"**

This project covers the full analyst workflow — from raw data generation to actionable segmentation to a production-grade interactive dashboard.

---

## 🧠 Key Analyses

### 1. Cohort Retention Analysis
- Monthly cohort construction: customers grouped by their **first order month**
- Retention tracked across **12+ months** per cohort
- Identifies the **M0→M1 drop** as the highest-leverage churn intervention point
- Avg month-1 retention: **~20%** — mirrors real food delivery benchmarks

### 2. RFM Segmentation
Customers scored on **Recency, Frequency, and Monetary** value using quintile-based scoring:

| Segment | Count | Avg LTV | Action |
|---|---|---|---|
| Champions | 1,008 | ₹4,707 | Reward, upsell |
| Loyal Customers | 1,071 | ₹3,852 | Loyalty program |
| At Risk | 920 | ₹4,050 | Re-engagement campaign |
| Potential Loyalists | 1,022 | ₹2,465 | Nurture with offers |
| Recent Customers | 590 | ₹2,470 | Onboarding experience |
| Lost | 388 | ₹1,851 | Win-back deep discount |

### 3. Revenue & AOV Trends
- ₹1.73Cr total revenue across 3 years (2022–2024)
- Avg Order Value: ₹375
- Month-on-month revenue growth tracked

### 4. Geo & Cuisine Analytics
- Revenue breakdown across 8 Indian metros
- Mumbai leads with ₹38.1L | Bangalore 3rd at ₹31.2L
- Biryani & Burger are top cuisine categories by order volume

---

## 🛠️ Tech Stack

| Layer | Tools |
|---|---|
| Data Generation | Python, NumPy, Faker |
| ETL & Analysis | Pandas, Scikit-learn |
| Visualisation | Matplotlib, Seaborn, Chart.js |
| Dashboard | HTML5, CSS3, Vanilla JS |

---

## 📁 Project Structure

```
foodpulse-retention-analytics/
│
├── analysis.py                     # Full Python pipeline (ETL + Cohort + RFM)
├── zomato_analytics_dashboard.html # Interactive multi-tab dashboard
├── cohort_heatmap.png              # Exported cohort heatmap
├── rfm_segments.png                # RFM segment chart
└── README.md
```

---

## 🚀 How to Run

```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Run the analysis pipeline
python analysis.py

# Open dashboard in browser
open zomato_analytics_dashboard.html
```

---

## 💡 Key Business Insights

1. **Month-1 churn is the #1 problem** — ~80% of new customers don't reorder. A D+3 push notification + 10% coupon can recover 8–12% of lapsed users.
2. **Champions (20% of customers) drive 31% of revenue** — highest ROI for loyalty investment.
3. **920 At-Risk customers** hold ₹37L in potential annual revenue — a win-back campaign targeting this segment is the single highest-value intervention.
4. **Mumbai + Delhi = 43% of revenue** — city-specific campaigns should be prioritised here.

---

## 📊 Dashboard Preview

The interactive dashboard (`zomato_analytics_dashboard.html`) includes:
- **Overview** — KPI cards, monthly revenue trend, AOV chart
- **Cohort Analysis** — colour-coded retention heatmap, avg retention curve
- **RFM Segmentation** — donut chart, segment deep-dive cards with actionable recommendations
- **Geo & Cuisine** — city revenue bars, cuisine order distribution

---

*Built by [Roshan Kohli](https://linkedin.com/in/roshan-kohli) · github.com/RoshanKohli1402*
