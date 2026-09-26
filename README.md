# Customer Analytics & Revenue Performance Dashboard

An end-to-end data analytics and business intelligence project analyzing Q1 performance (Jan – Mar 2023) for Springfield, IL retail operations. This project includes data cleaning, automated pipelines, feature engineering, RFM-based customer segmentation, and interactive dashboarding.

---

#DASHBOARD PREVIEW 

## BACKGROUND 

<img width="722" height="443" alt="Screenshot 2026-09-26 182126" src="https://github.com/user-attachments/assets/f8d3ec2f-481a-4341-872c-f76a698c3271" />

## DASHBOARD 

<img width="760" height="430" alt="Screenshot 2026-09-26 182557" src="https://github.com/user-attachments/assets/cfa63f77-7ae3-4ab9-b5b0-c716af625edd" />


--- 




## 📌 Executive Summary & Key Insights

Based on Q1 performance metrics, total revenue reached **$332** across **10 orders** with an average order value (AOV) of **$33**.

* **Revenue Peak & Decline:** Revenue peaked in February ($170+) before experiencing a drop in March (~$45).


* **Customer Concentration:** The top 3 customers (Bob, Grace, Hank) generate **~48% of total revenue**.


* **Data Quality & Governance:** Achieved **90% data completeness**, with **1 record imputed** for missing values.


* **Customer Tiers:** Segmented into **Champion**, **Regular**, and **At Risk** groups.



---

## 🛠️ Tech Stack & Architecture

* **Language:** Python 3.10+
* **Data Processing & Analysis:** Pandas, NumPy
* **Visualization:** Dash / Plotly, Matplotlib, Seaborn
* **Database & Storage:** PostgreSQL / SQLite
* **Environment & Tooling:** Jupyter Notebook, Docker, Git

---

## 📁 Repository Structure

```text
├── data/
│   ├── raw/                  # Original raw customer and order data
│   └── processed/            # Cleaned, transformed, and imputed datasets
├── notebooks/
│   ├── 01_eda_and_cleaning.ipynb   # Missing value imputation & distribution checks
│   └── 02_customer_segmentation.ipynb # Scoring & Tier classification logic
├── src/
│   ├── data_pipeline.py      # ETL automation script
│   ├── metrics.py            # Key business metric definitions (AOV, MoM, Score)
│   └── dashboard_app.py      # Dashboard code
├── assets/
│   └── dashboard_preview.png # Dashboard screenshot
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation

```

---

## 📊 Business Metrics & Analytics Breakdown

### 1. Key Performance Indicators (KPIs)

* **Total Revenue:** $332 (+40% MoM)


* **Total Orders:** 10


* **Active Customers:** 10


* **Average Order Value (AOV):** $33


* **Average Customer Score:** 67 / 100


* **Data Completeness:** 90% (1 record imputed)



### 2. Revenue Trend Analysis

| Month | Revenue Trend | Key Observation |
| --- | --- | --- |
| **Jan 2023** | ~$120

 | Baseline performance

 |
| **Feb 2023** | ~$170

 | Monthly peak driven by repeat orders

 |
| **Mar 2023** | ~$42

 | Significant drop requiring customer retention focus

 |

### 3. Revenue by Customer Analysis

* **Top Contributors:** Bob (~$58), Grace (~$52), Hank (~$42)


* **Mid-Tier:** Frank (~$38), Eve (~$28), Alice (~$23), Unknown (~$22)


* **Lower-Tier:** John (~$18), Charlie (~$18), Jane (~$12)



### 4. Tier Segmentation & Score vs. Revenue Correlation

* **Champion:** High revenue, high score metrics.


* **Regular:** Moderate spending and engagement metrics.


* **At Risk:** Low score or declining engagement requiring re-engagement campaigns.


* **Scatter Plot Insights:** Engagement score does not strictly correlate with spend; targeted upside potential exists for high-score, lower-spend customers.



---

## 🚀 Getting Started

### Prerequisites

* Python 3.10 or higher
* `pip` package manager

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/your-username/customer-analytics-dashboard.git
cd customer-analytics-dashboard

```


2. **Create and activate a virtual environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

```


3. **Install dependencies:**
```bash
pip install -r requirements.txt

```


4. **Run the Dashboard:**
```bash
python src/dashboard_app.py

```


Open `[http://127.0.0.1:8050/](http://127.0.0.1:8050/)` in your browser to view the dashboard.

---

## 💡 Recommendations & Next Steps

1. **Investigate March Churn:** Run cohort analysis to determine why revenue dropped substantially in March.


2. **Target High-Score / Low-Spend Segment:** Create cross-sell campaigns for customers with high engagement scores (70–90) who currently yield low revenue (<$30).


3. **Handle Data Quality:** Standardize identity verification to eliminate `Unknown` customer records.
