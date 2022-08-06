# nosql vs sql #

## Comparison between SQL and noSQL ##
| SQL | noSQL |
| ----------- | ----------- |
| primarily called as Relational Databases (RDBMS) | primarily called as non-relational or distributed database. |
| table based databases | document based, key-value pairs, graph databases or wide-column stores |
| predefined schema | dynamic schema for unstructured data |
| vertically scalable | horizontally scalable |
| uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful | queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database. |
| MySql, Oracle, Sqlite, Postgres and MS-SQL | MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb |
| good fit for the complex query intensive environment | not good fit for complex queries, don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language |
| not best fit for hierarchical data storage | fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.  |
| are vertically scalable | are horizontally scalable |
| best fit for heavy duty transactional type applications | transactions purpose, it is still not comparable and sable enough in high load and for complex transactional applications |
| Excellent support are available for all SQL database from their vendors | some NoSQL database you still have to rely on community support |
| emphasizes on ACID properties ( Atomicity, Consistency, Isolation and Durability) | follows the Brewers CAP theorem ( Consistency, Availability and Partition tolerance ) |
| either open-source or close-sourced from commercial vendors | can be classified on the basis of way of storing data as graph databases, key-value store databases, document store databases, column store database and XML databases. |


## Simple Comparison Table ## 
| SQL | noSQL |
| ----------- | ----------- |
| Data use Schemas | Schema-less |
| Relations | No/Few Relations |
| Data is distributed acroos multiple tables | Data is typically merged / nested in a few collections |
| Horizontal scaling is difficult/impossible; Vertical scalling is possible | Both horizontal and vertical scaling is possible |
| Limitaitons for lots of (thousands) read & write queries per second | Great performace for mass (simple) read & write requests |

## What kind of data is a good fit for an SQL database? ##
If your data is highly structured and associations among the program entities are clearly defined.

## Give a real world example. ##
for instance, if you are developing a point of sale system where you need to store customer orders and product records

## What kind of data is a good fit a NoSQL database? ##
large data with simple schema
 
## Give a real world example. ##
Social games are data-intensive applications that can explode from zero to millions of players literally overnight. That kind of rapid growth, both in terms of data volume and number of users, necessitates the right class of database to store all that information and scale to a growing user base. NoSQL provides scalability, consistently high performance, always-on 24×365 operations and a flexible data model. Some of the most popular social and mobile games come from the likes of Zynga, Electronic Arts, Tencent and Shuffle Master, which are all powered by NoSQL.

## Which type of database is best for hierarchical data storage? ##
noSQL

## Which type of database is best for scalability? ##
NoSQL, earning it's name by being “not only SQL” makes it easier to store all different types of data together. It's used for its flexibility and therefore speed and scalability in managing large volumes of data.


### *[Source](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)*  ###

<hr>
<hr>

# sql vs nosql  #

## What does SQL stand for? ##
Structured Query Language

**SELECT** id, name, price **FROM** products

- **bold** are SQL syntax / keywords
- normal are Data/Parameters

## What is a relational database? ##
we have a database which works with certain assumptions or in a certain way and it supports the sq language 

## What type of structure does a relational database work with? ##
Tables - like a storage container

## What is a ‘schema’? ##
when we query data with sql, we will have a very strict requirements for the data we store in our database table, it is also called fields

## What is a NoSQL database? ##
it is also called MongoDB which stands for Humongous because it can store lots and lots of data in a very effiecient way.

## How does it work? ##
we have data bases and we have collections instead of tables and inside it we have documents (rows and tables) they look like JSON and they dont have to use the same schema, we can have multiple documents in one collection which have different fields.

## What is inside of a Mongo database? ##


## Which is more flexible - SQL or MongoDB? and why. ##
MongoDB 
- You can add new data, and you want to fetch new data at some point, you can store them in the same collection.
- There is also no/few relations.

## What is the disadvantage of a NoSQL database? ##
You could have duplicated data, it needs to be updated

### *[Source](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)  ###

## Useful Resources ##
- [mongoose api](https://mongoosejs.com/docs/api.html#Model)
- [React Router](https://reactrouter.com/web/api/BrowserRouter)

<hr>
<hr>

## Things I want to know more about
