# 🏨 Travel, Tourism & Hospitality: Customer Retention and Dynamic Pricing Analysis

## 📊 Executive Problem Statement
In the highly competitive hospitality sector, unpredictable customer cancellations and sub-optimal pricing strategies lead to significant revenue leakage. Traditional booking systems lack the predictive capabilities needed to identify "at-risk" bookings before they cancel. 

**Objective:** This project leverages data analytics and machine learning to predict hotel booking cancellations, uncover the key drivers of churn, and provide actionable, data-driven recommendations to the Revenue Management team to optimize dynamic pricing and maximize occupancy rates.

---

## 📂 Project Phases

*   **Week 1: Data Preparation & Architecture** - Cleaned a large-scale dataset, handled missing values, removed extreme ADR (Average Daily Rate) outliers, and established strict version control using Git.
*   **Week 2: Exploratory Data Analysis (EDA)** - Conducted univariate, bivariate, and multivariate analysis to uncover booking patterns, seasonal trends, and the relationship between lead times and cancellations.
*   **Week 3: Predictive Machine Learning** - Engineered features, scaled data, and built predictive classification models (Logistic Regression, Decision Tree, Random Forest) to proactively identify cancellations.
*   **Week 4: Business Intelligence & Strategy** - Synthesized technical findings into a business-facing Dashboard and formulated strategic recommendations for revenue optimization.

---

## 🧠 Machine Learning Results
We built and evaluated multiple machine learning algorithms to predict whether a guest will cancel their booking.

*   **Champion Model:** **Random Forest Classifier**
*   **Performance Metrics:** The model was rigorously evaluated using Accuracy, Precision, Recall, and ROC-AUC curves, proving highly effective at identifying true cancellations.
*   **Top Churn Drivers (Feature Importance):**
    1.  **Lead Time:** The longer the gap between booking and arrival, the exponentially higher the cancellation probability.
    2.  **Deposit Type:** Bookings without a non-refundable deposit are significantly more likely to churn.
    3.  **Market Segment:** Online Travel Agencies (OTAs) exhibit different cancellation behaviors compared to direct corporate bookings.

*(Note: High-resolution visualizations including the ROC Curve, Confusion Matrix, and Feature Importance charts are available in the `ML_Models_Images/` directory).*

---

## 💡 Strategic Business Recommendations
Based on our predictive models and EDA findings, we recommend the following actions to the Revenue Management team:

1.  **Implement Dynamic Deposit Policies:** Since `lead_time` is the #1 driver of cancellations, the hotel should require a tiered non-refundable deposit for bookings made more than 60 days in advance.
2.  **Targeted Overbooking Strategy:** Utilize our Machine Learning model to flag specific dates with a high predicted cancellation volume. The hotel can safely overbook on these specific dates to ensure 100% capacity without risking "walking" a guest.
3.  **Optimize OTA Partnerships:** Because specific Market Segments have higher cancellation rates, the hotel should renegotiate terms with third-party Online Travel Agencies, or offer exclusive perks (like free breakfast) to incentivize booking directly through the hotel website.
4.  **Proactive Retention Campaigns:** Trigger automated "Excited for your stay!" emails or special upgrade offers to guests who are flagged by the AI as "high-risk" for cancellation to secure their commitment.

---

## 🛠️ Technologies Used
*   **Language:** Python 3
*   **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn
*   **Environment:** Jupyter Notebook / VS Code
*   **Version Control:** Git & GitHub
*   **Visualization:** Power BI / Tableau

---

## 🚀 How to Run the Project
1. Clone the repository: `git clone https://github.com/KrishnaveniMitukula/Hotel-Analytics-Project.git`
2. Ensure you have the required libraries installed: `pip install pandas numpy scikit-learn matplotlib seaborn`
3. Run the analysis in the following order:
   *   `week1_data_cleaning.py` (Generates the clean dataset)
   *   `Exploratory_Data_Analysis.ipynb`
   *   `Week3_Machine_Learning.ipynb`
