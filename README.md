# Customer Churn Prediction & Analysis

### This project focuses on predicting customer churn for a telecom company using the Telco Customer Churn dataset from Kaggle.

Churn (when customers leave a service) is a big issue for subscription businesses. If we can figure out which customers are most likely to churn, the company can take action to retain them—like offering discounts, better plans, or improved support.

### 🔍 What I Did

#### Loaded the dataset (7,043 customers).

#### Cleaned and prepared the data:

Converted TotalCharges from text to numeric and filled missing values with the median.

Turned Yes/No columns into 1/0.

One-hot encoded categorical columns like Contract, Payment Method, Internet Service, etc.

Split the data into training (80%) and testing (20%).

Built a Random Forest Classifier to predict churn.

#### Evaluated performance using:

Classification report (precision, recall, F1-score).

ROC AUC score (0.83 → good discrimination between churn and non-churn customers).

Scored customers with churn risk probabilities and saved the results in churn_scored.csv.

Prepared for visualization by exporting the scored data so it can be used in Tableau (or any dashboarding tool).

### 📊 Results

Overall model accuracy: ~80%

ROC AUC: 0.83 (shows good separation between churn vs non-churn customers).

Model does a solid job predicting customers who stay, but catching churners is harder (as expected in imbalanced datasets).

### 👉 Example: Month-to-month contracts and electronic check payments showed higher churn risk, while longer tenure and two-year contracts had lower churn.

### 🛠 Tech Stack

Python: pandas, scikit-learn, numpy

Modeling: Random Forest Classifier

Visualization: Tableau Public (dashboard-ready CSV output)

Other: joblib (to save the trained model for reuse)

### 📂 Project Files

Customer_Churn.ipynb → Jupyter notebook with full workflow.

churn_model.pkl → Saved Random Forest model.

churn_scored.csv → Scored dataset with churn probabilities (for dashboards).

WA_Fn-UseC_-Telco-Customer-Churn.csv → Original dataset (needs to be downloaded from Kaggle).

### 💡 Business Takeaways

Customers on month-to-month contracts are much more likely to churn.

Electronic check payments are strongly linked with higher churn.

Long-term contracts = stickier customers.

With this model, a telecom company could focus retention campaigns on the high-risk groups and potentially save significant revenue.

### ✨ Summary
This project shows an end-to-end workflow: data cleaning → feature engineering → modeling → evaluation → visualization-ready output.

### Also take a look at my Tableau vizzes here: [Link]([url](https://public.tableau.com/app/profile/siddhitabagwe/viz/KaggleTelcoCustomerChurn/CustomerChurnRateDashboard))
