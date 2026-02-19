SQL
---

* [SQL Police Department Exercises](https://sqlpd.com/)

* [SQL CheatSheet](https://devhints.io/mysql)

* [Write an SQL query builder in 150 lines of Python!](https://death.andgravity.com/query-builder-how) [[python]] [[design-patterns]] #orm

* [How We Went All In on sqlc/pgx for Postgres + Go](https://brandur.org/sqlc) #golang #orm
    * [gtihub.com/*/sqlc](https://github.com/kyleconroy/sqlc)
        * Write SQL and compile the statements to typesafe Golang

* [sqlite.org/fiddle](https://sqlite.org/fiddle/)
* SQLite[JSONB has landed](https://sqlite.org/forum/forumpost/fa6f64e3dc1a5d97) - json is kept in an internal binary format for performnce
* [sqlite-web](https://github.com/coleifer/sqlite-web)
    * `pip install sqlite-web` `sqlite_web /path/to/database.db` `open https://localhost:8080`

* [TailwindSQL](https://github.com/mmarinovic/tailwindsql)
    * TailwindSQL lets you write SQL queries using Tailwind-style class names. Just use className to query your database directly in React Server Components!
    * ```
        // Fetch and render a user's name
        <DB className="db-users-name-where-id-1" />
        // Renders: "Ada Lovelace"

        // Render products as a list
        <DB className="db-products-title-limit-5" as="ul" />
        // Renders: <ul><li>Mechanical Keyboard</li>...</ul>

        // Order by price and show as table
        <DB className="db-products-orderby-price-desc" as="table" />
       ```

* [[sqlite]]



[python]: python.md "python3"
[design-patterns]: design-patterns.md "Design patterns"
[sqlite]: sqlite.md "SQLite"

