# fastapi-pytest

https://www.jeffastor.com/blog/up-and-running-with-fastapi-and-docker


start the apps 

```
docker-compose up --build
```


To check contents of db 

```
docker-compose exec db psql -h localhost -U postgres --dbname=postgres

(base) anmolpal@Anmols-Air fastapi-pytest % docker-compose exec db psql -h localhost -U postgres --dbname=postgres
psql (13.11)
Type "help" for help.

postgres=# select id, name , price from cleanings;
 id | name | price
----+------+-------
(0 rows)
```


All Pydantic Models live in /app/models