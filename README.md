# docker-sqlite3

A sqlite3 client.

## Usage

```sh
touch ~/database.db

docker run \
-it \
--rm \
-v ~:/data \
sstc/sqlite3 \
sqlite3 database.db
```

```console
SQLite version 3.30.1 2019-10-10 20:19:45
Enter ".help" for usage hints.
sqlite> CREATE TABLE test (id INTEGER, name TEXT);
sqlite> .tables
test
sqlite> .exit
```
