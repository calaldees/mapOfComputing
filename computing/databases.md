https://www.prisma.io/blog/comparison-of-database-models-1iz9u29nwn37

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


in browser

* [drawsql.app](https://drawsql.app/templates) ER diagrams of open source projects

Activity Idea
-------------

generate SQL database relations and data based off a student name hash.
Ask questions (with known results)
Mark SQL compitence (no cheating)

* [geocode-sqlite](https://github.com/eyeseast/geocode-sqlite) - Geocode rows in a SQLite database table
    * take address and use web api to get lat/lon

PostgreSQL
----------

* [PostgreSQL beginner guide](https://knowledgepill.it/posts/postgresql-basics-guide/) - connecting, remote access, psql CLI and troubleshooting connection
* [Why you (probably) don't need PostGIS](https://blog.rebased.pl/2020/04/07/why-you-probably-dont-need-postgis)
* [psql command line tutorial and cheat sheet](https://tomcam.github.io/postgres/)
* [postgREST](https://github.com/PostgREST/postgrest)
* [Fuzzy Name Matching in Postgres](https://info.crunchydata.com/blog/fuzzy-name-matching-in-postgresql)
    * Levenshtein Matching - fuzzy string match
* [10 Things I Hate About PostgreSQL](https://rbranson.medium.com/10-things-i-hate-about-postgresql-20dbab8c2791)
    * Experienced data engineer talks about experiences with Postgres in production
* [pgvector](https://github.com/ankane/pgvector) - Open-source vector similarity search for Postgres 
* [PostGIS ](https://postgis.net/) - is a spatial database extender for PostgreSQL object-relational database. It adds support for geographic objects allowing location queries to be run in SQL. 

* [Things I Wished More Developers Knew About Databases](https://medium.com/@rakyll/things-i-wished-more-developers-knew-about-databases-2d0178464f78)

* [We Can Do Better Than SQL](https://edgedb.com/blog/we-can-do-better-than-sql/) - sql is not brilliant - here is why


SQLite
------

* [SQLite as a document database](https://dgl.cx/2020/06/sqlite-json-support)
    * insert JSON straight into SQLite and then have it extract data and index them