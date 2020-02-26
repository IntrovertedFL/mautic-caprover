
## This guide assumes you have a running instance of CapRover.

[CapRover install docs](https://caprover.com/docs/get-started.html/)

## 1. Create mysql database from one click apps

Replace enviroment variables (Only change password for db)
```
MAUTIC_DB_USER=root
MAUTIC_DB_NAME=mautic
MAUTIC_DB_PASSWORD=yourpassword

```
## 2. Create new app (check box: Has Persistent Data)

[Caprover Docs Connecting to Databases](https://caprover.com/docs/one-click-apps.html#connecting-to-databases/)

Add enviromental variables
```
MAUTIC_DB_HOST=change-me 
MAUTIC_DB_USER=root
MAUTIC_DB_NAME=mautic
MAUTIC_RUN_CRON_JOBS=true
MAUTIC_DB_PASSWORD=yourpassword
```
Add persistant directory /var/www/html

Fork or clone this repo and configure auto deploy in caprover. Push enjoy.

## Issues
[[Solved] Maxmind GeoLite2 & GeoIP Database Auto-Update | 2020.](https://mauteam.org/mautic/mautic-admins/solved-maxmind-geolite2-database-not-updating/)
