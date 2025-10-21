Task 2 – Exploratory Data Analysis (EDA)

This task involves Exploratory Data Analysis (EDA) as part of the Data Science Using Python Internship.
EDA is the process of examining raw and cleaned data both visually and statistically to discover patterns, trends, correlations, and relationships among variables.

The dataset used for this analysis is tested.csv, which contains Titanic passenger information. This dataset is suitable for analyzing both numerical and categorical features.

Objective

The main objectives of this EDA task are to:

Understand the overall structure of the dataset and variable patterns.

Identify missing values, outliers, and imbalances in features.

Examine correlations between different variables.

Extract meaningful insights to support subsequent predictive modeling.

Importing Libraries

Python libraries such as pandas, numpy, matplotlib, seaborn, and scipy were imported to perform data manipulation, statistical analysis, and visualizations.

Loading and Inspecting Data

The dataset (tested.csv) was loaded using pandas.read_csv().
Initial inspection with .shape, .info(), and .describe() helped to understand the dataset size, data types, and feature distributions.

Handling Missing Values

Missing values were identified using .isnull().sum() and addressed as follows:

Numerical features (e.g., Age, Fare) were filled with median values.

Categorical features (e.g., Embarked) were filled with the mode.

This approach ensured completeness of the dataset without losing important records.

Removing Duplicates

Duplicate records were checked using .duplicated().sum() and removed to prevent redundancy and maintain data integrity.

Univariate Analysis

Histograms and boxplots were plotted for numerical columns to observe distributions and detect outliers.

Countplots were used for categorical variables like Gender and Passenger Class to examine their frequency patterns.

Bivariate and Correlation Analysis

Feature relationships were explored through:

Correlation Heatmaps (seaborn.heatmap) to examine linear relationships among numerical variables.

Cross-tabulations (pd.crosstab) to analyze relationships between categorical features.

Key observations:

Higher fares were often associated with increased survival probability.

Passengers in 1st class had a significantly higher survival rate.

Outlier Detection

Outliers were identified using:

Boxplots to visualize extreme data points.

Z-score method to numerically detect values beyond ±3 standard deviations.

Additionally, skewness and kurtosis were calculated to assess the symmetry and peakedness of the data distributions, highlighting features that may require transformation before modeling.

Encoding and Saving

Categorical features were encoded using LabelEncoder to prepare the dataset for machine learning models.
The cleaned and processed dataset was saved as tested_eda_processed.csv.

Outcome

This EDA task provided a comprehensive understanding of the dataset through statistical and visual exploration.
The insights gained form a strong foundation for predictive modeling and informed decision-making in the next stages of the internship.
Overall, the process successfully transformed raw data into structured and actionable information for further analysis.
