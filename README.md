# Employee Attrition Analysis & Prediction

An end-to-end machine learning project to analyze employee turnover, identify key drivers of resignation, and predict flight risk using the IBM HR Analytics dataset.

## Project Overview

- **Dataset**: IBM HR Analytics Employee Attrition dataset (1,470 employee records, 35 features).
- **Factors Analyzed in EDA**:
  - **Demographic & Tenure**: Age Distribution, Tenure / Years at Company.
  - **Financial & Departmental**: Monthly Income by Department.
  - **Workplace & Well-being**: OverTime Status, Job Satisfaction, Work-Life Balance.
  - **Commute & Mobility**: Commute Distance From Home, Business Travel Frequency.
- **Classification Algorithms**: Logistic Regression, Decision Tree, and Random Forest Classifier with class imbalance handling (`class_weight='balanced'`).
- **Rigorous Model Evaluation**:
  - **Stratified 5-Fold Cross-Validation**: Cross-validated ROC-AUC and test metrics (Accuracy, Precision, Recall/Sensitivity, F1-Score, ROC-AUC).
  - **Confusion Matrix Analysis**: Multi-model confusion matrix heatmaps to inspect false positive and false negative trade-offs.
- **Interactive HR Dashboard**: Built with **Gradio**, featuring real-time organizational KPIs (Total Headcount, Attrition Rate, Average Monthly Salary) and a multi-factor Employee Flight Risk Predictor supporting 11 dynamic employee attributes.


## Key Insights from EDA

1. **OverTime**: Employees working overtime exhibit significantly higher attrition rates compared to non-overtime peers.
2. **Work-Life Balance**: Poor work-life balance (Rating 1) shows the highest turnover rates across all balance tiers.
3. **Commute Distance**: Employees living further away from the workplace (higher `DistanceFromHome`) are notably more prone to leaving.
4. **Business Travel Frequency**: Frequent business travelers show substantially higher resignation rates than non-travelers or rare travelers.
5. **Monthly Income & Department**: Attrition is heavily concentrated in lower-income brackets across Sales and R&D roles.
6. **Age & Tenure**: Younger employees (early 20s to early 30s) and employees in their first 1-2 years of tenure experience peak turnover.
7. **Job Satisfaction**: Strong inverse correlation with attrition—lower satisfaction ratings directly correlate with higher turnover.

##  How to Run on Google Colab (Recommended)
1. Click the **Open in Colab** badge above or navigate to [employee_attrition_analysis.ipynb](employee_attrition_analysis.ipynb).
2. Run all cells by selecting **Runtime** ➔ **Run all** (`Ctrl + F9`).
3. The interactive Gradio dashboard will launch inline and generate a public shareable link.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
