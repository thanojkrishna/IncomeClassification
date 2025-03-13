# Income Classification

## 📄 Project Overview
This project aims to predict individuals' income categories ('>50K' or '<=50K') based on various demographic attributes. Utilizing machine learning classifiers, the goal is to build a model that accurately classifies income levels.

## 📁 Repository Structure

### 📂 data/
Contains datasets used for analysis and modeling.
- `adult.data`: Training dataset with demographic attributes and income labels.
- `adult.test`: Testing dataset for model evaluation.

### 📂 notebooks/
Jupyter notebooks detailing data analysis, preprocessing, and model development.
- `Income_Classification.ipynb`: Main notebook encompassing data preprocessing, exploratory data analysis (EDA), and model implementation.

### 📂 scripts/
Python scripts for data processing and model functions.
- `data_preprocessing.py`: Script for cleaning and preparing the dataset.
- `model_training.py`: Script for training and evaluating classifiers.

### 📂 reports/
Documentation and reports generated from the analysis.
- `Final_Report.pdf`: Detailed report summarizing methodologies, findings, and conclusions.

### 📄 requirements.txt
Lists the Python packages required to run the project.

## 🔍 Exploratory Data Analysis (EDA)
- **Demographic Distribution**: Analysis of age, education, occupation, and other features.
- **Income Distribution**: Examination of income categories and class imbalance.
- **Feature Relationships**: Insights into correlations between features and income levels.

## 🧠 Modeling Approach
Implemented classifiers:
1. **Logistic Regression**: Baseline linear model.
2. **Decision Tree**: Captures non-linear relationships.
3. **Random Forest**: Ensemble method to improve accuracy.
4. **Support Vector Classification**: Effective in high-dimensional spaces.
5. **K-Nearest Neighbors**: Instance-based learning.
6. **Gaussian Naive Bayes**: Based on Bayes' theorem with independence assumptions.
7. **Quadratic Discriminant Analysis**: Considers class covariance.
8. **AdaBoost**: Boosting method to combine weak learners.
9. **Gradient Boosting**: Sequential ensemble technique.
10. **Multi-layer Perceptron Classifier**: Neural network-based approach.

### Evaluation Metrics
Models were evaluated using:
- **Accuracy**: Proportion of correct predictions.
- **Precision**: True positive rate among predicted positives.
- **Recall**: True positive rate among actual positives.
- **F1-Score**: Harmonic mean of precision and recall.

*Detailed performance metrics are available in the final report.*

## 🚀 How to Use This Repository

1. **Clone the Repository**:
```bash
git clone https://github.com/thanojkrishna/IncomeClassification.git
cd IncomeClassification
```

2. **Set Up the Environment**:
- Ensure you have Python installed (preferably version 3.7 or higher).
- Install necessary packages:
```bash
pip install -r requirements.txt
```

3. **Explore the Data**:
- Access the `notebooks/` directory to view and run Jupyter notebooks.
- Open `Income_Classification.ipynb` to follow the analysis and modeling steps.

## 🙏 Acknowledgements
- Data sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/adult).
- Special thanks to the course instructors for guidance and support.

---
Feel free to fork, star, or contribute to this repository if you find it useful!
