Data cleaning is the process of detecting and correcting (or removing) corrupt or inaccurate records from a dataset. The primary goal is to improve the quality of the data by addressing issues such as missing values, duplicates, outliers, and errors, thereby making the dataset more suitable for analysis.

**Steps Involved:**

**1. Importing Libraries and Data:**

•	Import Pandas library using import pandas as pd.

•	Load your data using **pd.read_csv("your_file.csv")** for CSV files (adjust for other file formats, excel..). This creates a Pandas DataFrame object.

**2. Exploring the Data:**

•	Use **df.head()** and **df.tail()** to view the first and last few rows.

•	Get basic information about the data using **df.info()**.

•	Check for missing values using **df.isnull().sum()**.

**3. Handling Missing Values:**

•	Drop rows with missing values using **df.dropna()**.
**
•	Impute missing values with statistical methods (e.g., df.fillna(df.mean())) or custom logic.

**4. Removing Duplicates:**

•	Identify and remove duplicate rows using **df.drop_duplicates()**.

**5. Renaming Columns :**

•	Rename columns to more meaningful names **df.rename(columns= {‘old name’: ‘new name’})**

**6. Cleaning Specific Columns:**

•	Formatting: Use string methods like **df['column_name'].str.strip()** to remove leading/trailing spaces.

•	Replace unwanted characters/values using **df['column_name'].str.replace().**

•	Working with regex

•	Converting data types: Use **df['column_name'] = pd.to_numeric(df['column_name'])** to convert strings to numeric data types.

**7. Saving the Cleaned Data:**

•	Save the cleaned DataFrame to a new file using **df.to_csv("cleaned_data.csv")**.

