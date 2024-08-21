## Partitioning
Why? 
- To make access of important data easier
- To help with storage

## Horizontal and Vertical Partitioning
**Horizontal**

**Vertical** 
- Increases query performance (full table scans)
- Reduce access times: Any large tables can be split into their own tables
- Restrict access sometimes (like sensitive data)
- TRIGGERS direct INSERTs to specific partitions
- VPs arent used widely
