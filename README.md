Task 2 – Exploratory Data Analysis (EDA)

This project focuses on **Exploratory Data Analysis (EDA)** as part of the *Data Science Using Python Internship*.
EDA is the stage where raw, cleaned data is explored visually and statistically to uncover insights, patterns, correlations, and relationships among variables.
The dataset used for this task is **tested.csv**, which contains passenger information from the Titanic dataset — ideal for mixed data analysis (numerical and categorial.

The objective of this task is to analyze the dataset using statistical and visualization techniques to:

* Understand data structure, patterns, and relationships.
* Detect missing values, outliers, and feature imbalances.
* Identify correlations between variables.
* Derive meaningful insights that can support model building in later stages.
Importing Libraries
Libraries such as **pandas**, **numpy**, **matplotlib**, **seaborn**, and **scipy** were imported for data analysis, visualization, and statistical operations.
Loading and Inspecting Data
The dataset (`tested.csv`) was loaded using `pandas.read_csv()`.
Initial checks like `.shape`, `.info()`, and `.describe()` helped understand the data size, types, and distribution.
Handling Missing Values
Missing values were identified using `.isnull().sum()` and handled through:
Median imputation for numerical features (e.g., Age, Fare).
Mode imputation for categorical features (e.g., Embarked).
  This ensured the dataset was complete without dropping valuable records.
Removing Duplicates
Duplicate rows were detected using `.duplicated().sum()` and removed to avoid data redundancy.
Univariate Analysis

Histograms and Boxplots were plotted for numerical columns to visualize data distribution and outliers.
Countplots were used for categorical features such as gender and class to examine frequency patterns.

Bivariate and Correlation Analysis

Relationships between features were explored using:

  * `seaborn.heatmap()` for correlation matrices.
  * `pd.crosstab()` for categorical variable relationships.
Example findings:

  * Higher fares were associated with higher survival probability.
  * 1st class passengers had significantly better survival rates.

Outlier Detection

Outliers were detected using:

Boxplots to visualize extreme points.
Z-score method to numerically identify values beyond ±3 standard deviations.
Skewness and Kurtosis were calculated to assess data symmetry and peakedness.
These measures helped in identifying non-normal features that might need transformation before modeling.
Encoding and Saving

Categorical columns were encoded using `LabelEncoder` to prepare data for modeling.
The cleaned and analyzed dataset was saved as `tested_eda_processed.csv`.


Outcome

This task provided a clear understanding of how to analyze, visualize, and interpret structured datasets using Python.
The insights gained formed the foundation for predictive modeling and decision-making in subsequent stages of the internship.
The EDA process successfully transformed raw data into meaningful information that drives further analysis.
