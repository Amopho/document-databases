# document-databases
Exploring usage possibilities of noSql databases like MongoDB

## Advantages of Document databases
- no predefine schema
- flexible
- avoiding complicated migrations in case of any change
- intuitive, natural way to work with - JSON files are human readable
- maps through objects - less codingm simpler, fast
- storing objects as documents are created
- scalable by <strong>sharding</strong> technique. Horizontal scalability


Limitations
- more awareness on the data, checking twice before pkacing in the document
- redundant data - duplications, to optimize queries - odify the name (rmember to change everywhere)

## When to use them

- transactions, security controls, query engines.
- e-commerce web sites whicha re storing catalogs of their product information - thanks to polymorfic feature- different traits compare to other products. Moreover we one may embedded related addituional inforrmations. All of them would be retrieved with a single query
- event logging - user logging in, purchase, errors. Sharded. Sharding technique by: time, type of evenr.
- Storing user profiles- which may vary over time (comments...)
- real time analytics - page views, unique visitors...

## They are not suitable for
- if we already have structured data,
- when we want our data to be always consistent- document databases are not consistent. They change dynamically.

## MQL Mongo DB Query Language

- index on any field type
- offers ACID (Atomicity, Consistency, Isolation, Durability)
- can JOIN queries

### Features
- horizontal scaling
- replication, up to 50 data copies available

```
db.users.find({"address.zipcode": "10245"})
```

## Some advantages in replacing other DB (e.g. Oracle) with MongoDB
- improvement of the performance
- horizontal scaling
- flexible schema means quicker development (implementing tags, comments)
- new query patterns
- costs reduction

## Products
- Mongo DB Atlas - Cloud
- MongoDB Enterprise Advanced
- MongoDB Charts- Data Visualisation
- Realm Mobile Database

## Column family databases queries - Google BigTable data storage system

Also known as a wide column database. For dealing with a large volume of data.

Data storing in column families, that group together frequently accessed and  related data.

## Structure

Column family is like a table in relational SQL database

### Examples

- cassandra
- Apache Hbase
- accumulo
