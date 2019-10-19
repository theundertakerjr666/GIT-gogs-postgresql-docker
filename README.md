## Gogs and Postgres Docker Compose
### Run
---
0. Clone repository and create folder `data/gogs` and `data/postgres`
1. Run `docker-compose up -d` to run docker compose.
2. Check that your Gogs application is running enter url `http://localhost:10800`.
3. Check postgres docker container is running at localhost:5432.
4. Initialise your Gogs application at `http://localhost:10800`, choose PostgreSQL as your database, Host: `x.x.x.x:5432`, User:`gogs`, Password:`changeme`, Database Name:`gogs`. You can define these in `docker-compose.yaml`.

### Reset/Delete docker images and data
---

1. Run `docker-compose stop` to stop Gogs and postgresql containers.
2. Run `docker-compose rm -f` to remove Gogs and postgresql containers.
3. Run `./cleanup.sh` if you want remove Gogs and postgresql data.
