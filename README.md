# Predicting User Churn for an E-commerce Platform

## Project Overview

This project aims to predict user churn on an e-commerce platform using behavioral data. The goal is to:

- Identify users likely to churn (stop engaging with the platform).
- Provide actionable insights to improve user retention.

## Dataset

**Filename:** `events.csv`

### Columns:

- **event\_time**: Datetime of the event (e.g., `2020-12-01 09:00:00`)
- **event\_type**: Type of event (e.g., `view`, `cart`, `purchase`)
- **product\_id**: Product identifier
- **category\_id**: Category identifier
- **category\_code**: Human-readable category code (if available)
- **brand**: Product brand
- **price**: Price of the product
- **user\_id**: User identifier
- **user\_session**: Session identifier

## Steps

### 1. Data Inspection & Preprocessing

- Loaded the dataset and performed initial exploration.
- Cleaned data by handling missing values, duplicates, and inconsistencies.
- Parsed `event_time` into datetime format and ensured correct data types.

### 2. Exploratory Data Analysis (EDA)

- Explored event distributions (e.g., `view`, `cart`, `purchase`) over time.
- Analyzed user-level summaries:
  - Total spend per user.
  - Frequency of visits and time between visits.
- Identified key patterns and anomalies in user behavior.

### 3. Defining Churn

- **Definition**: A user is considered to have churned if they made no purchase or site visit within the last 30 days.
- **Justification**: This threshold captures a significant gap in user engagement based on typical e-commerce behavior.

### 4. Feature Engineering

Key features include:

- **Recency, Frequency, Monetary (RFM)** metrics.
- Session-based metrics (e.g., session count, average session duration).
- Behavioral patterns (e.g., view-to-cart ratio, cart-to-purchase ratio).
- Product/brand preferences.

### 5. Predictive Modeling

- Trained a machine learning model to predict churn using the engineered features.
- Evaluated the model using metrics such as AUC, Precision, Recall, and F1 score.

### 6. Interpretability & Insights

- Used SHAP values to identify influential features.
- Highlighted categories and products contributing to churn.

### 7. Business Recommendations

- Personalized retention strategies (e.g., targeted offers).
- Improved product recommendations and pricing strategies.
- Enhanced user experience based on behavioral insights.

## Deliverables

1. **Jupyter Notebook**: Contains the full analysis and code.
2. **Summary Report**: Highlights findings, methodology, and business recommendations.
3. **Dataset**: Included if permissible.

## Requirements

### Libraries

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- shap

### Running Instructions

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ecommerce-churn-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd ecommerce-churn-prediction
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Run the notebook step-by-step.

## Insights from Research Paper

Incorporated best practices from the provided research paper to guide feature engineering and churn definition.

## Contact

For any queries, feel free to reach out:

- **Name**: Prathamesh Atkare
- **Email**: prathmeshatkare07@gmail.com
- **GitHub**: (https://github.com/prathameshatkare)

---

Thank you for reviewing this project!

good

