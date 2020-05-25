# Mautic has been added to the one click apps. https://github.com/caprover/one-click-apps/blob/master/public/v2/apps/mautic.json

## What is [Mautic?](https://www.mautic.org/)

Mautic is an open marketing software platform that gives a high level of marketing integration with audience intelligence that enables you to make personalized emails, create landing pages, create intuitive workflows for customer experiences and the capabilities to track your marketing activities.

## This guide assumes that you have a running instance of [CapRover.](https://caprover.com/)

#### See link below for installation instructions

[CapRover install docs](https://caprover.com/docs/get-started.html/)

## 1. Create mysql database from one click apps

Replace environment variables (Only change password for db)
```
MAUTIC_DB_USER=root
MAUTIC_DB_NAME=mautic
MAUTIC_DB_PASSWORD=yourpassword

```
## 2. Create new app (check box: Has Persistent Data)

[Caprover Docs Connecting to Databases](https://caprover.com/docs/one-click-apps.html#connecting-to-databases/)

Add environmental variables
```
MAUTIC_DB_HOST=change-me 
MAUTIC_DB_USER=root
MAUTIC_DB_NAME=mautic
MAUTIC_RUN_CRON_JOBS=true
MAUTIC_DB_PASSWORD=yourpassword
```
Add persistent directory 
```
- Path: /var/www/html 
- Label: mautic-data
```

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

- CapRover for providing such an awesome environment to work in. (https://caprover.com/)
- The Mautic Team for creating an dockerized version. (https://github.com/mautic/docker-mautic)
- And a big shout out to Jeffrey Epstein for not killing himself. (https://en.wikipedia.org/wiki/Death_of_Jeffrey_Epstein)


