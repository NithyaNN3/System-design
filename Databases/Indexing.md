### Indexing

## What are Indexes?
- Way to optimize query performance on a database by speeding up the way we fetch regularly used columns
- Data organized in the indexes columns in a way that makes fetching data easy
- Accommodates growth of a dataset as the query performance isn't compromised

## Types of Indexes
1) Clustered Indexes - A database can have only one of these (the primary key). Data is physically ordered according to the indexed column.
2) Non clustered indexes - references the data in a table with pointers from a different structure that maintains the indexed columns. Data isn't physically ordered here. A table can have multiple non-clustered indexes which allows for querying on different columns or combinations of columns.
3) Unique indexes - enforces uniqueness in the column(s) that is/are indexed
4) Filtered indexes - filters placed on specific portions of the data that meets the criteria of the filter. Specifically on the WHERE clause

## Indexing strategies
1) Analyze queries executed on the columns and the commonly used clauses like WHERE, ORDER BY and JOIN.
2) Choose columns with unique values used in the clauses or in general
3) Evaluate data distribution - if it is unevenly distributed then an index may not help. In this case, consider composite indexes to improve selectivity (multiple columns)
4) Balance index size and query coverage - try to use only columns that are commonly used in queries to improve performance.

   
