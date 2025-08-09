# customer-churn-prediction

Uses Kaggle Telco Customer Churn data: https://www.kaggle.com/datasets/blastchar/telco-customer-churn

###  Customer Churn Prediction and Analysis — Project Overview
This project aims to predict customer churn for a telecom company using machine learning and provide actionable insights through interactive visualizations. Customer churn—the loss of customers—is a critical business problem that impacts revenue and growth. Early identification of at-risk customers enables targeted retention strategies.

### Data and Preparation
The project uses the publicly available Telco Customer Churn dataset, which includes customer demographics, service details, account information, and churn labels. Initial steps involve:

### Data cleaning 
Handling missing or inconsistent values (e.g., converting TotalCharges to numeric),

### Encoding 
Transforming categorical variables into numerical formats suitable for machine learning,

### Feature engineering 
Creating relevant features such as tenure, contract types, and payment methods.

### Modeling
A Random Forest Classifier is trained to predict the probability that a customer will churn based on the input features. Model development includes:

Splitting data into training and testing sets,

Training the model on the training set,

Evaluating performance using metrics like accuracy, precision, recall, and ROC AUC,

Generating churn risk scores for each customer in the test set.

### Output
The model outputs a scored dataset containing:

Customer features,

Actual churn label,

Predicted churn risk score (a probability between 0 and 1).

This output is saved as a CSV file (churn_scored.csv), which serves as the basis for visualization.

### Visualization
Using Tableau Public, an interactive dashboard is created to visualize the churn analysis results:

Distribution of churn risk scores across customers,

Churn rates segmented by contract types and tenure,

Filters for exploring data by payment methods and other demographics,

Clear, color-coded visual elements that highlight high-risk segments.

### Business Impact
This end-to-end solution combines predictive modeling with rich visual storytelling to:

Identify customers at highest risk of churn,

Help business teams prioritize retention efforts,

Inform decisions on contract offers and customer engagement strategies,

Provide an easily accessible dashboard for continuous monitoring.

### How to Use
Run the Jupyter notebook Customer_Churn.ipynb to reproduce the data preparation, modeling, and scoring steps,

Load the generated CSV into Tableau to explore or update the dashboard,

Use the interactive dashboard link to view insights without installing any software.

### Technologies Used
Python (pandas, scikit-learn, matplotlib) for data analysis and modeling,

Tableau Public for interactive visualizations,

Git and GitHub for version control and portfolio hosting.
