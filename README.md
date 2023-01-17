# Data-Analysis-with-Python-NumPy-Pandas-Masterclass
Detailed Study of Data Analysis with Pandas and Numpy.

**CONTENTS AND TOPICS**

# Section 1 : Get Started.
# Section 2 : Numpy Primer.
## Numpy Arrays and Array Properties.
   A numpy array is a grid of values, all of the same type, and is indexed by a tuple of nonnegative integers. The number of dimensions is the rank of the array; the shape of an array is a tuple of integers giving the size of the array along each dimension.
## Array Creation.
    ```python
    import numpy as np
    a = np.array([1,2,3])# Create a rank 1 array
    print(type(a))       # Prints "<class 'numpy.ndarray'>"
    print(a.shape)       # Prints "(3,)"
    print(a[0], a[1], a[2])# Prints "1 2 3"
    a[0] = 5                # Change an element of the array
    print(a)                # Prints "[5, 2, 3]"
    b = np.array([[1,2,3],[4,5,6]])  # Create a rank 2 array
    print(b.shape)                   # Prints "(2, 3)"
    print(b[0, 0], b[0, 1], b[1, 0])# Prints "1 2 4"
    ```
## Indexing and Slicing.
## Array Operations.
## Filtering and Modifying Array Values.
## The Where Function. `np.where(array_condition, values if True, value if False)`
## Array Aggregations.
## Array Functions.
## Array Sorting.
## Vectorization and BroadCasting Concepts

# Section 3 : Pandas Series.
## Pandas Series Basics.
## Series Index and Custom Indices.
## Filtering Series, Logical Tests and Sorting Series.
## Numerical and text Series Operations
## Numerical and Categorical Series Aggregations.
## Missing Values and handling them.
## Applying Custom functions and .where() method

# Section 4 : Introduction to DataFrames.
## Dataframe Basics, Creating a Dataframe.
## Explore the Dataframe.
## Accessing the Dataframe Columns and Rows.
## Dropping rows and columns, and duplicates rows.
### `data.drop()`
### `data.drop_duplicates(subset = "column")`
## Handling the Missing Data.
### Checking the Missing Values, `data.isna().sum()`
### Fill the missing values, `data.fillna(value)`
## Filtering the Dataframe.
### `We can filter using the Different Masks that are applied in Series and numpy Arrays.`
### `We can use the .query method to do the filtering.`
## Sorting Dataframes.
### We can sort by Index using `.sort_index()`
### We can sort by Values using `.sort_values()`
## Renaming and Reordering Columns.
### `df.columns = ["column1","column2","column3"]` or `df.rename(columns = {"column1":"column_one","column2":"column_two"})`
### `.reindex` or `data.reindex(labels = ["column1","column2',"column3"], axis = 1)`
## Arithmetic and Boolean Column Creation.
### You can create Columns using Arithemtic Operations.
### You can create a Boolean Column by assigning them a Logical Test.
### Numpy's `.select` method lets you put different condition to create columns.
## Mapping Values to Columns, Creating new Columns with `.assign` method.
### Mapping Method - `.map()`

# Categorical Data Types:

Categorical data is a type of data that can be divided into groups or categories. In Python, the pandas library has a Categorical data type that can be used to represent categorical variables. Here's an example of how to create a categorical variable in a pandas DataFrame:

```python
import pandas as pd

# Create a dataframe
df = pd.DataFrame({'animal': ['cat', 'dog', 'bird', 'cat', 'dog', 'bird']})

# Convert the 'animal' column to a categorical data type
df['animal'] = pd.Categorical(df['animal'])

```
# Type Conversion:
In Python, variables can be converted from one data type to another using type conversion functions. For example, the int() function can be used to convert a variable to an integer, and the str() function can be used to convert a variable to a string. Here's an example of converting a variable from a float to an integer:

```python
x = 3.14
y = int(x)
print(y) # Output: 3
```
# Memory Usage and Data Types:

Different data types use different amounts of memory. For example, an integer variable uses less memory than a float variable. In Python, the sys module has a getsizeof() function that can be used to check the memory usage of a variable. Here's an example of checking the memory usage of an integer and a float variable:

```python
import sys

x = 5
y = 3.14

print(sys.getsizeof(x)) # Output: 28
print(sys.getsizeof(y)) # Output: 24
```

# Downcasting Numeric Data Types:

This is the process of converting a data type of higher precision to a data type of lower precision. For example, float64 to int32. In pandas, we can use the astype() method to downcast the data types. Here's an example of downcasting float64 to int32:

```python
import pandas as pd

# Create a dataframe
df = pd.DataFrame({'number': [1.23, 2.45, 3.67, 4.89]})

# Downcast float64 to int32
df['number'] = df['number'].astype('int32')

```
