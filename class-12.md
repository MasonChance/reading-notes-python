# Pandas

Pandas is a data analysis/manipulation library that leverages NumPy to quickly and easily sort, examine and manage large data-sets including easy built-in methods for converting real and relational data to visual form. 

the base structure for pandas is the use of a dataframe the convention for identifying variables that are dataframes is to include `df` in the variable name. wehn creating a dataframe pandas will automatically index the values entered and rows and columns can be labeled. unlike NumPy, pandas dataframes can contain multiple datatypes; each column can have a diferent datatype. objects, lists, numpyArrays, dictionarys etc may all be passed into the creation of a dataframe. 

Pandas is Extensive and thus we will not go into detail here, but below are the conventional imports and basic method call signatures to get started

```import numpy as np
   import pandas as pd
```
Creating a data frame in pandas follows the function signature below:

```
  class pandas.DataFrame(data=None, index=None, columns=None, dtype=None, copy=False) 
    # data: required arguement- this is the data that will be converted into a pandas dataframe
    # index: defaults to RangeIndex if no alternate is specified or if no indexing is inherrent to the input data
    # column: defaults to RangeIndex, to label columns pass in a list of column labels as the argument
    # dtype: defaults to infer based on input. can be forced
    # copy: only affects 2 dimensional ndarray input

```

for a comprehensive look at dataframes and their construction please reference [Pandas-Docs-dataframe](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html#pandas.DataFrame)






#### [Return to Main index of Notes](./README.md)