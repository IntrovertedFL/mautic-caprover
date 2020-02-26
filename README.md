# 1. Create mysql database from one click apps

Replace enviroment variables (Only change password for db)
```
MAUTIC_DB_USER=root
MAUTIC_DB_NAME=mautic
MAUTIC_DB_PASSWORD=yourpassword

```
# 2. Create new app (check box: Has Persistent Data)

Add enviromental variables
```
MAUTIC_DB_HOST=change-me
MAUTIC_DB_USER=root
MAUTIC_DB_NAME=mautic
MAUTIC_RUN_CRON_JOBS=true
MAUTIC_DB_PASSWORD=yourpassword
```
Add persistant directory /var/www/html

# 3. Fork or clone this repo and configure auto deploy in caprover. Push enjoy.

