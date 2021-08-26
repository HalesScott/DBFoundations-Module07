Evan Hales
8/25/2021
IT FDN 130 A: Foundations of Databases & SQL Programming
Assignment07: Functions

# Fun with Functions!

## Introduction
This document will provide information regarding when to use an SQL UDF as well as the differences between Scalar, Inline and Multi-Statement Functions.

**_Explain when you would use an SQL UDF._**
One would create a User Defined Function (UDF) when they want to return data they can’t call on using SQL’s built-in functions.  A good example of this is creating a UDF to perform a complex calculation in order to return a single (scalar) value or an entire result set.  UDF’s can also be used as check constraints because you cannot otherwise reference a column in another table. (Course note, RRoot, 2021).

**_What are the differences between Scalar, Inline and Multi-Statement Functions._**
For starters, Scalar functions return a single value as an expression where Inline and MSF’s will return a table of data.  While inline and multi-statement functions both return tables as their result, inline functions include only a single SELECT statement while, MSF’s allow multiple select statements.  MSF’s also include a table variable that stores the rows that are returned as the value of the function.  Lastly, the definition of the RETURNS TABLE for inline functions is based on the SELECT statement vs MSF’s where the RETURNS syntax explicitly specifies the structure of the returned table.

## Summary
This document provided information regarding when to use an SQL UDF as well as the differences between Scalar, Inline and Multi-Statement Functions.
