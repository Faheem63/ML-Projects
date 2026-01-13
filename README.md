# End To End Customer Churn Prediction Using Machine Learning -


-------------------------------------------------------------------------------------------
# 🧠 How I Approached the Problem ---


# 1️⃣ Data Understanding & Preparation
# Dataset Telco Customer Churn dataset (Kaggle)
  Link- https://www.kaggle.com/datasets/ankitverma2010/ecommerce-customer-churn-analysis-and-prediction
# Consumer Complaints (Kaggle)
  Link- https://www.kaggle.com/datasets/selener/consumer-complaint-database
  
  Analyzed numerical and categorical features
  
  Checked class imbalance and churn patterns
  
  Handled missing values and cleaned incorrect data types
  
  Removed outliers using the IQR method
  
  Performed EDA to understand key churn drivers
  
# 2️⃣ Feature Engineering
  Created meaningful features like average charges per month
  Captured customer behavior using tenure and contract information
  Selected important features using correlation and tree-based importance
  This step significantly improved model performance.
  
# 3️⃣ Model Building
  Trained and compared multiple models:
  Logistic Regression (baseline)
  Random Forest (main model)
  Neural Network (MLP) (advanced model)
  The Random Forest model performed best overall.
  
# 4️⃣ Model Tuning & Evaluation
  Used GridSearchCV for hyperparameter tuning
  Focused on Recall and F1-score, since missing churn customers is costly
  Evaluated performance using confusion matrix and classification metrics
  
# 5️⃣ Error Analysis
  Analyzed false positives and false negatives
  Found that:
  Short-tenure, month-to-month customers are often predicted to churn
  Long-tenure customers may churn after sudden price increases
  Used these insights to guide feature improvements

# 6️⃣ Text Data Integration (NLP)
  Processed customer complaint text using:
  Text cleaning
  TF-IDF vectorization
  Logistic Regression
  Generated a complaint risk score to capture customer dissatisfaction
  Used this score as an additional signal to improve churn understanding

# 7️⃣ Model Explainability
  Used SHAP to explain model predictions
  Identified top churn drivers such as contract type, tenure, and monthly charges
  Made predictions more transparent and business-friendly

# 🚀 Deployment Thinking
  Although not deployed, the system was designed with production in mind:
  FastAPI for serving predictions
  REST API for real-time inference
  AWS (EC2 / ECS) for cloud deployment
  Monitoring for model performance and drift

# 📌 Key Learnings
  Feature engineering matters more than model complexity
  Accuracy alone is not enough for churn problems
  Error analysis provides valuable business insights
  Text data adds context that structured data misses
  Explainability is essential for real-world ML systems
  Thinking about deployment early improves solution quality

# ✅ Why This Project Matters
  This project demonstrates my ability to:
  
  Work with real-world data
  Build and compare ML models
  Apply NLP to enhance predictions
  Explain model decisions clearly
  Think beyond notebooks toward production systems
