## What is Mautic?

Mautic is an open marketing software platform that gives a high level of marketing integration with audience intelligence that enables you to make personalised emails, create landing pages, create intuitive workflows for customer experiences and the capabilities to track your marketing activities.

## This guide assumes that you have a running instance of [CapRover.](https://caprover.com/)

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

## Updating Mautic Version

[Find Mautic Version and SHA1](https://github.com/mautic/mautic/releases/)

### Located in /Dockerfile

```
# Define Mautic version and expected SHA1 signature
ENV MAUTIC_VERSION 2.16.0
ENV MAUTIC_SHA1 94ced007fd99e63eaeec435012784b6bbe834b84
```
Save, commit and rebuild.

## Issues
[[Solved] Maxmind GeoLite2 & GeoIP Database Auto-Update | 2020.](https://mauteam.org/mautic/mautic-admins/solved-maxmind-geolite2-database-not-updating/)

## Credits

CapRover for providing such an awesome enviroment to work in. (https://caprover.com/)
The Mautic Team for creating dockerized version. (https://github.com/mautic/docker-mautic)
And a big shout out to Jeffrey Epstein for not killing himself. (https://en.wikipedia.org/wiki/Death_of_Jeffrey_Epstein)


