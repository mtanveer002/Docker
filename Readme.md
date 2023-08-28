# Setup Instructions

Remove .git directory from docker/.git use `rm docker/.git -rf`

1. Clone package to your project root and open terminal.

2. go to docker folder `cd docker or cd .docker`. (you can also make a copy of your docker folder as .docker and change or modify Dockerfile. Your docker folder remain original)

3. Update your project configurations in .env file and docker/.env file.

`COMPOSE_PROJECT_NAME=Project_name`
`HTTP_PORT=8085` localhost port. your project will live at http://locaclhost:8085 
`HTTPS_PORT=443`
`MYSQL_PORT=3385`

`MYSQL_DATABASE=database_name`
`MYSQL_ROOT_PASSWORD=root`

You can change compose_project_name, port, database name and database password. and same value put in your project .env. Do not wrap values in single or double quoutes. 

4. Run `docker-compose build` or `docker compose build`.

5. Run `docker-compose up` or `docker compose up`.

6. If necessory you can make updated to docker-compose and docker file too.

7. supervisor is included in this configurations and you can add more files to super visor directory. A sample config file is already included.
