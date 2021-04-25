Data stored in relational databases are stored in tables.A table represents particular entity and columns in the table represent attributes of the entity. 
Data stored in the relational db is structured.Most of rel. DB support SQL that gives poweful quering capabilities.

Someone might argue that, we can use python or JS to query that data. But, when we are working on a large scale distributed system, we are dealing with terabytes of data. 
Loading that kind of data into memory will be non trivial.


SQL DB must use ACID transaction.
Atomicity->If a transaction consists of multiple operations, either they all succed or they all fail. If one of 'em fails, all fail.transaction is rolledback.(commit)
Consistency-> There will be mo stale state in the database. Any future transaction takes past transaction into account.
Isolation-> Transactions are able to be done concurrently, but, they will be done swquentially.
Durability-> When you make transaction, that transaction is permanent. Data stored in the database is stored in the disc.

DB index->A database index is a data structure that improves the speed of data retrieval operations on a database table at the cost of additional writes and storage space to maintain the index data structure.
Indexes are used to quickly locate data without having to search every row in a database table every time a database table is accessed.
Indexes can be created using one or more columns of a database table, providing the basis for both rapid random lookups and efficient access of ordered records.
An index is a copy of selected columns of data, from a table, that is designed to enable very efficient search. An index normally includes a "key" or direct link to the original
row of data from which it was copied, to allow the complete row to be retrieved efficiently. Some databases extend the power of indexing by letting developers create indexes on
column values that have been transformed by functions or expressions.
Creating index is creating auxialiary data structure.
