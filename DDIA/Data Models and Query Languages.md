# Data models
### Relational Model vs Document Model
- Relational databases come from needing business data processing
- Other databases back in the day required developers to think about the arrangement of data in the database
### NoSQL
- greater scalability including very large datasets or very high write throughput
- preference for free and open source software
- specialized query operations not supported by a relational model
- to avoid the restrictiveness of a relational schema
### Object Relational Mismatch
- if data is in relational tables, a translation layer is needed between objects in the application code and database model - 'impedance mismatch'
- Object relational mapping frameworks reduce amount of differences between two models
- JSON has some flexibility since all the data is in one place than a multi table schema and reduces impedance mismatch to a degree

### Many to One and Many to Many Relationships
- Information may require changes in the future, hence involve removing duplicate copies. This means write overheads and data inconsistency during updation. All this is avoided by **Normalization**.
- Normalizing data means many-to-one relationships but these don't fit well with the document model since Joins arent very well supported (some do support like RethinkDB)
- The onus of Joins are on the application code instead of the document database itself and hence, multiple queries need to be made on the database

- IBM's Information Management System (IMS) used a hierarchical model (which are like JSON storage of data) but it couldn't solve the problem of many-to-many relationships and didn't support Joins.
- Solutions to the hierarchical model were the *relational model* and *network model* (which is obscure now)

### Network model
- **CODASYL** - tree structure - a different entities were stored as a path of a record - in may-to-many relationships, when the entity was a part of multiple records, CODASYL would traverse through all the paths and make a store of the traversed paths -> became a traversal problem in a n-dimensional space

### Relational model
- Query optimizer is the 'access path' decider and hence not done on the application layer

### Document model
- Document DBs have one thing in common with network DBs which is that they store nested records within their parent records instead of in a separate table
- document references are like foreign keys which enable JOINs in document DBs
- not strict on schema 



