# Metabase and Postgres

To run containers add `db_password.txt` to current directory with password to database.

Then run 

`docker compose up -d`

After launching containers Metabase will be available at http://localhost:3000, Postgres DB will be available at `localhost:5432` having postgres `database` and `postgres` user.

To stop and delete containers run

`docker compose down`

Persistent volume `postgres_db_volume` will keep data base file for a net run.