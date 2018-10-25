# DataCamp---R-language
Exercises and notes from DataCamp on the R language for financial modelling.

# Chapter 1
## Exercise 2
### Types, Classes and Dimensions of Objects in R
Every variable in R is an object which has its own type, class and dimension. There are only few basic types of variables such as numeric (e.g. 5 or 5.0), character (e.g. "a") and logical (e.g TRUE). The dimensions are the number of rows and columns of the object. Finally, the class of an object can alter the behavior of the same functions. For example, the print() function will behave differently for a variable that is a data frame as compared to a variable that is a linear model.

The classes of objects that we work with in this chapter are vectors and data frames. Data frames, as pointed out earlier, are like excel tables which are most commonly used in financial computing. Vectors are like a single row or column of data consisting of same type of variables. In other words, a data frame is comprised of vectors.

## Exercise 3
### Extract data frame cell value
While working with tables you need to be able to select a specific data value from any row or column.

Recall that in Microsoft Excel, you can select a cell by specifying its location in the spreadsheet. For example, cell A1 represents column A and row 1. In data frames in R, the location of a cell is specified by row and column numbers.

Check out the different syntaxes which can be used for extracting data:

Extract value of a single cell: df_name[x, y], where x is the row number and y is the column number of a data frame called df_name.
Extract the entire row: df_name[x, ], where x is the row number. By not specifying the column number, we automatically choose all the columns for row x.
Extract the entire column: df_name[, y] where y is the column number. By not specifying the row number, we automatically choose all the rows for column y.
Another way to extract data from df_name is by using the dollar sign in combination with the column names:

df_name$colname refers to the entire column col_name in df_name data frame.
df_name$colname[x] refers to row x of column colname in data frame df_name.
Which of the following lines will give you the correct value of the closing price in the 100th row of data_maruti? The data_maruti data frame is already available in the workspace. The name of the column containing closing prices is Close.

## Exercise 4
