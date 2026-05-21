# E-Commerce Dataset Cleaning and Analysis using Pandas

This project focuses on cleaning and analyzing a raw e-commerce dataset downloaded from Kaggle using Python and the Pandas library. The complete work was performed in Jupyter Notebook/Google Colab as part of a data analysis and preprocessing project. 

The main objective of this project was to transform an unorganized raw dataset into a clean, structured, and analysis-ready CSV file. During the project, different data cleaning and exploratory data analysis (EDA) techniques were applied to improve the quality and usability of the dataset. 

The project started with importing the dataset into a Pandas DataFrame using `pd.read_csv()`. After loading the data, the dataset structure was explored by checking rows, columns, data types, and sample records using functions like `head()`, `tail()`, `shape`, and `info()`. 

Several important data cleaning operations were then performed. Missing values were identified using `isnull().sum()` and handled properly using `fillna()` and `dropna()`. Duplicate records were removed using `drop_duplicates()` to improve data accuracy and consistency. 

The project also involved filtering products based on customer ratings and selecting only the relevant columns needed for analysis. Unnecessary columns such as images, videos, seller information, delivery options, breadcrumbs, and product specifications were removed to make the dataset cleaner and more optimized. 

A new derived column called `total_amount` was created using the formula:

total_amount = final_price * ratings_count

This helped calculate the weighted revenue potential for each product. Data types were also converted where required, such as converting float values into integers using `astype(int)`. 

After completing all preprocessing and cleaning steps, the final cleaned dataset was exported and saved as `cleaned_csv.csv` using `to_csv()`. The final dataset contains structured and organized product information that can now be used for further data analysis, visualization, business insights, or machine learning tasks. 

Through this project, important skills were learned, including:

* Data cleaning using Pandas
* Handling missing values
* Removing duplicates
* Filtering and selecting data
* Feature engineering
* Working with CSV datasets
* Data preprocessing
* Exploratory Data Analysis (EDA)
* Using Jupyter Notebook and Google Colab


