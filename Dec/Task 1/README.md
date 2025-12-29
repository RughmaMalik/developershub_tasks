# Term Deposit Subscription Prediction

## Objective
The goal of this project is to predict whether a bank customer will subscribe to a term deposit based on direct marketing campaign data. By applying machine learning classification models, this system identifies high-probability prospects to help financial institutions optimize their marketing strategies.

## Dataset
- **Source:** UCL - Bank Marketing Data Set (`bank-additional-full.csv`)
- **Attributes:**
  - age, job, marital, education
  - default, housing, loan
  - contact, month, day_of_week, duration
  - campaign, pdays, previous, poutcome
  - emp.var.rate, cons.price.idx, cons.conf.idx, euribor3m, nr.employed
- Link: [UCL Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)

## Steps Performed
1.  **Preprocessing:** handled 'unknown' values, encoded categorical variables using Label Encoding, and applied StandardScaler to normalize numerical features.
2.  **EDA:** Visualized target distribution, age demographics, and subscription rates by job type and month to identify trends.
3.  **Model Comparison:**
    * **Logistic Regression:** Used as a baseline linear classifier.
    * **Random Forest:** Implemented to capture complex, non-linear relationships in customer behavior.
4.  **Explainability:** Integrated **LIME** (Local Interpretable Model-agnostic Explanations) to provide transparency on why specific predictions were made (e.g., why a specific customer was rejected).

## Results
* **Logistic Regression:**
  * F1-Score: 0.52
  * ROC-AUC: 0.94
* **Random Forest:**
  * F1-Score: 0.60
  * ROC-AUC: 0.95

*Conclusion:* The Random Forest model outperformed Logistic Regression. Feature importance analysis and LIME explanations highlighted that **call duration**, **contact type**, and **previous campaign outcomes** are the strongest predictors of subscription success.

## How to Run
1. Open the notebook in Google Colab or Jupyter Notebook.
2. Install the necessary library for explainability:
   `!pip install lime`
3. Upload the dataset (`bank-additional-full.csv`).
4. Run all cells to train the models and visualize the LIME explanations.
