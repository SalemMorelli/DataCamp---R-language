Exercises and notes from DataCamp on the R language for data modelling.

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
### Extract value of consecutive cells in a column
So far, you have learned to extract the value of a single row in a column. Now you will learn to extract data in a sequence of rows for the given column.

We use the colon operator, :, in R to specify the first and last number of the sequence. For example, to extract the first ten values in the column Date in data_maruti, simply run this code:

data_maruti$Date[1:10]
Run the code in the console and check the results!

Which of the following codes will extract the closing prices in rows 100 to 110? The data_maruti data frame is already available in the workspace. The name of column of closing prices is Close.

## Exercise 5
### Function c()
The function c() is one of the most useful functions in R. It is used to create a new vector that can be saved as a new column in a data frame.

We can use the c() function in different ways. Check out the syntaxes below for creating a vector with values 1, 2, 3, 4 and 5:

Give all the values as arguments: c(1, 2, 3, 4, 5).
To create a vector of consecutive integers, use the colon operator: c(1:5).
In this exercise, you will learn to create vectors and run basic arithmetic operations on them.
