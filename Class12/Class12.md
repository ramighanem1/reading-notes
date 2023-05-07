# Pandas

Pandas is an open-source Python library that provides high-performance data manipulation and analysis tools. It is built on top of the NumPy library .
##  common operations :

* Data Loading:  read_csv(), read_excel(), read_sql()

* Data Cleaning:  dropna(), fillna(), drop_duplicates(), replace()

* Data Selection and Filtering:  loc , iloc 

* Data Transformation: apply(), groupby(), merge(), and join()

* Data Analysis and Statistics: describe(), mean(), sum(),  plot(),his() 

* Data Visualization:  You can generate line plots, bar plots, scatter plots, histograms, and more

# The primary data structures in Pandas

the Series and DataFrame. Both structures are designed to handle and manipulate data

the Series data structure is useful for working with a single variable or a sequence of data points, while the DataFrame data structure is designed for handling structured, tabular data with multiple variables. Choosing the appropriate data structure depends on the nature of the data and the specific analysis tasks at hand.


# Loading a dataset

Loading a dataset into a Pandas DataFrame involves a few steps, which include identifying the file format, selecting the appropriate Pandas function, specifying the file path or data source

## commonly used functions:

* read_csv(): Reads data from a CSV file and returns a DataFrame.
* read_excel(): Reads data from an Excel file and returns a DataFrame.
* read_sql(): Executes an SQL query against a SQL database and returns a DataFrame.
* read_json(): Reads data from a JSON file or API and returns a DataFrame.
* read_html(): Parses HTML tables from a web page and returns a list of DataFrames.


## example:

```
import pandas as pd

# Specify the file path
file_path = 'data.csv'

# Use read_csv() to load the data into a DataFrame
df = pd.read_csv(file_path)
```