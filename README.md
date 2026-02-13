# Employee Retention Analysis Using Machine Learning

A data-driven analysis to predict employee turnover and identify key factors affecting employee retention using logistic regression.

## 📋 Project Overview

This project analyzes employee data to understand what factors contribute to employee turnover and builds a predictive model to help HR departments make data-driven decisions about retention strategies.

## 🎯 Objectives

1. Perform exploratory data analysis (EDA) to identify variables that impact employee retention
2. Visualize the relationship between salary levels and employee retention
3. Analyze the correlation between departments and employee retention
4. Build a logistic regression model to predict employee turnover
5. Evaluate model performance and accuracy

## 📊 Dataset

**Source**: HR Employee Data (HR_comma_sep.csv)

**Features**:
- `satisfaction_level`: Employee satisfaction level (0-1)
- `last_evaluation`: Last performance evaluation score (0-1)
- `number_project`: Number of projects assigned
- `average_montly_hours`: Average monthly working hours
- `time_spend_company`: Years spent at the company
- `Work_accident`: Whether employee had a work accident (0/1)
- `left`: Target variable - whether employee left (0/1)
- `promotion_last_5years`: Promotion in last 5 years (0/1)
- `Department`: Employee's department
- `salary`: Salary level (low/medium/high)

**Dataset Size**: 14,999 employees

## 🔍 Key Findings

### Exploratory Data Analysis

1. **Satisfaction Level Impact**
   - Strongest negative relationship with employee turnover
   - Lower satisfaction → Higher likelihood of leaving

2. **Salary Impact**
   - Low salary employees have significantly higher turnover rates
   - Clear correlation between compensation and retention

3. **Department Analysis**
   - Sales and Support departments show higher turnover
   - Different retention patterns across departments

4. **Time in Company**
   - Employees with longer tenure are paradoxically more likely to leave
   - Suggests potential career stagnation issues

## 🤖 Machine Learning Model

### Model: Logistic Regression

**Selected Features**:
- `satisfaction_level`
- `average_montly_hours`
- `number_project`
- `time_spend_company`
- `promotion_last_5years`
- `salary_low`
- `salary_medium`

### Model Performance

- **Accuracy**: 76%
- **Precision (Class 0 - Stayed)**: 0.80
- **Recall (Class 0 - Stayed)**: 0.92
- **F1-Score (Class 0 - Stayed)**: 0.85

The model shows strong performance in predicting employees who will stay, with moderate performance for predicting turnover.

## 📈 Visualizations

The analysis includes:

1. **Bar Chart**: Salary Level vs Employee Retention
   - Shows clear trend of higher retention with higher salaries

2. **Bar Chart**: Department vs Employee Retention
   - Compares retention rates across all departments

## 🛠️ Technologies Used

- **Python 3.x**
- **Libraries**:
  - `pandas` - Data manipulation and analysis
  - `numpy` - Numerical computations
  - `matplotlib` - Data visualization
  - `scikit-learn` - Machine learning model and evaluation
  - `warnings` - Warning management

## 🚀 How to Run

### Prerequisites

```bash
pip install pandas numpy matplotlib scikit-learn
```

### Running in Google Colab

1. Upload the notebook to Google Colab
2. Upload `HR_comma_sep.csv` to your Google Drive
3. Update the file path in the notebook:
   ```python
   employee = pd.read_csv("/content/drive/MyDrive/HR_comma_sep 1.csv")
   ```
4. Run all cells sequentially

### Running Locally

1. Clone this repository
2. Install required packages
3. Update the file path to your local CSV location
4. Run the Jupyter notebook

## 📁 Project Structure

```
employee-retention-analysis/
│
├── employee_retention_analysis.ipynb  # Main analysis notebook
├── HR_comma_sep.csv                   # Dataset (not included - too large)
├── README.md                          # This file
└── requirements.txt                   # Python dependencies
```

## 💡 Key Insights for HR

1. **Focus on Satisfaction**: Employee satisfaction is the strongest predictor of retention
2. **Competitive Compensation**: Salary adjustments could significantly reduce turnover
3. **Career Development**: Address career stagnation for long-tenure employees
4. **Department-Specific Strategies**: Tailor retention programs by department
5. **Work-Life Balance**: Monitor project load and working hours

## 📊 Results Summary

| Metric | Value |
|--------|-------|
| Model Accuracy | 76% |
| Most Important Factor | Satisfaction Level |
| Salary Impact | High (low salary → high turnover) |
| Department with Highest Turnover | Sales, Support |

## 🔮 Future Improvements

- [ ] Test additional models (Random Forest, XGBoost)
- [ ] Perform feature engineering
- [ ] Handle class imbalance with SMOTE
- [ ] Cross-validation for robust evaluation
- [ ] Deep dive into department-specific factors
- [ ] Time-series analysis of retention trends
- [ ] Interactive dashboard for HR insights

## 📝 Conclusions

The logistic regression model successfully predicts employee retention with **76% accuracy**. The analysis reveals that:

- **Employee satisfaction** is the most critical factor
- **Compensation** plays a significant role in retention
- **Department** and **tenure** also influence turnover decisions

These insights can help HR departments develop targeted retention strategies to reduce turnover and improve employee satisfaction.

## 👤 Author

[OJUMU OLUWABUKOLA]
- GitHub: [@bouqui-x](https://github.com/bouqui-x)

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments

- Dataset sourced from HR analytics study
- Data scientist and engineering| Women Techster
