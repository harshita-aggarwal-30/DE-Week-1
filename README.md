1.Overview:
This report presents a summary of the data analysis project completed as part of the internship/training program. The project involved collecting a raw e-commerce product dataset, performing systematic data cleaning operations, and producing a structured, analysis-ready CSV file using Python and Pandas in a Jupyter Notebook environment.
The work demonstrates practical skills in data handling, preprocessing, and exploratory data analysis (EDA) — core competencies in the field of data science and analytics.

 2.Project Details:
Field	                      Details
Project Title             	E-Commerce Dataset Cleaning & Analysis
Tools Used                 	Python 3, Pandas, Jupyter Notebook, Google Colab
Dataset Source	            Combined e-commerce product dataset (Combined_dataset.csv)
Output File	                cleaned_csv.csv
Dataset Size	              1,000 records across 11 columns
Currency	                  INR (Indian Rupee)
Total Categories	          97 product categories

3.Work Performed in Jupyter Notebook:
The Jupyter Notebook (jupyter_nb.ipynb) contains the complete, step-by-step data cleaning and analysis pipeline. The following tasks were completed:
Step 1 — Data Loading
•	Imported the raw CSV file into a Pandas DataFrame using pd.read_csv().
Step 2 — Data Exploration (EDA)
•	Inspected the first and last few rows using head() and tail().
•	Checked the shape, column names, and data types of the dataset.
Step 3 — Handling Missing Values
•	Identified null/missing values using isnull().sum() and info().
•	Applied fillna() and dropna() to handle incomplete records.
•	Note: 121 records had missing discount values; these were handled appropriately.
Step 4 — Filtering & Column Selection
•	Filtered products with a customer rating of 3.8 or above.
•	Selected only relevant columns for the final output.
Step 5 — Removing Duplicates
•	Applied drop_duplicates() to remove any repeated product entries.
Step 6 — Creating a Derived Column
•	Computed a new column total_amount = final_price x ratings_count to represent weighted revenue potential per product.
•	Converted final_price and ratings_count to integer type for accurate calculation.
Step 7 — Dropping Irrelevant Columns
•	Removed non-essential columns: delivery_options, product_details, breadcrumbs, product_specifications, amount_of_stars.
Step 8 — Exporting the Cleaned Data
•	Saved the final cleaned dataset as cleaned_csv.csv using to_csv().
•	Downloaded the file from Google Colab for submission.

4.. Final Dataset Summary (cleaned_csv.csv):
Column Descriptions:-
Column Name	                 Data Type	                          Description
product_id	                  Integer	                            Unique identifier for each product
title                        	Text	                              Product/brand name
product_description	          Text                              	Short description of the product
quantity	                    Integer                           	Stock quantity available
ratings_count	                Integer                            	Number of customer ratings received
initial_price	                Integer                           	Original price before discount (INR)
discount	                    Float                             	Discount percentage applied
final_price                 	Integer                            	Selling price after discount (INR)
currency	                    Text	                              Currency (all records: INR)
category	                    Text	                              Product category (e.g., tops, jeans, watches)
total_amount	                Integer                           	Derived column: final_price x ratings_count

5.Skills Demonstrated:
This project showcases the following technical and analytical competencies:
1.	Data Ingestion — Loading and inspecting large CSV datasets using Pandas.
2.	Exploratory Data Analysis (EDA) — Understanding dataset structure, shape, types, and distributions.
3.	Data Cleaning — Handling null values, removing duplicates, fixing data types.
4.	Feature Engineering — Creating new meaningful columns (total_amount) from existing data.
5.	Data Filtering & Selection — Applying condition-based filtering and selecting relevant columns.
6.	Data Export — Saving clean, structured data for downstream analysis or reporting.
7.	Python & Pandas Proficiency — Writing clean, readable data processing code.
8.	Google Colab Environment — Working in a cloud-based Jupyter Notebook setup.
   

