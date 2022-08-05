- Upgrade postgresql from 9.6 to 10

`initdb --locale=C -E UTF8 --lc-ctype=UTF-8`

`pg_upgrade -b /usr/local/Cellar/postgresql@9.6/9.6.11/bin -B /usr/local/Cellar/postgresql/10.5/bin/ -d /usr/local/var/postgres.backup -D /usr/local/var/postgres`


- Export
  - `pg_dump -U username -h host db_name > exported_db.dump`
  - `pg_dump -U username -h host db_name > exported_db.pgsql`
  - schema only `pg_dump -U username -h host -s db_name > exported_db.pgsql`
  - data only `pg_dump -U username -h host -a db_name > exported_db.pgsql`

- Import

  - If file .dump `psql -U username -h host -d dbname < exported_db.dump`
  - `pg_restore -U username -h host -d dbname < exported_db.pgsql`
