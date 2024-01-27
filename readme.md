Commands runned:

```bash
docker run -it   -e POSTGRES_USER="root"   -e POSTGRES_PASSWORD="root"   -e POSTGRES_DB="ny_taxi"   -v /c/Users/Devboti/Documents/TI/data_engineering_zoomcamp/data_ny_taxi:/var/lib/postgresql/data   -p 5432:5432 --network=pg-network --name pg-database   postgres:13
```

```bash
pgcli -h localhost -p 5432 -u root -d ny_taxi
```

```bash
pip install jupyter

jupyter notebook
```

```bash
docker network create pg-network
```

```bash
docker run -it \
-e PGADMIN_DEFAULT_EMAIL="admin@admin.com" \
-e PGADMIN_DEFAULT_PASSWORD="root" \
-p 8080:80 \
--network=pg-network \
--name pgadmin-2 \
dpage/pgadmin4
```