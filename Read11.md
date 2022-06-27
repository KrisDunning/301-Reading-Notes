[Return to Course 301 Notes](https://KrisDunning.github.io/301-Reading-Notes)

-----

# Reading 11- Mongo and Mongoose

We will be using monDB amd mongoose in class as our DB. This will give us a overview of DB's strength and weaknesses.



## Reading NoSQL vs SQL

Five differences between SQL and NoSQL databases:

### SQL

- Relational Database
- Table based databases
- Predefined Schema
- Vertically scalable
- SQL lanquage

### NoSQL

- Non-relational Database(distributed)
- Document based databases
- Dynamic Schema
- Horizontal scalable
- UnSQL language

> What kind of data is a good fit for an SQL database?

- Complex query intensive environment. Heavy duty transactional type apps. 

> Give a real world example.

- MySQL, Postgres

> What kind of data is a good fit a NoSQL database?

- Heirarchical data storage, key-value like JSON.

> Give a real world example.

- MongoDB,Redis,CouchDB

> Which type of database is best for hierarchical data storage?

- NoSQL

> Which type of database is best for scalability?

- NOSQL

## Video SQL vs NoSQL

> What does SQL stand for?

- Structured Query Language

> What is a relational database?

- DB works with tables. Table is a databin, a storage container.

> What type of structure does a relational database work with?

-Tables. Schema contains fields, rules how data can be stored or accessed.

> What is a ‘schema’?

- a set of data or properties that all records must have an entry for. even if it is just an empty string.

> What is a NoSQL database?

- a database that uses collections and does not need to adhere to a strict schema

> How does it work?

- uses collections and documents to store sets of data that can be stored in one place. Can pull that information as needed. 

> What is inside of a Mongo database?

- database that has collections which has documents. 

> Which is more flexible - SQL or MongoDB? and why.

- MongoDB. No strict schemas.

> What is the disadvantage of a NoSQL database?

- Not sure if all data adheres to your format. Also may have duplicate data. Have to update info in multiple locations if there are duplicates. 

## Things I want to know more about

MongoDB good for many reads of data. Scales wide and no strict schema. But the flexibility usually requires a mental/design structure. How should collections/documents be ordered to minimize complexity? 

-----
