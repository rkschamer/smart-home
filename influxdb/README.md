# influxdb

Connect to container and execute shell.

## Login

```bash
influx -username <user> -password <password>
```

## Databases

```sql
CREATE DATABASE "telegraf" WITH DURATION 7d
CREATE DATABASE "dresden-sensors" WITH DURATION 30d
```

## Users

```sql
CREATE USER "telegraf" WITH PASSWORD '<password>';
GRANT ALL ON "telegraf" TO telegraf;
CREATE USER "sensors" WITH PASSWORD '<password>';
GRANT ALL ON "dresden-sensors" TO sensors;
```
