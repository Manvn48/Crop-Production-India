# Crop Production Analysis and Prediction

## Table of Contents
- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Cleaning and Preprocessing](#data-cleaning-and-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Visualization](#data-visualization)
- [Predictive Modeling](#predictive-modeling)
  - [Linear Regression](#linear-regression)
  - [Random Forest Regressor](#random-forest-regressor)
  - [Decision Tree Regressor](#decision-tree-regressor)
  - [XGBoost Regressor](#xgboost-regressor)
- [Model Evaluation](#model-evaluation)
- [Conclusion](#conclusion)
- [Technical Skills and Tools](#technical-skills-and-tools)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project involves a comprehensive analysis of crop production data from various states in India. The primary objective is to uncover key trends and insights and build predictive models to forecast crop production. The project utilizes various data analysis and machine learning techniques to achieve these goals.

## Dataset
The dataset contains crop production details from different states and districts in India over multiple years. It includes the following columns:
- `State_Name`
- `District_Name`
- `Crop_Year`
- `Season`
- `Crop`
- `Area`
- `Production`

## Data Cleaning and Preprocessing
The initial dataset contained 246,091 records with some missing values in the `Production` column. Key steps in data cleaning included:
- Dropping rows with null values in the `Production` column.
- Removing records where `Production` was zero.
- Handling duplicate records.

## Exploratory Data Analysis (EDA)
EDA was performed to understand the distribution of data and uncover patterns and trends. Key analyses included:
- Year-wise distribution of crop production.
- Correlation analysis between different features.
- State-wise and season-wise crop production trends.

## Data Visualization
Data visualization played a crucial role in this project. Key visualizations include:
- Heatmaps to analyze feature correlations.
- Bar plots showing the number of crops by state.
- Line plots depicting production trends over the years.
- Interactive visualizations using Plotly Express for state-wise production analysis.

## Predictive Modeling
Several machine learning models were developed to predict crop production:

### Linear Regression
A basic linear regression model was implemented, but it did not perform well, achieving an R2 score of 0.156.

### Random Forest Regressor
A Random Forest model was implemented, significantly improving the performance with an R2 score of 0.689.

### Decision Tree Regressor
A Decision Tree Regressor was also used, yielding similar results to the Random Forest with an R2 score of 0.689.

### XGBoost Regressor
The best performance was achieved with the XGBoost Regressor, which obtained an R2 score of 0.776, making it the optimal model for this dataset.

## Model Evaluation
The models were evaluated using Mean Squared Error (MSE) and R2 score. The XGBoost model outperformed others, demonstrating its robustness in handling the dataset's complexity.

## Conclusion
This project provided valuable insights into crop production trends across India and successfully developed predictive models to forecast production. The XGBoost Regressor was identified as the most effective model.

## Technical Skills and Tools
- **Programming Languages:** Python
- **Libraries and Tools:** Pandas, NumPy, Seaborn, Matplotlib, Plotly Express, Scikit-Learn, XGBoost
- **Data Processing:** Data Cleaning, Data Wrangling, Feature Engineering, Data Transformation
- **Machine Learning:** Linear Regression, Random Forest, Decision Tree, XGBoost
- **Visualization:** Interactive and static data visualizations, Heatmaps, Bar plots, Line plots
- **Evaluation Metrics:** R2 Score, Mean Squared Error (MSE)
