# MySQL Server in Docker

Run MySQL Server in Docker for local development.

### Configs

Create a config file `configs/config.env` by copying from `configs/config.env.example`, and update environment values.

```bash
# create new config file
cp configs/config.env.example configs/config.env

# update config values
MYSQL_IMAGE_TAG=8.4
MYSQL_PORT=3306
MYSQL_DATABASE=mysqldb
```

### Secrets

Create three secret files inside `secrets/` directory, and add values to them.

- msyql-root-password.txt
- mysql-user.txt
- mysql-pass.txt

### Run Commands

```bash
# start mysql server
task dc-up

# stop mysql server
task dc-stop

# remove mysql server
task dc-down

# show container logs
task dc-logs
```
