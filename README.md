# Elevatelabs_Day1Task
Gain hands-on experience in identifying and fixing common data issues like missing values, duplicates, and inconsistent formatting. Learn to use Excel functions or Pandas in Python for real-world data cleaning, understanding of data pre-processing, which is a critical step before data analysis or visualization.
1. Text to Columns
The dataset was originally tab-separated.
Used Excel’s “Text to Columns” tool to split columns correctly.

2. Renaming Columns
Renamed columns for clarity. For example:
YEAR_BIRTH ➝ birth_year
MntWines ➝ wine_spend and etc for other columns also.

All column names were converted to lowercase using the =LOWER() function in a new row, then pasted back as values.

3. Removing Duplicates
Removed duplicate entries using Excel's “Remove Duplicates” feature.

4. Handling Missing Values
Identified 24 missing values in the Income column.

Filled them using the median value:
replace missing values with MEDIAN.
=MEDIAN(range)

5. Correcting Data Types
Checked and fixed data types using Power Query:
Converted dt_time to date format (dd-mm-yyyy).

6. Text Formatting
Standardized values in Education and Marital_Status columns to lowercase using Flash Fill for convenience.

7. Feature Engineering
Added several new columns:
age = YEAR(TODAY()) - birth_year
total_child = kidhome + teenhome
total_spend = sum of all product spending columns
total_purchases = sum of all purchase-related columns

8. Dropping Irrelevant Columns
Removed z_costcontact and z_revenue as they contained identical values for all rows.

Tools Used
Microsoft Excel
Text to Columns
Remove Duplicates
Flash Fill
Power Query
Formulas: =LOWER(), =MEDIAN(), =YEAR(), =TODAY(), SUM()