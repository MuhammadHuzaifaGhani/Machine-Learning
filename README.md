# Student Performance Analysis

A comprehensive data analysis project that explores factors affecting student performance and builds predictive models to estimate exam scores based on study hours.

## 📊 Project Overview

This project analyzes student performance data to understand the relationship between various factors and exam scores. It includes exploratory data analysis (EDA), data visualization, and machine learning models to predict student performance.

## 🎯 Objectives

- Analyze student performance factors and their correlations
- Visualize data patterns and distributions
- Build predictive models for exam scores
- Compare linear and polynomial regression models
- Provide insights for educational improvement

## 📁 Dataset

The project uses `StudentPerformanceFactors.csv` which contains student data including:
- **Hours_Studied**: Number of hours spent studying
- **Exam_Score**: Student's exam performance score
- Additional categorical and numerical features

## 🛠️ Technologies Used

- **Python 3.x**
- **pandas**: Data manipulation and analysis
- **matplotlib**: Data visualization
- **seaborn**: Statistical data visualization
- **scikit-learn**: Machine learning models and metrics
- **numpy**: Numerical computations

## 📋 Requirements

\`\`\`bash
pip install pandas matplotlib seaborn scikit-learn numpy
\`\`\`

## 🚀 Getting Started

1. **Clone the repository**
   \`\`\`bash
   git clone <repository-url>
   cd student-performance-analysis
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   pip install -r requirements.txt
   \`\`\`

3. **Ensure dataset is available**
   - Place `StudentPerformanceFactors.csv` in the project root directory

4. **Run the analysis**
   \`\`\`bash
   python main.py
   \`\`\`

## 📈 Analysis Pipeline

### 1. Data Exploration
- **Data Loading**: Import and examine the dataset structure
- **Data Quality Check**: Identify missing values, duplicates, and data types
- **Basic Statistics**: Generate descriptive statistics for numerical features

### 2. Data Preprocessing
- **Missing Value Handling**: Remove rows with missing data
- **Data Type Analysis**: Separate numerical and categorical columns
- **Data Cleaning**: Ensure data quality for analysis

### 3. Exploratory Data Analysis (EDA)

#### Correlation Analysis
- Generate correlation matrix for numerical features
- Visualize correlations using heatmap
- Identify relationships between variables

#### Distribution Analysis
- Create histograms with KDE for numerical features
- Analyze data distribution patterns
- Identify potential outliers

#### Categorical Analysis
- Examine unique values in categorical columns
- Generate value counts for categorical features
- Understand data composition

### 4. Data Visualization
- **Scatter Plot**: Hours_Studied vs Exam_Score relationship
- **Correlation Heatmap**: Feature relationships visualization
- **Distribution Plots**: Individual feature distributions

### 5. Machine Learning Models

#### Linear Regression
- **Features**: Hours_Studied
- **Target**: Exam_Score
- **Evaluation Metrics**:
  - Mean Absolute Error (MAE)
  - R-squared Score
- **Visualization**: Regression line overlay

#### Polynomial Regression
- **Degree**: 2nd order polynomial
- **Feature Engineering**: Polynomial feature transformation
- **Comparison**: Performance vs Linear Regression

## 📊 Model Performance

The project compares two regression models:

| Model | MAE | R-squared |
|-------|-----|-----------|
| Linear Regression | [Value from output] | [Value from output] |
| Polynomial Regression | [Value from output] | [Value from output] |

## 🔍 Key Insights

- **Study Hours Impact**: Direct relationship between study hours and exam performance
- **Model Comparison**: Polynomial regression may capture non-linear patterns better
- **Feature Importance**: Hours studied is a significant predictor of exam scores

## 📁 Project Structure

\`\`\`
student-performance-analysis/
│
├── README.md
├── requirements.txt
├── main.py                    # Main analysis script
├── StudentPerformanceFactors.csv
└── outputs/
    ├── correlation_heatmap.png
    ├── distribution_plots/
    └── regression_plots/
\`\`\`

## 🔧 Code Structure

### Data Loading and Exploration
```python
# Load and examine data
df = pd.read_csv('StudentPerformanceFactors.csv')
df.info()
df.describe()
