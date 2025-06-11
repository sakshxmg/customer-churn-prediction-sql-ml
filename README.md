#  Customer Churn Prediction using Logistic Regression

This project aims to predict customer churn using a logistic regression model. It leverages customer transaction history, service interactions, and feedback data to identify customers likely to churn and provides actionable insights for improving customer retention.

---

##  Project Structure

├── data/ # Raw and cleaned datasets
├── notebooks/ # Jupyter/Colab notebooks for EDA, preprocessing, and modeling
├── models/ # Saved models (pickle, joblib)
├── outputs/ # Evaluation results, plots, and visualizations
├── README.md # Project overview
└── requirements.txt # Dependencies



##  Problem Statement

Customer churn impacts profitability. The goal is to identify high-risk churn customers so that the business can take preemptive action to retain them.

---

##  Datasets Used

- `customers.csv` – Customer demographics and registration info
- `transaction.csv` – Purchase and spending details
- `feedback.csv` – Ratings and feedback comments
- `service_tickets.csv` – Tickets raised, issue types
- `churn_labels.csv` – Target variable indicating churn status

---

##  Features Engineered

- `total_spent`: Total money spent
- `avg_rating`: Average feedback rating
- `num_tickets`: Number of tickets raised
- `days_since_last_tx`: Days since last purchase
- `num_issues`: Number of different issue types raised

---

##  Model Used

- **Logistic Regression**
- Train-Test Split: 70-30 stratified
- Evaluated on Accuracy, Precision, Recall, and F1-score
- Feature importance plotted using model coefficients

---

##  Results

- **Accuracy**: ~87%
- **Key Drivers of Churn**:
  - Low `avg_rating`
  - High `days_since_last_tx`
  - High `num_issues`

---

##  Key Insights

- Dissatisfied and inactive users are highly likely to churn.
- Loyal and frequent spenders are likely to stay.
- Number of unique issue types correlates with churn risk.

---

##  Recommendations

- Launch retention campaigns for at-risk segments.
- Proactively follow up with low-rating customers.
- Improve customer support experience.

---

##  Tools & Technologies

- Python, Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook / Google Colab

---

##  How to Run

```bash
# Clone the repo
git clone https://github.com/your-username/customer-churn-prediction.git
cd customer-churn-prediction

# Install dependencies
pip install -r requirements.txt

# Open the notebook
jupyter notebook notebooks/Churn_Modeling.ipynb
