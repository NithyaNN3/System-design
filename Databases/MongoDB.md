## Other Concepts - 
### Partial matching 
- use /<word>/ as a value. Example: 

```
// Query
db.users.find({ name: /like/ })

// Result
;[
  {
    email: 'one@email.com',
    name: 'One for like and comment',
  },
]
```

### Aggregations on Compass
- Performs a function on multiple documents
- groups values from multiple documents together
- aggregation pipelines to perform multiple sequence of tasks on data 
- essentially running queries in a sequence - result of one query is used for another query and so on - done in different stages

### $lookup() 
- under Aggregations
- [MongoDB Lookups](https://docs.mongodb.com/manual/reference/operator/aggregation/lookup)
