# Database instructions
## H2 In-Memory Database
## MySQL Database
### Check if data is added to H2 In-Memory Database using the Command Line Interface (CLI)
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
```
show databases;
```
```
use servers;
```
```
show tables;
```
```
desc server;
```
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
## DBeaver Universal Database client
