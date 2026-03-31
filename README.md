# Project 7: Titanic Preprocessing Project

This notebook demonstrates a complete data preprocessing pipeline for the Titanic dataset. The goal is to prepare the raw data for machine learning model training.

## Steps Performed:

1.  **Import Required Libraries**: Essential libraries like pandas, numpy, sklearn's `train_test_split`, `LabelEncoder`, `StandardScaler`, and `MinMaxScaler` are imported.

2.  **Load The CSV File From GITHUB**: The Titanic dataset is loaded into a pandas DataFrame from a provided CSV string.

3.  **Display First 5 Rows**: A quick look at the initial rows of the dataset to understand its structure.

4.  **Check The Shape of The DATASET**: Determine the number of rows and columns in the dataset.

5.  **Check The Column Names of The Dataset**: List all column names to identify available features.

6.  **Check The Basic Information About The Dataset**: Review data types, non-null counts, and memory usage for initial insights into data quality.

7.  **Check Missing Values**: Identify columns with missing data and the extent of those missing values.

8.  **Drop Unnecessary Columns**: Columns such as 'Cabin', 'Name', 'Ticket', and 'PassengerId' are removed due to high missing values or irrelevance for a basic model.

9.  **Handle Missing Values**: Missing 'Age' values are imputed with the median, and missing 'Embarked' values are filled with the mode.

10. **Separate Features (X) and Target (Y)**: The dataset is split into independent features (X) and the target variable (y), 'Survived'.

11. **Apply One-Hot Encoding To Categorical Input Columns**: Categorical features like 'Sex' and 'Embarked' are converted into numerical format using one-hot encoding to make them suitable for machine learning algorithms.

12. **Apply Label Encoding To The Target Column**: The 'Survived' target variable is label-encoded, converting its values into numerical representations (though often already 0/1).

13. **Split Data Into Training And Testing Sets**: The dataset is divided into training and testing sets to evaluate model performance fairly.

14. **Apply Standardization**: Numerical features in the training and testing sets are standardized using `StandardScaler`, ensuring they have a mean of 0 and a standard deviation of 1.

15. **Apply Normalization**: Numerical features are also normalized using `MinMaxScaler`, scaling them to a range between 0 and 1.

16. **Final Summary**: A conclusive message indicating the successful completion of the preprocessing steps.
