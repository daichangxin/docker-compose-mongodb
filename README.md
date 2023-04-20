# Setup mongodb server

1. create keyfile

```
openssl rand -base64 756 >  .docker/mongo/keyfile.pem
```

2. create folder

`data/db`

3. up

```
docker-compose up -d
```
