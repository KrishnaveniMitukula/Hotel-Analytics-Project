# 🏨 Travel, Tourism & Hospitality - Customer Retention and Dynamic Pricing Analysis

## 📊 Executive Problem Statement
In the highly competitive travel and hospitality sector, unpredictable customer cancellations and sub-optimal pricing strategies lead to significant revenue leakage. Traditional booking systems lack the predictive capabilities needed to identify "at-risk" bookings before they cancel.

**Objective:** This project leverages data analytics and machine learning to predict hotel booking cancellations, uncover the key drivers of churn, and provide actionable, data-driven recommendations to the Revenue Management team to optimize dynamic pricing and maximize occupancy rates.

---

## 📂 Project Phases

| Week | Phase | Description |
|------|-------|-------------|
| **Week 1** | Data Cleaning & Feature Engineering | Cleaned 119K+ records, handled missing values, removed ADR outliers, engineered new features |
| **Week 2** | Exploratory Data Analysis (EDA) | Univariate, bivariate & multivariate analysis to uncover booking patterns and seasonal trends |
| **Week 3** | Predictive Machine Learning | Built Logistic Regression, Decision Tree & Random Forest classifiers for churn prediction |
| **Week 4** | Business Intelligence Dashboard | Synthesized findings into an interactive Power BI dashboard for the Revenue Management team |

---

## 🧠 Machine Learning Results
We built and evaluated multiple machine learning algorithms to predict whether a guest will cancel their booking.

- **Champion Model:** Random Forest Classifier
- **Performance Metrics:** Evaluated using Accuracy, Precision, Recall, and ROC-AUC curves
- **Top Churn Drivers (Feature Importance):**
  1. **Lead Time:** Longer booking gaps = exponentially higher cancellation probability
  2. **Deposit Type:** Bookings without non-refundable deposits cancel significantly more
  3. **Market Segment:** Online Travel Agencies exhibit higher cancellation rates than direct bookings

> 📁 High-resolution ML visualizations (ROC Curve, Confusion Matrix, Feature Importance) are available in the ML_Models_Images/ directory.

---

## 📊 Business Intelligence Dashboard
![Executive Overview](Finalweek4_Dashbord/DAshboardpage%281%29.png)

![Customer Segmentation](Finalweek4_Dashbord/Dashboardpage%282%29.png)


> 💡 To interact with the dashboard live, download the .pbix file from the Finalweek4_Dashboard/ folder and open it in Power BI Desktop.

### Key Dashboard Insights
- **37.2% Cancellation Rate** — Over 1 in 3 guests cancel their booking
- **Lead Time** is the #1 driver of cancellations
- **Online Travel Agencies** account for 46.9% of all cancellations
- **Non-Refundable Deposits** nearly eliminate cancellations

---

## 💡 Strategic Business Recommendations

1. **Implement Dynamic Deposit Policies:** Require a tiered non-refundable deposit for bookings made more than 60 days in advance to reduce cancellations from early bookers.
2. **Targeted Overbooking Strategy:** Use the ML model to flag specific dates with high predicted cancellation volume. The hotel can safely overbook on these dates to ensure 100% capacity.
3. **Optimize OTA Partnerships:** Since Online Travel Agencies account for 46.9% of cancellations, renegotiate terms with third-party OTAs or offer exclusive perks to incentivize direct bookings.
4. **Proactive Retention Campaigns:** Trigger automated emails or special room upgrade offers to guests flagged by the AI as high-risk for cancellation.
5. **Seasonal Dynamic Pricing:** Leverage the seasonal revenue trends to implement peak-season pricing adjustments, maximizing Revenue Per Available Room (RevPAR) during high-demand months.

---

## 🛠️ Technologies Used

| Category | Tools |
|----------|-------|
| **Language** | Python 3 |
| **Libraries** | Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn |
| **ML Models** | Logistic Regression, Decision Tree, Random Forest |
| **Dashboard** | Microsoft Power BI |
| **Environment** | Jupyter Notebook, VS Code |
| **Version Control** | Git & GitHub |

---

## 📁 Project Structure

    Hotel-Analytics-Project/
    ├── hotel_analyis.ipynb                    # Week 1: Data Cleaning
    ├── Exploratory_Data_Analysis.ipynb        # Week 2: EDA
    ├── Week3_Machine_Learning.ipynb           # Week 3: ML Models
    ├── ML_Models_Images/                      # ML visualizations
    ├── Finalweek4_Dashboard/                  # Power BI Dashboard
    │   ├── hotel_report.pbix
    │   ├── DAshboardpage(1).png
    │   └── Dashboardpage(2).png
    └── README.md                              # This file

## 📥 Dataset Source
The original dataset is publicly available on Kaggle:

🔗 [Hotel Booking Demand Dataset - Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)

Download the dataset and place it in the project root folder before running the notebooks.

---

## 📈 Key Performance Indicators (KPIs)

| KPI | Value | Business Impact |
|-----|-------|-----------------|
| Total Bookings Analyzed | 119,000+ | Comprehensive dataset for reliable insights |
| Overall Cancellation Rate | 37.2% | Critical revenue leakage identified |
| Average Daily Rate (ADR) | $102.40 | Baseline for dynamic pricing optimization |
| Average Lead Time | 104 days | Key predictor for cancellation risk |
| Top Cancellation Source | Online TA (46.9%) | Priority channel for retention strategy |

---

## 🔄 Git Workflow

This project followed a professional Feature Branch Workflow throughout all 4 weeks:

- main — Production-ready, reviewed code
- feature/week3-ml — Machine Learning development branch
- feature/week4 — Dashboard and final documentation branch

Each feature branch was developed independently and merged into main via Pull Requests after thorough review.

---

## 🚀 How to Run the Project

1. Clone the repository:

       git clone https://github.com/KrishnaveniMitukula/Hotel-Analytics-Project.git

2. Install required libraries:

       pip install pandas numpy scikit-learn matplotlib seaborn

3. Run the notebooks in order:
   - hotel_analyis.ipynb (Week 1: Data Cleaning)
   - Exploratory_Data_Analysis.ipynb (Week 2: EDA)
   - Week3_Machine_Learning.ipynb (Week 3: ML Models)

4. Open Finalweek4_Dashboard/hotel_report.pbix in Power BI Desktop for the interactive dashboard.

---

## 👩‍💻 Author
**Krishnaveni Mitukula**

📧 Connect with me on [GitHub](https://github.com/KrishnaveniMitukula)

---

> *This project was developed as part of the Data Analytics Certification Program — Project 2: Travel, Tourism & Hospitality Analysis.*
