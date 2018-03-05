# Docker Compose for Magento1 Development

## Project installation
***
_No need to create the database it's created when starting the containers._
Copy and rename .env.sample to .env and fill the contents

```bash
cd docker && docker-compose up -d
```
>The `-d` will make docker run in the background, leave this off when you want to debug or see the logs.

## Uninstall
***
_Remove the database directories inside the project_
```bash
cd docker && docker-compose down
sudo rm -Rf mysql/db_storage elastic-search/es_storage redis/redis_storage 
```

