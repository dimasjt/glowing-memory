- Upgrade postgresql from 9.6 to 10

`initdb --locale=C -E UTF8 --lc-ctype=UTF-8`

`pg_upgrade -b /usr/local/Cellar/postgresql@9.6/9.6.11/bin -B /usr/local/Cellar/postgresql/10.5/bin/ -d /usr/local/var/postgres.backup -D /usr/local/var/postgres`
