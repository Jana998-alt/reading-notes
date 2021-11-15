# Pandas

## Pandas - Getting Started
(from the [documentation](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html))

pandas is a Python package that provides data structures designed to make working with “relational” or “labeled” data both easy and intuitive. It aims to be the fundamental high-level building block for doing practical, real-world data analysis in Python.

A DataFrame is a 2-dimensional data structure that can store data of different types (including characters, integers, floating point values, categorical data and more) in columns. It is similar to a spreadsheet, a SQL table or the data.frame in R.

Each column in a DataFrame is a Series, and can be displayed like this: ``` df["col "] `label``

## What is Pandas? Why and How to Use Pandas in Python 
(from [this youtube video](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s))

a package to manipulate data based of the idea of _data frame_. 

methods to use on data-frames:
- df.describe()  -> tell basic statistics about the df
- df.value_counts()  -> the number of certain data in df
- df.groupby()  -> groups data depending on a certain criteria.
- df.plot()  -> for plotting data, and it has many arguments to customize the graph as you want.