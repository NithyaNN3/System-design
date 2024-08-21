## Partitioning
Why? 
- To make access of important data easier
- To help with storage

## Horizontal and Vertical Partitioning
**Horizontal**
- Used when there are a large number of rows
- most common
- same columns in every partition
- Full table scans are limited to full partition scans - can add localised indexes
- Partitioning BY range, list or hash
- Range partitions are based on dates and distance, etc
- List partitions are based on states, countries, sales regions, products, etc
- Hash partitions are based on numeric values or strings, when no logical groupings are obvious. Use of modulus determines which partition the data goes to.
- Downside to hash partitions is that you can't make new partitions afterwards

**Vertical** 
- Used with very wide tables esp. with [CLOBs or BLOBs](https://www.ibm.com/docs/en/informix-servers/12.10?topic=types-clob-blob-data)
- Increases query performance (full table scans)
- Reduce access times: Any large tables can be split into their own tables
- Restrict access sometimes (like sensitive data)
- TRIGGERS direct INSERTs to specific partitions
- VPs arent used widely

Partitioning with [PostgreSQL](https://www.postgresql.org/docs/9.1/ddl-partitioning.html)

## Partitioning Steps
1) Make a partition function: in SQL server for example, CREATE PARTITION FUNCTION [myDateRange] (datetime)
2) Use a partitioning scheme: basically what columns are to be used, etc
3) Create the partitioned table based on the scheme
