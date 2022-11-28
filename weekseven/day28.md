<aside>
🔐 What role do ORM like Sequelize, and Database like MySQL have respectively?

</aside>

Sequelize is a promise-based ORM for Node.js and io.js. It supports the dialects PostgreSQL, MySQL, MariaDB, SQLite and MSSQL and features solid transaction support, relations, read replication and more.

Sequelize will setup a connection pool on initialization so you should ideally only ever create one instance per database.

Sequelize only provides ORM, to interact with a database, a database driver is still needed, like mysql2. In sequelize, database tables are referred as models. A model is an abstraction that represents a table in the database. To create a database connection, put the database name, username and password in an environment variable.