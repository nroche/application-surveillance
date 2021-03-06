# application-surveillance
A demo project to show how to setup a **Telegraf-InfluxDB-Grafana** application surveillance tool. The aim is both to monitor and help diagnose issues.

## Prerequisite

You need to have Docker and Docker Compose installed on your machine to use this project (Java might also be necessary if you want to run the PostgreSQL ping demo application). Otherwise, you need to manually install all the technical components.

## Technical stack

* Java;
* Docker;
* Grafana;
* InfluxDB;
* Telegraf;
* PostgreSQL.

**Remember to change the default passwords before running something based on this project in production ;) !!!**

## Presentations

* [French presentation](presentation/presentation_fr.adoc).

## Helpful commands

* To build the PostgreSQL ping demo application : 

```mvnw clean install```

```docker build -t postgres-ping .```
* Start : ```docker-compose up -d```

Access demo links via : http://localhost

The default Grafana user is **admin/admin**.

* Stop : ```docker-compose stop```
* View the logs : ```docker-compose logs```
* Remove the Docker containers : ```docker-compose rm```. Emptying the storage and log directories can be helpful.

## Extra links

* PgAdmin : http://localhost:5050 pgadmin4@pgadmin.org / admin (the PostgreSQL server can be found at "postgres", not (127.0.0.1))
