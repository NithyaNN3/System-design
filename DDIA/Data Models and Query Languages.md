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

### Many to One and May to Many Relationships
