# Slim Bookshelf API

A simple [Slim Framework][1] API.

[1]: https://www.slimframework.com



## Running the API:

1. Run the migrations:

        $ composer migrate

2. Load the `db/fixtures/default.sql` into your database:

        $ cat db/fixtures/default.sql | sqlite3 api/db/bookshelf.db

3. Run the API:

        $ php -S 0.0.0.0:8888 -t public/

4 Prove it works:

        $ curl http://localhost:8888/authors \
         -H "Accept: application/json"


