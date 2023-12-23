Created API with docker container and postgre
1. Setup env
DB_CONNECTION=pgsql
DB_HOST=db
DB_PORT=5432
DB_DATABASE=qlope_db
DB_USERNAME=postgres
DB_PASSWORD=postgres

2. If you found refused connection while do migration file
Execute this syntax docker-compose exec {PHP_SERVICE} bash

3. Dont forget give all privileges on user database
create user postgres with password 'postgres';
grant all privileges on qlope_db to postgres;