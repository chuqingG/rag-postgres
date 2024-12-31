# Start

```bash
# init a new data store
initdb -D /ssd_root/gao688/rag_db

# start the server and set log path
pg_ctl -D /ssd_root/gao688/rag_db -l /ssd_root/gao688/log/pgserver.log start
# the db we have
psql -d azrag

# install pgvector
sudo apt install postgresql-16-pgvector

CREATE EXTENSION IF NOT EXISTS vector;


```

Before build the frontend, the node version need to >= 18.0.0