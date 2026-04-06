ex-14
Nikunj Deep Upadhyay
ENTC B1
25070123081

THEORY
1. Data Binning (Discretization)

Data binning is a preprocessing technique used to convert continuous numerical data into categorical data. It groups values into intervals called bins.

Key Points:
Helps in data analysis and visualization
Reduces noise in data
Converts numerical values into meaningful categories (Low, Medium, High)
In your code:
Price, Units Sold, Order Value, Delivery Time, and Distance are divided into categories using pd.cut()

Example:

Price → Low (0–10000), Medium (10000–30000), High (30000–60000)
2. Data Formatting

Data formatting ensures that the dataset is clean, consistent, and in the correct structure.

Operations used:
a) Data Type Conversion
Converts column data types (e.g., int → float)
Done using .astype()
Useful for calculations and analysis
b) String Operations
Convert text to uppercase using .str.upper()
Ensures uniformity in text data
c) Rounding Values
Used to control decimal precision
Done using .round()
3. Sorting Data

Sorting arranges data in ascending or descending order.

Types:
Ascending (default)
Descending (ascending=False)
Uses:
Helps in ranking
Easier data analysis
4. Unique Values
Used to identify distinct categories in a column
Done using .unique()

ALGORITHM

Algorithm for Data Binning
Start
Import pandas and numpy libraries
Create dataset using dictionary
Convert dictionary into DataFrame
Define bin ranges (e.g., bins = [0,10000,30000,60000])
Define labels (Low, Medium, High)
Apply pd.cut() to create categories
Store result in new column
Display updated DataFrame
Stop

Algorithm for Data Formatting
Start
Load dataset into DataFrame
Check data types using .dtypes
Convert required column using .astype()
Apply string formatting using .str.upper()
Round values using .round()
Display updated dataset
Stop

Algorithm for Sorting Data
Start
Load dataset
Choose column to sort (e.g., Price)
Apply .sort_values()
For ascending → default
For descending → ascending=False
Store or update DataFrame
Display sorted data
Stop

Algorithm for Finding Unique Values
Start
Select column
Apply .unique()
Display unique values
Stop

Algorithm for Multiple Binning (Order Dataset)
Start
Create DataFrame (Order data)
Define bins for:
Order Value
Delivery Time
Distance
Define labels for each
Apply pd.cut() for each column
Create new categorical columns
Display final DataFrame
Stop
