# Database instructions
## H2 In-Memory Database
## MySQL Database
### Check if data is added to MySQL Database using the Command Line Interface (CLI)
Position yourself using **Command Line Interface (CLI)** in the folder where `docker-compose.yml` file is:
```
cd DOCKER-COMPOSE_FILE_PATH
```
Check if data is added to MySQL Database using the **Command Line Interface (CLI)**
```
docker exec -ti mysql bash
```
```
mysql -u sa -h localhost -p
```
```
Enter password: zgadija
```
Show all the databases:
```
show databases;
```
Choose your database:
```
use servers;
```
Show all the tables in the chosen database:
```
show tables;
```
```
desc server;
```
Show all the data in a table:
```
TABLE server;
```
```
SELECT * FROM server;
```
```
exit
```
```
exit
```
## PostgreSQL Database
### Check if data is added to PostgreSQL Database using the Command Line Interface (CLI)
Position yourself using **Command Line Interface (CLI)** in the folder where `docker-compose.yml` file is:
```
cd DOCKER-COMPOSE_FILE_PATH
```
Check if data is added to PostgreSQL Database using the **Command Line Interface (CLI)**
```
docker exec -ti postgres bash
```
```
psql -h localhost -p 5432 -U sa postgres -W
```
```
Password: zgadija
```
Show all the databases:
```
\l
```
Choose your database:
```
\c database_name
```
```
\c servers
```
```
Password: zgadija
```
Show all the tables in the chosen database:
```
\dt
```
Show all the data in a table:
```
TABLE server;
```
```
SELECT * FROM server;
```
```
exit
```
```
exit
```
## DBeaver Universal Database client
