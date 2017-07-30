# docker-sqlite3
A sqlite3 client.

## Usage

```sh
docker run \
-it \
--rm \
-v ~/database.db:/data/database.db \
sstc/sqlite3 \
sqlite3 database.db
```

```
SQLite version 3.18.0 2017-03-28 18:48:43
Enter ".help" for usage hints.
sqlite> .tables
co_art_map       co_container     co_session       co_username_log
co_block         co_entity        co_sign          co_version     
co_chat          co_entity_map    co_skull         co_world       
co_command       co_material_map  co_user        
sqlite> .exit
```