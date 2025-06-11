# customer-churn-prediction-sql-ml
#  Customer Churn Prediction with SQL + Machine Learning

This project combines the power of **SQL** for data exploration and **Python (ML)** for customer churn prediction.

##  Objective

Predict which customers are at risk of churn using their:
- Purchase behavior
- Feedback ratings
- Customer service tickets

##  Stack Used
- SQL (MySQL Workbench)
- Python (Google Colab, Pandas, Scikit-learn, Seaborn, Matplotlib)
- Logistic Regression Model

##  Project Structure

├── data/ # CSVs exported from MySQL
├── sql/ # Database schema & churn queries
├── notebooks/ # ML model in Google Colab
├── images/ # Visualizations & plots
├── churn_project_report.pdf # Final report
└── README.md


##  Model Performance


| Metric       | Value     |
|--------------|-----------|
| Accuracy     | 92%       |
| Precision    | 84%       |
| Recall       | 77%       |
| F1-Score     | 80%       |


##  Insights

- Poor feedback (<2.5) and frequent support issues (>3) are strong churn predictors.
- Inactive customers (no purchase in 6 months) are at risk.
- Certain regions show higher churn.


##  Business Actions

- Send re-engagement offers to at-risk customers.
- Improve support experience to reduce service-related churn.
- Regularly monitor churn flags from the dashboard.

---

##  How to Run

1. Import CSVs from `data/` into MySQL.
2. Run SQL scripts in `sql/` for data preparation and churn flagging.
3. Open `notebooks/churn_prediction.ipynb` in Google Colab.
4. Run all cells to clean data, train ML model, and visualize.
