# Medical Cost Prediction

This project focuses on analyzing and predicting medical costs based on various features such as age, sex, BMI, number of children, smoking habits, and the region of residence.

## Dataset Overview

The dataset used in this project is provided in the file `insurance.csv` and contains the following columns:

- **age**: Age of the individual.
- **sex**: Gender of the individual (male/female).
- **bmi**: Body mass index of the individual.
- **children**: Number of children or dependents the individual has.
- **smoker**: Whether the individual is a smoker (yes/no).
- **region**: The region the individual resides in.
- **charges**: The medical charges incurred by the individual.

## Objective

The main objective of this project is to analyze the dataset and predict medical costs (`charges`) based on other factors like age, gender, BMI, smoking habits, and region.

## Key Steps

1. **Data Loading**: The dataset is loaded into a Pandas DataFrame using `pd.read_csv("insurance.csv")`.

2. **Data Inspection**: The dataset is inspected using `df.info()` and `df.describe()` to understand the structure and summary statistics of the data.

3. **Data Preprocessing**:
   - Numerical columns and categorical columns are identified separately for further analysis.
   - Outliers are identified and handled appropriately.
   - Categorical variables such as `sex`, `smoker`, and `region` are encoded for use in machine learning models.

4. **Data Visualization**:
   - Boxplots, histograms, and pairplots are used to explore the relationships between the features and the target variable (`charges`).
   - Correlation heatmaps are plotted to understand how numerical features relate to each other.

5. **Modeling**:
   - A regression model is built to predict medical charges using the available features.
   - The model is evaluated using appropriate metrics (e.g., Mean Absolute Error, R-squared, etc.).

6. **Conclusion**:
   - The model's performance is analyzed, and insights are drawn regarding the factors that most influence medical costs.

## Libraries Used

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Matplotlib**: For data visualization.
- **Seaborn**: For advanced visualization and statistical analysis.
- **Scikit-learn**: For machine learning model building and evaluation.

## Setup

To run this project locally, you will need to install the following Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
