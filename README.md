# docker-sqlite3

A dockerized [sqlite3](https://www.sqlite.org/index.html) client.

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
Enter ".help" for usage hints.
sqlite> CREATE TABLE test (id INTEGER, name TEXT);
sqlite> .tables
test
sqlite> .exit
```
