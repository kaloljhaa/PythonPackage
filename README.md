# Python Package : Pandas
In computer programming, **Pandas** is a software library written for the Python programming language for data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series
### Key Features
  1. Fast and efficient DataFrame object with the default and customized indexing.
  2. Tools for loading data into in-memory data objects from different file formats.
  3. Data alignment and integrated handling of missing data.
  4. Reshaping and pivoting of data sets.
  5. Label-based slicing, indexing, and subsetting of large data sets.
  6. Columns from a data structure can be deleted or inserted.
  7. Group by data for aggregation and transformations.
  8. High-performance merging and joining of data.
  9. Time Series functionality.
# Install and Run Instructions
1. Check to see if Python is downloaded by running the command:
   - python --version
   - If Python is already installed, it will generate a message with the Python version available.
2. Next, use a PIP command to install Pandas. PIP is a package management system used to install and manage software packages/libraries written in Python. 
   - To install Pandas on Windows, use the command 
      - pip install pandas
   - To install Pandas on Linux (OSX), open the Terminal Window (Commad+spacebar) and type the following command
      - $ python -m pip install pandas
3. Press enter and Linux will automatically download and install the packages/files required to run Pandas in Python
4. To import Pandas all you have to do is run the following code: 
    - import pandas as PD
    - import NumPy as np 
# Code
Open a remote file or database like a CSV or a JSONon a website through a URL or read from a SQL table/database to retrieve a dataset.
```
import pandas as pd
url = "https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data"
columns = ["age", "work-class", "fnlwgt", "education", "education-num", "marital-status", "occupation", "relationship", "race", "sex", "capital-gain", "capital loss", "hours-per-week", "native-country", "income"]
data = pd.read_csv(url, names=columns, sep = ",", na_values = "?", skipinitialspace = True)
data.head()
```
This code shows the dataset for a census. By using the data.head () function of pandas, it shows the first 5 rows of the dataset. Changing this function to another function, such as data.describe or data.info will change the output of the code. For instance, data.describe will produce the numerical attributes such as age, FnlWgt, education-num, capital-gain, capital-loss, and hours-per-week. Pandas has numerous functions that will all provide a different output and a new perspective on the data.
