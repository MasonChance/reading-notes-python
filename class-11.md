# Jupyter

we won't spend alot of time on jupyter notebooks/labs suffice to say it is a useful interface for working with various segements of code, files, notes, images and organizing them on your screen to improve workflow and collaboration.

# NumPy (said, nhum-pee?)

NumPy is a package for working with multi-dimensional arrays (matrices), full overview and tutorial can be found at [dataquest.io/blog](https://www.dataquest.io/blog/numpy-tutorial-python/). 

here I intend to touch on the very basics and provide a useful analogy for wrapping the brain around how nested lists or matrixes are processed. 
for the purpose of example we will use a 2-dimensional matrix. values are access by specifying row, and column just like coordinate pairs on a graph.
coords are always entered in the `(x, y)` format and matrices are accessed the same way using `(row, column)` additional dimensions are added using comma separated values.

Picture a spreadsheet with its rows and columns, now imagine that someone unstacked the rows and put them in-line with each other the begining of the next row placed after the value of the last column. If you are like me, and a physical visual representation of the shape of the data is more useful, consider having a hardcopy of the matrix where you "stack" all the inner arrays on top of each other, this is often how some .json data appears and can be very useful in orienting yourself.

now lets talk about the most common/basic Numpy methods. (dont forget to `import numpy`, and any other packages necessary for accessing the data you need)

- *numpy.array*: the function argument structure looks like this: `numpy.array(matrix['optional_range/slice'], dtype= 'data_type')`
    - standard array range and slice syntax may be used to select a specific subset of the data to be parsed

- *numpy_array.shape*: lets you check the number of rows and columns in a two dimensional array. more accurately it allows you to check the length of each dimension of the matrix it is called on. return looks like this: `(len_of_dim_1, len_of_dim_2,... len_of_dim_n) `

- *numpy.zeros* creates a matrix with a fixed length for a fixed number of dimensions `numpy.zeros((dim1, dim2...dimN))`

- *numpy.random.rand*: creates a matrix with fixed number and length of dimensions with random values assigned to each element

-*numpy.genfromtxt* is used to generate a matrix from a text file, specifying a filepath, delimiter and skip_header=block_to_be_excluded. 
  `numpy.genfromtxt('path', delimiter='char', skip_header='row_to_be_excluded')`

#### [Return to Main index of Notes](./README.md)