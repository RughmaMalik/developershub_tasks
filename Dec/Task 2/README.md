# Customer Segmentation Using Unsupervised Learning

## Objective
The primary aim of this study is to categorize mall clientele into actionable groups based on their profiles and habits. The project aims to uncover hidden patterns within the data, enabling optimized business decision-making and maximizing customer engagement.

## Dataset
- Source: Kaggle – Mall_Customers
- Attributes:
  - CustomerID, Genre, Age
  - Annual Income (k$), Spending Score (1-100)
- Link: [Kaggle Dataset](https://www.kaggle.com/datasets/shwetabh123/mall-customers)

## Steps Performed
1.  **Data Ingestion & Profiling**: Initial inspection to assess data integrity and structure.
2.  **Exploratory Data Analysis (EDA)**: Visualizing distributions of age, gender, and financial metrics to detect early trends.
3.  **Preprocessing**: Encoding categorical data (Gender) and applying feature scaling to standardize numerical ranges.
4.  **Hyperparameter Tuning**: Utilizing the **Elbow Method** to scientifically determine the optimal cluster count ($k$).
5.  **Model Training**: Applying the **K-Means algorithm** to partition the data.
6.  **Visualization**: Employing **PCA** and **t-SNE** to project high-dimensional clusters onto a 2D plane for visual verification.
7.  **Strategic Interpretation**: Translating statistical clusters into business personas.

## Results
The modeling process successfully partitioned the customer base into **five unique clusters**. Each group exhibited high internal similarity regarding financial status and age, validating the model's ability to distinguish between diverse shopper profiles effectively.

### Strategic Recommendations
Based on the characteristics of the identified segments, the following approaches are proposed:

| Segment Profile | Strategy Description |
| :--- | :--- |
| **High Income, High Spend** | Sell premium and luxury items. Offer VIP rewards to keep them loyal. |
| **High Income, Low Spend** | Send personalized recommendations and reminders to encourage them to buy. |
| **Low Income, High Spend** | Offer "buy more, save more" bundles and fun rewards for frequent shopping. |
| **Low Income, Low Spend** | Focus on big sales, discount coupons, and clearance items. |
| **Moderate Income/Spend** | Suggest related products (like accessories) to slightly increase their total bill. |


## How to Run
1. Open the notebook in Google Colab.
2. Upload the dataset (`Mall_Customers.csv`)
3. Run all cells to reproduce results.
