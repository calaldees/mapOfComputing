Databases
=========

* [Build Your Own X From Scratch Books](https://build-your-own.org/)
    * [database](https://build-your-own.org/#section-database) [book_done](https://build-your-own.org/blog/20230420_byodb_done/)

* [how query engines work](https://howqueryengineswork.com/)
    * Good description of query (loads of step by step detail)
        * Like average over a dataset etc

* [[sql]]
    * [[sqlite]]
* [[nosql]]
* Vector Database's
    * [A Gentle Introduction to Vector Databases](https://frankzliu.com/2021/12/23/a_gentle_introduction_to_vector_databases.html)
        * Float for how related two items are

* Stackoverflow: [How does database indexing work?](https://stackoverflow.com/questions/1108/how-does-database-indexing-work)

https://www.prisma.io/blog/comparison-of-database-models-1iz9u29nwn37

* [42 things I learned from building a production database](https://maheshba.bitbucket.io/blog/2021/10/19/42Things.html)

Just use memory?

Redis?
200ms loss
Mongo(ohno)db
My(els)SQL -> MariaDB
Elastic Search (stemming -> plurals)
File system
S3?

Relication (cascade)

Test your backups

[[postgresql]]

in browser

* [drawsql.app](https://drawsql.app/templates) ER diagrams of open source projects

Activity Idea
-------------

generate SQL database relations and data based off a student name hash.
Ask questions (with known results)
Mark SQL compitence (no cheating)

* [geocode-sqlite](https://github.com/eyeseast/geocode-sqlite) - Geocode rows in a SQLite database table
    * take address and use web api to get lat/lon

Immutable - Zero Trust
----------------------

* [immudb](https://github.com/codenotary/immudb)





Object Relational Model (ORM) #orm
-----------------------

* [prisma.io](https://www.prisma.io/)
    * Next-generation Node.js and TypeScript ORM
    * Prisma helps app developers build faster and make fewer errors with an open source database toolkit for PostgreSQL, MySQL and SQLite.

Moving away from database api to data layer
-------------------------------------------

[[nosql]]

* [NoneSQL, All the DevEx](https://planetscale.com/blog/nonesql-all-the-devex)
    * Most products today are database focused
    * Database internals will eventually just not matter
    * Moving towards [[developer-experience]]
        * Migrations
        * Version control (for data)
        * user management

* [fauna.com](https://fauna.com/)
    * The data API for modern applications
    * Fauna is a flexible, developer-friendly, transactional database delivered as a secure and scalable cloud API with native GraphQL. Never again worry about database provisioning, scaling, sharding, replication, or correctness.
    * Think data, not database operations

---

* [Joins 13 Ways](https://justinjaffray.com/joins-13-ways/)
    * 13 different conceptual understandings of a JOIN in sql
    * A join is a nested loop over rows
    * A join is a lookup
    * A join is flatMap
    * A join is the solution to the N+1 problem
    * A join is paths through a graph
    * A join is typechecking


[//begin]: # "Autogenerated link references for markdown compatibility"
[sql]: sql.md "sql"
[sqlite]: sqlite.md "SQLite"
[nosql]: nosql.md "nosql"
[postgresql]: postgresql.md "PostgreSQL"
[developer-experience]: developer-experience.md "Developer Experience"
[//end]: # "Autogenerated link references"