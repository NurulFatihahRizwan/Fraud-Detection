# Vehicle Insurance Fraud Detection & Analysis

This project provides a complete solution for detecting fraudulent insurance claims using machine learning. It includes data preprocessing, a Random Forest classification model, and a Power BI dashboard for business intelligence.

## Project Overview
Insurance fraud costs the industry billions annually. This project automates the detection process by:
- Cleaning and preprocessing raw claim data.
- Training a **Random Forest Classifier** to predict the `FraudFound_P` target.
- Exporting results to **Power BI** for interactive visualization.

## Repository Structure
- `Fraud_Detection.ipynb`: Interactive Jupyter Notebook containing the full data science workflow.
- `fraud_detection.py`: Python script version of the model for production or batch processing.
- `fraud_predictions.csv`: The output file containing original features, actual labels, and model-predicted fraud probabilities.

## Technical Details
### Data Pipeline
1. **Data Cleaning**: Numeric missing values are filled with the median, and categorical values with the mode.
2. **Feature Engineering**: Categorical variables are transformed using One-Hot Encoding.
3. **Model**: A `RandomForestClassifier` with 100 estimators and `class_weight='balanced'` to handle the inherent imbalance in fraud datasets.

### Model Performance
The model was evaluated on a 20% test split, achieving the following results:
- **Accuracy**: 94.0%

## Power BI Dashboard
The project concludes by generating `fraud_predictions.csv`, which is optimized for Power BI. 

## Requirements
- Python 3.x
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Power BI Desktop (to view the .pbix dashboard)
