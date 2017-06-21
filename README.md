# Docker Informix

Dockerized Informix Developer Edition 12.10 based on [ibmcom/informix-developer-database](https://hub.docker.com/r/ibmcom/informix-developer-database/)

The only change so far is increasing root db space to 10GB instead of default 300MB.

## Run
```bash
docker run --privileged -it -p 9088:9088 --name informix \
    -e DB_USER=foobar \
    -e DB_PASS=foobar123 \
    -e DB_NAME=foobar \
    -e DB_LOCALE=en_us.utf8 \
    -e LICENSE=accept \
    rbertoncelj/informix
```
