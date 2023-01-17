# Data-Analysis-with-Python-NumPy-Pandas-Masterclass
Detailed Study of Data Analysis with Pandas and Numpy.

**CONTENTS AND TOPICS**

+ Section 1 : Get Started.
+ Section 2 : Numpy Primer.
    + Numpy Arrays and Array Properties.
    + Array Creation.
    + Indexing and Slicing.
    + Array Operations.
    + Filtering and Modifying Array Values.
    + The Where Function. `np.where(array_condition, values if True, value if False)`
    + Array Aggregations.
    + Array Functions.
    + Array Sorting.
    + Vectorization and BroadCasting Concepts
    
+ Section 3 : Pandas Series.
    + Pandas Series Basics.
    + Series Index and Custom Indices.
    + Filtering Series, Logical Tests and Sorting Series.
    + Numerical and text Series Operations
    + Numerical and Categorical Series Aggregations.
    + Missing Values and handling them.
    + Applying Custom functions and .where() method
    
+ Section 4 : Introduction to DataFrames.
    + Dataframe Basics, Creating a Dataframe.
    + Explore the Dataframe.
    + Accessing the Dataframe Columns and Rows.
    + Dropping rows and columns, and duplicates rows.  
         + `data.drop()`
         + `data.drop_duplicates(subset = "column")`
    + Handling the Missing Data.
        + Checking the Missing Values, `data.isna().sum()`
        + Fill the missing values, `data.fillna(value)`
    + Filtering the Dataframe. 
        + `We can filter using the Different Masks that are applied in Series and numpy Arrays.`
        + `We can use the .query method to do the filtering.`
    + Sorting Dataframes.
        + We can sort by Index using `.sort_index()`
        + We can sort by Values using `.sort_values()`
    + Renaming and Reordering Columns.
        + `df.columns = ["column1","column2","column3"]` or `df.rename(columns = {"column1":"column_one","column2":"column_two"})`
        + `.reindex` or `data.reindex(labels = ["column1","column2',"column3"], axis = 1)`
    + Arithmetic and Boolean Column Creation.
        + You can create Columns using Arithemtic Operations.
        + You can create a Boolean Column by assigning them a Logical Test.
        + Numpy's `.select` method lets you put different condition to create columns.
    + Mapping Values to Columns, Creating new Columns with `.assign` method.
        + Mapping Method - `.map()`

+ Section 5 : Aggregating and Reshaping Dataframes.

    + Basic Aggregation and Groupby methods.
        + `df.groupby(["column1","column2"])[["column"]]`
