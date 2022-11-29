# DBFoundations-Module07

**SQL Functions**

***Introduction***

SQL functions provide a way to refine data programmatically in an RDBMS. Most RDBMS contain built in functions for simple tasks like averaging counts, or more complicated tasks like LEAD() or LAG() where a new column gets generated based on the value in the current row and adjacent rows. In addition to pre-defined functions, an RDBMS will also allow users to create their own specific functions. These functions are fine tuned to the data, and can contain pre-defined functions within them.

***User Defined Functions***

User defined functions are objects stored in the database that perform an operation and return some kind of output (Drkusic, 2020). Storing functions in the database allows the function to be called without rewriting the code. This provides a way to share code within the database, and save time by not having to rewrite code. These objects can have permissions as well. User defined functions can return a range of objects, including a single integer, a column, or an entire table.

For example, if an IT department has a webpage of devices they manage, and each has a warranty with an expiration date. A function could be created that calculates the remaining time of the warranty displaying as a separate column. If the page is checked when a warranty expires, the device can be flagged as well as showing the time past expiration. This function could also be written to extend to software warranties,

***Scalar, Inline, and Multi-Statement Functions***

A scalar function takes one or multiple inputs, and returns a single value (_SQL Server Scalar Functions by Practical Examples_, n.d.). These functions cannot update data directly (_SQL Server Scalar Functions by Practical Examples_, n.d.). A scalar function can return a one result, like the sum of a column, or be applied to each row of a result, like calculating the net profit on individual products.

An Inline table-valued function returns a table of data based on a SELECT statement (Brown, 2013b). This function can take a set of parameters, apply it to a SELECT statement, and return the table based on the conditions. This is similar to a VIEW in execution, except a VIEW cannot accept parameters. This function can be used in a FROM clause (Erkec, 2019).

A multi-statement table-value function (MSTVF) is similar to an inline table-value function in that it returns a table, but an MSTVF includes additional processing on the table (Brown, 2013a). An MSTVF will return a new table with potentially new datatypes from the data it's pulling from.

***Conclusion***

Functions in SQL are powerful tools to analyze the data in a database. User defined functions provide the means for a person to fine-tune results for the task at hand. Scalar functions provide a way to do quick calculations on a table without needing to do it by hand. Both kinds of table-value functions, inline and multi-statement, allow complex table operations and new data to be generated.

**References**

Brown, A. (2013a, February). _Multi-Statement Table-Valued Functions_. Www.wiseowl.co.uk. https://www.wiseowl.co.uk/blog/s347/multi-statement.htm

Brown, A. (2013b, February 13). _Simple (in-line) table-valued functions_. Www.wiseowl.co.uk. https://www.wiseowl.co.uk/blog/s347/in-line.htm

Drkusic, E. (2020, February 25). _Learn SQL: User-Defined Functions_. SQL Shack - Articles about Database Auditing, Server Performance, Data Recovery, and More. https://www.sqlshack.com/learn-sql-user-defined-functions/

Erkec, E. (2019, August 29). _SQL Server inline table-valued functions_. SQL Shack - Articles about Database Auditing, Server Performance, Data Recovery, and More. https://www.sqlshack.com/sql-server-inline-table-valued-function/

rwestMSFT. (n.d.). _Create User-defined Functions (Database Engine) - SQL Server_. Learn.microsoft.com. Retrieved November 28, 2022, from https://learn.microsoft.com/en-us/sql/relational-databases/user-defined-functions/create-user-defined-functions-database-engine?view=sql-server-ver16

_SQL Server Scalar Functions By Practical Examples_. (n.d.). SQL Server Tutorial. https://www.sqlservertutorial.net/sql-server-user-defined-functions/sql-server-scalar-functions/

‌
