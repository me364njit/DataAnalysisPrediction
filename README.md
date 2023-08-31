# DataAnalysisPrediction

**Code Description: Exploring Affordable Housing Production Dataset**

**File: explore_housing_data.py**

This Python script focuses on exploring and analyzing a dataset related to affordable housing production. It utilizes the Pandas library for data manipulation, Seaborn for visualization, and the LabelEncoder from Scikit-learn for encoding categorical variables. The main goal is to gain insights into the dataset's content, distribution, correlations, and missing data.

**Step 1: Import Required Libraries**
- Import the necessary libraries: `pandas` for data handling, `seaborn` for visualization, and `LabelEncoder` from `sklearn.preprocessing` for encoding categorical variables.

**Step 2: Load the Dataset**
- Load the dataset named 'Affordable_Housing_Production_by_Building.csv' into a Pandas DataFrame named `data`.

**Step 3: Label Encoding for Borough Column**
- Apply `LabelEncoder` to the 'Borough' column to convert categorical borough names into numerical labels. The encoded values are stored in a new column named 'Borough_encoded'.

**Step 4: Summary Statistics of Numerical Features**
- Display the summary statistics of numerical features in the dataset using the `describe()` function. This provides information like mean, standard deviation, minimum, and maximum for each numerical column.

**Step 5: Distribution of Numerical Features**
- Create histograms to visualize the distribution of numerical features using the `hist()` function. This helps understand the data distribution and identify potential outliers.

**Step 6: Correlation Matrix Heatmap**
- Generate a correlation matrix using the `corr()` function to understand the relationships between numerical features. Visualize the correlation matrix as a heatmap using Seaborn's `heatmap()` function. Correlation values are displayed in the heatmap, indicating how features correlate with each other.

**Step 7: Missing Data Analysis**
- Check for missing data in the dataset using the `isna().sum()` function. This provides the count of missing values in each column.

**Step 8: Value Counts of Categorical Features**
- For each categorical feature (those of data type 'object'), calculate the value counts using a loop and the `value_counts()` function. This reveals the frequency of unique values in each categorical column.

**Step 9: Order Features Based on Correlation**
- Calculate the correlation between the encoded 'Borough' column and other features using the previously generated correlation matrix. Order the features based on their correlation with the target variable ('Borough_encoded'). The most correlated features are sorted in descending order of correlation strength.

**Step 10: Print Ordered Features**
- Print the ordered features list to the console. These features are ranked based on their correlation with the encoded 'Borough' variable.

**Conclusion:**
This Python script performs exploratory data analysis on an affordable housing production dataset. It handles data loading, preprocessing, visualization, correlation analysis, and identification of missing values. The code provides insights into the dataset's characteristics, distribution, and relationships among features.
